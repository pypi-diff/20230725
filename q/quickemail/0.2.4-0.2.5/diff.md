# Comparing `tmp/quickemail-0.2.4-py3-none-any.whl.zip` & `tmp/quickemail-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8562 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    27312 b- defN 21-May-25 06:05 quickemail.py
--rw-rw-rw-  2.0 fat     3086 b- defN 21-May-25 06:08 quickemail-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 21-May-25 06:08 quickemail-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 21-May-25 06:08 quickemail-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      381 b- defN 21-May-25 06:08 quickemail-0.2.4.dist-info/RECORD
-5 files, 30882 bytes uncompressed, 7854 bytes compressed:  74.6%
+Zip file size: 8593 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    28615 b- defN 23-Jul-25 06:52 quickemail.py
+-rw-rw-rw-  2.0 fat     3170 b- defN 23-Jul-25 06:55 quickemail-0.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-25 06:55 quickemail-0.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-25 06:55 quickemail-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      381 b- defN 23-Jul-25 06:55 quickemail-0.2.5.dist-info/RECORD
+5 files, 32269 bytes uncompressed, 7885 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: quickemail.py
 Comment: 
 
-Filename: quickemail-0.2.4.dist-info/METADATA
+Filename: quickemail-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: quickemail-0.2.4.dist-info/WHEEL
+Filename: quickemail-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: quickemail-0.2.4.dist-info/top_level.txt
+Filename: quickemail-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: quickemail-0.2.4.dist-info/RECORD
+Filename: quickemail-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quickemail.py

```diff
@@ -1,33 +1,32 @@
 # -*- coding: utf-8 -*-
 
 import os
-import sys
 import smtplib
 from email.mime.text import MIMEText
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.header import Header
 from email.utils import parseaddr, formataddr, formatdate
 from email import encoders
-import base64 
+import base64
 import time
 import random
 
 __doc__ = """
     
     简易的邮件发信工具。支持认证/不认证发信。
     使用UTF-8编码。
     from quickemail import QuickEmail
 
     1. 发信前先定义发信要素：
 
         指定主机和端口，必须参数：
         quicksend = QuickEmail('mail.test.com', 25)    # SMTP发信端口，默认是25 SSL链接使用465
-
+        quicksend.debug = True                         # 打开调试
         定义HELO主机名，参数可省略：
         quicksend.helo = 'QuickEmail'                 # HELO主机名不能使用有空格的字符串
 
         认证用户名和密码，authsend()必须的参数：
         quicksend.mail_user = 'a'                     # 认证用户名
         quicksend.user_pass = 'test'                  # 认证用户的密码
 
@@ -59,373 +58,359 @@
 
         quicksend.authsend(msg)
         quicksend.send(msg)
     
     4. 错误显示 (成功返回True，失败返回错误说明字符串)
 
         result = quicksend.authsend(msg)
-        if result != True:
+        if result:
             print(result)
             
         result = quicksend.send(msg)
-        if result != True:
+        if result:
             print(result)
 
 """
 
 __version__ = '0.2.4'
 
 __author__ = 'clayboy <clayboy@foxmail.com>'
 
+
 class QuickEmail:
-    
     _content_type = {
-    'acp':'audio/x-mei-aac',
-    'aif':'audio/aiff',
-    'aiff':'audio/aiff',
-    'asa':'text/asa',
-    'asp':'text/asp',
-    'au':'audio/basic',
-    'awf':'application/vnd.adobe.workflow',
-    'bmp':'application/x-bmp',
-    'c4t':'application/x-c4t',
-    'cal':'application/x-cals',
-    'cdf':'application/x-netcdf',
-    'cel':'application/x-cel',
-    'cg4':'application/x-g4',
-    'cit':'application/x-cit',
-    'cml':'text/xml',
-    'cmx':'application/x-cmx',
-    'crl':'application/pkix-crl',
-    'csi':'application/x-csi',
-    'cut':'application/x-cut',
-    'dbm':'application/x-dbm',
-    'dcd':'text/xml',
-    'der':'application/x-x509-ca-cert',
-    'dib':'application/x-dib',
-    'doc':'application/msword',
-    'drw':'application/x-drw',
-    'dwf':'Model/vnd.dwf',
-    'dwg':'application/x-dwg',
-    'dxf':'application/x-dxf',
-    'emf':'application/x-emf',
-    'ent':'text/xml',
-    'eps':'application/x-ps',
-    'etd':'application/x-ebx',
-    'fax':'image/fax',
-    'fif':'application/fractals',
-    'frm':'application/x-frm',
-    'gbr':'application/x-gbr',
-    'gif':'image/gif',
-    'gp4':'application/x-gp4',
-    'hmr':'application/x-hmr',
-    'hpl':'application/x-hpl',
-    'hrf':'application/x-hrf',
-    'htc':'text/x-component',
-    'html':'text/html',
-    'htx':'text/html',
-    'ico':'image/x-icon',
-    'iff':'application/x-iff',
-    'igs':'application/x-igs',
-    'img':'application/x-img',
-    'isp':'application/x-internet-signup',
-    'java':'java/*',
-    'jpe':'image/jpeg',
-    'jpeg':'image/jpeg',
-    'jpg':'application/x-jpg',
-    'jsp':'text/html',
-    'lar':'application/x-laplayer-reg',
-    'lavs':'audio/x-liquid-secure',
-    'lmsff':'audio/x-la-lms',
-    'ltr':'application/x-ltr',
-    'm2v':'video/x-mpeg',
-    'm4e':'video/mpeg4',
-    'man':'application/x-troff-man',
-    'mdb':'application/msaccess',
-    'mfp':'application/x-shockwave-flash',
-    'mhtml':'message/rfc822',
-    'mid':'audio/mid',
-    'mil':'application/x-mil',
-    'mnd':'audio/x-musicnet-download',
-    'mocha':'application/x-javascript',
-    'mp1':'audio/mp1',
-    'mp2v':'video/mpeg',
-    'mp4':'video/mpeg4',
-    'mpd':'application/vnd.ms-project',
-    'mpeg':'video/mpg',
-    'mpga':'audio/rn-mpeg',
-    'mps':'video/x-mpeg',
-    'mpv':'video/mpg',
-    'mpw':'application/vnd.ms-project',
-    'mtx':'text/xml',
-    'net':'image/pnetvue',
-    'nws':'message/rfc822',
-    'out':'application/x-out',
-    'p12':'application/x-pkcs12',
-    'p7c':'application/pkcs7-mime',
-    'p7r':'application/x-pkcs7-certreqresp',
-    'pc5':'application/x-pc5',
-    'pcl':'application/x-pcl',
-    'pdf':'application/pdf',
-    'pdx':'application/vnd.adobe.pdx',
-    'pgl':'application/x-pgl',
-    'pko':'application/vnd.ms-pki.pko',
-    'plg':'text/html',
-    'plt':'application/x-plt',
-    'png':'application/x-png',
-    'ppa':'application/vnd.ms-powerpoint',
-    'pps':'application/vnd.ms-powerpoint',
-    'ppt':'application/x-ppt',
-    'prf':'application/pics-rules',
-    'prt':'application/x-prt',
-    'ps':'application/postscript',
-    'pwz':'application/vnd.ms-powerpoint',
-    'ra':'audio/vnd.rn-realaudio',
-    'ras':'application/x-ras',
-    'rdf':'text/xml',
-    'red':'application/x-red',
-    'rjs':'application/vnd.rn-realsystem-rjs',
-    'rlc':'application/x-rlc',
-    'rm':'application/vnd.rn-realmedia',
-    'rmi':'audio/mid',
-    'rmm':'audio/x-pn-realaudio',
-    'rms':'application/vnd.rn-realmedia-secure',
-    'rmx':'application/vnd.rn-realsystem-rmx',
-    'rp':'image/vnd.rn-realpix',
-    'rsml':'application/vnd.rn-rsml',
-    'rtf':'application/msword',
-    'rv':'video/vnd.rn-realvideo',
-    'sat':'application/x-sat',
-    'sdw':'application/x-sdw',
-    'slb':'application/x-slb',
-    'slk':'drawing/x-slk',
-    'smil':'application/smil',
-    'snd':'audio/basic',
-    'sor':'text/plain',
-    'spl':'application/futuresplash',
-    'ssm':'application/streamingmedia',
-    'stl':'application/vnd.ms-pki.stl',
-    'sty':'application/x-sty',
-    'swf':'application/x-shockwave-flash',
-    'tg4':'application/x-tg4',
-    'tif':'image/tiff',
-    'tiff':'image/tiff',
-    'top':'drawing/x-top',
-    'tsd':'text/xml',
-    'uin':'application/x-icq',
-    'vcf':'text/x-vcard',
-    'vdx':'application/vnd.visio',
-    'vpg':'application/x-vpeg005',
-    'vsd':'application/x-vsd',
-    'vst':'application/vnd.visio',
-    'vsw':'application/vnd.visio',
-    'vtx':'application/vnd.visio',
-    'wav':'audio/wav',
-    'wb1':'application/x-wb1',
-    'wb3':'application/x-wb3',
-    'wiz':'application/msword',
-    'wk4':'application/x-wk4',
-    'wks':'application/x-wks',
-    'wma':'audio/x-ms-wma',
-    'wmf':'application/x-wmf',
-    'wmv':'video/x-ms-wmv',
-    'wmz':'application/x-ms-wmz',
-    'wpd':'application/x-wpd',
-    'wpl':'application/vnd.ms-wpl',
-    'wr1':'application/x-wr1',
-    'wrk':'application/x-wrk',
-    'ws2':'application/x-ws',
-    'wsdl':'text/xml',
-    'xdp':'application/vnd.adobe.xdp',
-    'xfd':'application/vnd.adobe.xfd',
-    'xhtml':'text/html',
-    'xls':'application/x-xls',
-    'xml':'text/xml',
-    'xq':'text/xml',
-    'xquery':'text/xml',
-    'xsl':'text/xml',
-    'xwd':'application/x-xwd',
-    'sis':'application/vnd.symbian.install',
-    'x_t':'application/x-x_t',
-    'apk':'application/vnd.android.package-archive',
-    'tif':'image/tiff',
-    '0.301':'application/x-301',
-    '0.906':'application/x-906',
-    'a11':'application/x-a11',
-    'ai':'application/postscript',
-    'aifc':'audio/aiff',
-    'anv':'application/x-anv',
-    'asf':'video/x-ms-asf',
-    'asx':'video/x-ms-asf',
-    'avi':'video/avi',
-    'biz':'text/xml',
-    'bot':'application/x-bot',
-    'c90':'application/x-c90',
-    'cat':'application/vnd.ms-pki.seccat',
-    'cdr':'application/x-cdr',
-    'cer':'application/x-x509-ca-cert',
-    'cgm':'application/x-cgm',
-    'class':'java/*',
-    'cmp':'application/x-cmp',
-    'cot':'application/x-cot',
-    'crt':'application/x-x509-ca-cert',
-    'css':'text/css',
-    'dbf':'application/x-dbf',
-    'dbx':'application/x-dbx',
-    'dcx':'application/x-dcx',
-    'dgn':'application/x-dgn',
-    'dll':'application/x-msdownload',
-    'dot':'application/msword',
-    'dtd':'text/xml',
-    'dwf':'application/x-dwf',
-    'dxb':'application/x-dxb',
-    'edn':'application/vnd.adobe.edn',
-    'eml':'message/rfc822',
-    'epi':'application/x-epi',
-    'eps':'application/postscript',
-    'exe':'application/x-msdownload',
-    'fdf':'application/vnd.fdf',
-    'fo':'text/xml',
-    'g4':'application/x-g4',
-    '':'application/x-',
-    'gl2':'application/x-gl2',
-    'hgl':'application/x-hgl',
-    'hpg':'application/x-hpgl',
-    'hqx':'application/mac-binhex40',
-    'hta':'application/hta',
-    'htm':'text/html',
-    'htt':'text/webviewhtml',
-    'icb':'application/x-icb',
-    'ico':'application/x-ico',
-    'ig4':'application/x-g4',
-    'iii':'application/x-iphone',
-    'ins':'application/x-internet-signup',
-    'IVF':'video/x-ivf',
-    'jfif':'image/jpeg',
-    'jpe':'application/x-jpe',
-    'jpg':'image/jpeg',
-    'js':'application/x-javascript',
-    'la1':'audio/x-liquid-file',
-    'latex':'application/x-latex',
-    'lbm':'application/x-lbm',
-    'ls':'application/x-javascript',
-    'm1v':'video/x-mpeg',
-    'm3u':'audio/mpegurl',
-    'mac':'application/x-mac',
-    'math':'text/xml',
-    'mdb':'application/x-mdb',
-    'mht':'message/rfc822',
-    'mi':'application/x-mi',
-    'midi':'audio/mid',
-    'mml':'text/xml',
-    'mns':'audio/x-musicnet-stream',
-    'movie':'video/x-sgi-movie',
-    'mp2':'audio/mp2',
-    'mp3':'audio/mp3',
-    'mpa':'video/x-mpg',
-    'mpe':'video/x-mpeg',
-    'mpg':'video/mpg',
-    'mpp':'application/vnd.ms-project',
-    'mpt':'application/vnd.ms-project',
-    'mpv2':'video/mpeg',
-    'mpx':'application/vnd.ms-project',
-    'mxp':'application/x-mmxp',
-    'nrf':'application/x-nrf',
-    'odc':'text/x-ms-odc',
-    'p10':'application/pkcs10',
-    'p7b':'application/x-pkcs7-certificates',
-    'p7m':'application/pkcs7-mime',
-    'p7s':'application/pkcs7-signature',
-    'pci':'application/x-pci',
-    'pcx':'application/x-pcx',
-    'pdf':'application/pdf',
-    'pfx':'application/x-pkcs12',
-    'pic':'application/x-pic',
-    'pl':'application/x-perl',
-    'pls':'audio/scpls',
-    'png':'image/png',
-    'pot':'application/vnd.ms-powerpoint',
-    'ppm':'application/x-ppm',
-    'ppt':'application/vnd.ms-powerpoint',
-    'pr':'application/x-pr',
-    'prn':'application/x-prn',
-    'ps':'application/x-ps',
-    'ptn':'application/x-ptn',
-    'r3t':'text/vnd.rn-realtext3d',
-    'ram':'audio/x-pn-realaudio',
-    'rat':'application/rat-file',
-    'rec':'application/vnd.rn-recording',
-    'rgb':'application/x-rgb',
-    'rjt':'application/vnd.rn-realsystem-rjt',
-    'rle':'application/x-rle',
-    'rmf':'application/vnd.adobe.rmf',
-    'rmj':'application/vnd.rn-realsystem-rmj',
-    'rmp':'application/vnd.rn-rn_music_package',
-    'rmvb':'application/vnd.rn-realmedia-vbr',
-    'rnx':'application/vnd.rn-realplayer',
-    'rpm':'audio/x-pn-realaudio-plugin',
-    'rt':'text/vnd.rn-realtext',
-    'rtf':'application/x-rtf',
-    'sam':'application/x-sam',
-    'sdp':'application/sdp',
-    'sit':'application/x-stuffit',
-    'sld':'application/x-sld',
-    'smi':'application/smil',
-    'smk':'application/x-smk',
-    'sol':'text/plain',
-    'spc':'application/x-pkcs7-certificates',
-    'spp':'text/xml',
-    'sst':'application/vnd.ms-pki.certstore',
-    'stm':'text/html',
-    'svg':'text/xml',
-    'tdf':'application/x-tdf',
-    'tga':'application/x-tga',
-    'tif':'application/x-tif',
-    'tld':'text/xml',
-    'torrent':'application/x-bittorrent',
-    'txt':'text/plain',
-    'uls':'text/iuls',
-    'vda':'application/x-vda',
-    'vml':'text/xml',
-    'vsd':'application/vnd.visio',
-    'vss':'application/vnd.visio',
-    'vst':'application/x-vst',
-    'vsx':'application/vnd.visio',
-    'vxml':'text/xml',
-    'wax':'audio/x-ms-wax',
-    'wb2':'application/x-wb2',
-    'wbmp':'image/vnd.wap.wbmp',
-    'wk3':'application/x-wk3',
-    'wkq':'application/x-wkq',
-    'wm':'video/x-ms-wm',
-    'wmd':'application/x-ms-wmd',
-    'wml':'text/vnd.wap.wml',
-    'wmx':'video/x-ms-wmx',
-    'wp6':'application/x-wp6',
-    'wpg':'application/x-wpg',
-    'wq1':'application/x-wq1',
-    'wri':'application/x-wri',
-    'ws':'application/x-ws',
-    'wsc':'text/scriptlet',
-    'wvx':'video/x-ms-wvx',
-    'xdr':'text/xml',
-    'xfdf':'application/vnd.adobe.xfdf',
-    'xls':'application/vnd.ms-excel',
-    'xlw':'application/x-xlw',
-    'xpl':'audio/scpls',
-    'xql':'text/xml',
-    'xsd':'text/xml',
-    'xslt':'text/xml',
-    'x_b':'application/x-x_b',
-    'sisx':'application/vnd.symbian.install',
-    'ipa':'application/vnd.iphone',
-    'xap':'application/x-silverlight-app',
+        'acp': 'audio/x-mei-aac',
+        'aif': 'audio/aiff',
+        'aiff': 'audio/aiff',
+        'asa': 'text/asa',
+        'asp': 'text/asp',
+        'au': 'audio/basic',
+        'awf': 'application/vnd.adobe.workflow',
+        'bmp': 'application/x-bmp',
+        'c4t': 'application/x-c4t',
+        'cal': 'application/x-cals',
+        'cdf': 'application/x-netcdf',
+        'cel': 'application/x-cel',
+        'cg4': 'application/x-g4',
+        'cit': 'application/x-cit',
+        'cml': 'text/xml',
+        'cmx': 'application/x-cmx',
+        'crl': 'application/pkix-crl',
+        'csi': 'application/x-csi',
+        'cut': 'application/x-cut',
+        'dbm': 'application/x-dbm',
+        'dcd': 'text/xml',
+        'der': 'application/x-x509-ca-cert',
+        'dib': 'application/x-dib',
+        'doc': 'application/msword',
+        'drw': 'application/x-drw',
+        'dwg': 'application/x-dwg',
+        'dxf': 'application/x-dxf',
+        'emf': 'application/x-emf',
+        'ent': 'text/xml',
+        'etd': 'application/x-ebx',
+        'fax': 'image/fax',
+        'fif': 'application/fractals',
+        'frm': 'application/x-frm',
+        'gbr': 'application/x-gbr',
+        'gif': 'image/gif',
+        'gp4': 'application/x-gp4',
+        'hmr': 'application/x-hmr',
+        'hpl': 'application/x-hpl',
+        'hrf': 'application/x-hrf',
+        'htc': 'text/x-component',
+        'html': 'text/html',
+        'htx': 'text/html',
+        'iff': 'application/x-iff',
+        'igs': 'application/x-igs',
+        'img': 'application/x-img',
+        'isp': 'application/x-internet-signup',
+        'java': 'java/*',
+        'jpeg': 'image/jpeg',
+        'jsp': 'text/html',
+        'lar': 'application/x-laplayer-reg',
+        'lavs': 'audio/x-liquid-secure',
+        'lmsff': 'audio/x-la-lms',
+        'ltr': 'application/x-ltr',
+        'm2v': 'video/x-mpeg',
+        'm4e': 'video/mpeg4',
+        'man': 'application/x-troff-man',
+        'mfp': 'application/x-shockwave-flash',
+        'mhtml': 'message/rfc822',
+        'mid': 'audio/mid',
+        'mil': 'application/x-mil',
+        'mnd': 'audio/x-musicnet-download',
+        'mocha': 'application/x-javascript',
+        'mp1': 'audio/mp1',
+        'mp2v': 'video/mpeg',
+        'mp4': 'video/mpeg4',
+        'mpd': 'application/vnd.ms-project',
+        'mpeg': 'video/mpg',
+        'mpga': 'audio/rn-mpeg',
+        'mps': 'video/x-mpeg',
+        'mpv': 'video/mpg',
+        'mpw': 'application/vnd.ms-project',
+        'mtx': 'text/xml',
+        'net': 'image/pnetvue',
+        'nws': 'message/rfc822',
+        'out': 'application/x-out',
+        'p12': 'application/x-pkcs12',
+        'p7c': 'application/pkcs7-mime',
+        'p7r': 'application/x-pkcs7-certreqresp',
+        'pc5': 'application/x-pc5',
+        'pcl': 'application/x-pcl',
+        'pdx': 'application/vnd.adobe.pdx',
+        'pgl': 'application/x-pgl',
+        'pko': 'application/vnd.ms-pki.pko',
+        'plg': 'text/html',
+        'plt': 'application/x-plt',
+        'ppa': 'application/vnd.ms-powerpoint',
+        'pps': 'application/vnd.ms-powerpoint',
+        'prf': 'application/pics-rules',
+        'prt': 'application/x-prt',
+        'pwz': 'application/vnd.ms-powerpoint',
+        'ra': 'audio/vnd.rn-realaudio',
+        'ras': 'application/x-ras',
+        'rdf': 'text/xml',
+        'red': 'application/x-red',
+        'rjs': 'application/vnd.rn-realsystem-rjs',
+        'rlc': 'application/x-rlc',
+        'rm': 'application/vnd.rn-realmedia',
+        'rmi': 'audio/mid',
+        'rmm': 'audio/x-pn-realaudio',
+        'rms': 'application/vnd.rn-realmedia-secure',
+        'rmx': 'application/vnd.rn-realsystem-rmx',
+        'rp': 'image/vnd.rn-realpix',
+        'rsml': 'application/vnd.rn-rsml',
+        'rv': 'video/vnd.rn-realvideo',
+        'sat': 'application/x-sat',
+        'sdw': 'application/x-sdw',
+        'slb': 'application/x-slb',
+        'slk': 'drawing/x-slk',
+        'smil': 'application/smil',
+        'snd': 'audio/basic',
+        'sor': 'text/plain',
+        'spl': 'application/futuresplash',
+        'ssm': 'application/streamingmedia',
+        'stl': 'application/vnd.ms-pki.stl',
+        'sty': 'application/x-sty',
+        'swf': 'application/x-shockwave-flash',
+        'tg4': 'application/x-tg4',
+        'tiff': 'image/tiff',
+        'top': 'drawing/x-top',
+        'tsd': 'text/xml',
+        'uin': 'application/x-icq',
+        'vcf': 'text/x-vcard',
+        'vdx': 'application/vnd.visio',
+        'vpg': 'application/x-vpeg005',
+        'vsw': 'application/vnd.visio',
+        'vtx': 'application/vnd.visio',
+        'wav': 'audio/wav',
+        'wb1': 'application/x-wb1',
+        'wb3': 'application/x-wb3',
+        'wiz': 'application/msword',
+        'wk4': 'application/x-wk4',
+        'wks': 'application/x-wks',
+        'wma': 'audio/x-ms-wma',
+        'wmf': 'application/x-wmf',
+        'wmv': 'video/x-ms-wmv',
+        'wmz': 'application/x-ms-wmz',
+        'wpd': 'application/x-wpd',
+        'wpl': 'application/vnd.ms-wpl',
+        'wr1': 'application/x-wr1',
+        'wrk': 'application/x-wrk',
+        'ws2': 'application/x-ws',
+        'wsdl': 'text/xml',
+        'xdp': 'application/vnd.adobe.xdp',
+        'xfd': 'application/vnd.adobe.xfd',
+        'xhtml': 'text/html',
+        'xml': 'text/xml',
+        'xq': 'text/xml',
+        'xquery': 'text/xml',
+        'xsl': 'text/xml',
+        'xwd': 'application/x-xwd',
+        'sis': 'application/vnd.symbian.install',
+        'x_t': 'application/x-x_t',
+        'apk': 'application/vnd.android.package-archive',
+        '0.301': 'application/x-301',
+        '0.906': 'application/x-906',
+        'a11': 'application/x-a11',
+        'ai': 'application/postscript',
+        'aifc': 'audio/aiff',
+        'anv': 'application/x-anv',
+        'asf': 'video/x-ms-asf',
+        'asx': 'video/x-ms-asf',
+        'avi': 'video/avi',
+        'biz': 'text/xml',
+        'bot': 'application/x-bot',
+        'c90': 'application/x-c90',
+        'cat': 'application/vnd.ms-pki.seccat',
+        'cdr': 'application/x-cdr',
+        'cer': 'application/x-x509-ca-cert',
+        'cgm': 'application/x-cgm',
+        'class': 'java/*',
+        'cmp': 'application/x-cmp',
+        'cot': 'application/x-cot',
+        'crt': 'application/x-x509-ca-cert',
+        'css': 'text/css',
+        'dbf': 'application/x-dbf',
+        'dbx': 'application/x-dbx',
+        'dcx': 'application/x-dcx',
+        'dgn': 'application/x-dgn',
+        'dll': 'application/x-msdownload',
+        'dot': 'application/msword',
+        'dtd': 'text/xml',
+        'dwf': 'application/x-dwf',
+        'dxb': 'application/x-dxb',
+        'edn': 'application/vnd.adobe.edn',
+        'eml': 'message/rfc822',
+        'epi': 'application/x-epi',
+        'eps': 'application/postscript',
+        'exe': 'application/x-msdownload',
+        'fdf': 'application/vnd.fdf',
+        'fo': 'text/xml',
+        'g4': 'application/x-g4',
+        '': 'application/x-',
+        'gl2': 'application/x-gl2',
+        'hgl': 'application/x-hgl',
+        'hpg': 'application/x-hpgl',
+        'hqx': 'application/mac-binhex40',
+        'hta': 'application/hta',
+        'htm': 'text/html',
+        'htt': 'text/webviewhtml',
+        'icb': 'application/x-icb',
+        'ico': 'application/x-ico',
+        'ig4': 'application/x-g4',
+        'iii': 'application/x-iphone',
+        'ins': 'application/x-internet-signup',
+        'IVF': 'video/x-ivf',
+        'jfif': 'image/jpeg',
+        'jpe': 'application/x-jpe',
+        'jpg': 'image/jpeg',
+        'js': 'application/x-javascript',
+        'la1': 'audio/x-liquid-file',
+        'latex': 'application/x-latex',
+        'lbm': 'application/x-lbm',
+        'ls': 'application/x-javascript',
+        'm1v': 'video/x-mpeg',
+        'm3u': 'audio/mpegurl',
+        'mac': 'application/x-mac',
+        'math': 'text/xml',
+        'mdb': 'application/x-mdb',
+        'mht': 'message/rfc822',
+        'mi': 'application/x-mi',
+        'midi': 'audio/mid',
+        'mml': 'text/xml',
+        'mns': 'audio/x-musicnet-stream',
+        'movie': 'video/x-sgi-movie',
+        'mp2': 'audio/mp2',
+        'mp3': 'audio/mp3',
+        'mpa': 'video/x-mpg',
+        'mpe': 'video/x-mpeg',
+        'mpg': 'video/mpg',
+        'mpp': 'application/vnd.ms-project',
+        'mpt': 'application/vnd.ms-project',
+        'mpv2': 'video/mpeg',
+        'mpx': 'application/vnd.ms-project',
+        'mxp': 'application/x-mmxp',
+        'nrf': 'application/x-nrf',
+        'odc': 'text/x-ms-odc',
+        'p10': 'application/pkcs10',
+        'p7b': 'application/x-pkcs7-certificates',
+        'p7m': 'application/pkcs7-mime',
+        'p7s': 'application/pkcs7-signature',
+        'pci': 'application/x-pci',
+        'pcx': 'application/x-pcx',
+        'pdf': 'application/pdf',
+        'pfx': 'application/x-pkcs12',
+        'pic': 'application/x-pic',
+        'pl': 'application/x-perl',
+        'pls': 'audio/scpls',
+        'png': 'image/png',
+        'pot': 'application/vnd.ms-powerpoint',
+        'ppm': 'application/x-ppm',
+        'ppt': 'application/vnd.ms-powerpoint',
+        'pr': 'application/x-pr',
+        'prn': 'application/x-prn',
+        'ps': 'application/x-ps',
+        'ptn': 'application/x-ptn',
+        'r3t': 'text/vnd.rn-realtext3d',
+        'ram': 'audio/x-pn-realaudio',
+        'rat': 'application/rat-file',
+        'rec': 'application/vnd.rn-recording',
+        'rgb': 'application/x-rgb',
+        'rjt': 'application/vnd.rn-realsystem-rjt',
+        'rle': 'application/x-rle',
+        'rmf': 'application/vnd.adobe.rmf',
+        'rmj': 'application/vnd.rn-realsystem-rmj',
+        'rmp': 'application/vnd.rn-rn_music_package',
+        'rmvb': 'application/vnd.rn-realmedia-vbr',
+        'rnx': 'application/vnd.rn-realplayer',
+        'rpm': 'audio/x-pn-realaudio-plugin',
+        'rt': 'text/vnd.rn-realtext',
+        'rtf': 'application/x-rtf',
+        'sam': 'application/x-sam',
+        'sdp': 'application/sdp',
+        'sit': 'application/x-stuffit',
+        'sld': 'application/x-sld',
+        'smi': 'application/smil',
+        'smk': 'application/x-smk',
+        'sol': 'text/plain',
+        'spc': 'application/x-pkcs7-certificates',
+        'spp': 'text/xml',
+        'sst': 'application/vnd.ms-pki.certstore',
+        'stm': 'text/html',
+        'svg': 'text/xml',
+        'tdf': 'application/x-tdf',
+        'tga': 'application/x-tga',
+        'tif': 'application/x-tif',
+        'tld': 'text/xml',
+        'torrent': 'application/x-bittorrent',
+        'txt': 'text/plain',
+        'uls': 'text/iuls',
+        'vda': 'application/x-vda',
+        'vml': 'text/xml',
+        'vsd': 'application/vnd.visio',
+        'vss': 'application/vnd.visio',
+        'vst': 'application/x-vst',
+        'vsx': 'application/vnd.visio',
+        'vxml': 'text/xml',
+        'wax': 'audio/x-ms-wax',
+        'wb2': 'application/x-wb2',
+        'wbmp': 'image/vnd.wap.wbmp',
+        'wk3': 'application/x-wk3',
+        'wkq': 'application/x-wkq',
+        'wm': 'video/x-ms-wm',
+        'wmd': 'application/x-ms-wmd',
+        'wml': 'text/vnd.wap.wml',
+        'wmx': 'video/x-ms-wmx',
+        'wp6': 'application/x-wp6',
+        'wpg': 'application/x-wpg',
+        'wq1': 'application/x-wq1',
+        'wri': 'application/x-wri',
+        'ws': 'application/x-ws',
+        'wsc': 'text/scriptlet',
+        'wvx': 'video/x-ms-wvx',
+        'xdr': 'text/xml',
+        'xfdf': 'application/vnd.adobe.xfdf',
+        'xls': 'application/vnd.ms-excel',
+        'xlw': 'application/x-xlw',
+        'xpl': 'audio/scpls',
+        'xql': 'text/xml',
+        'xsd': 'text/xml',
+        'xslt': 'text/xml',
+        'x_b': 'application/x-x_b',
+        'sisx': 'application/vnd.symbian.install',
+        'ipa': 'application/vnd.iphone',
+        'xap': 'application/x-silverlight-app',
     }
 
     def __init__(self, host, port=25):
+
+        self.debug = False
         self._host = host
         self._port = port
         self._debuglevel = 0
         self._auth_user = None
         self._user_pass = None
         self._mail_from = ''
         self._mail_to = ''
@@ -437,15 +422,14 @@
         self._is_html = True
         self._time_out = 20
         self._helo = "QuickEmail"
         self._content_from = None
         self._content_to = None
         self._content_cc = None
         self._msg = None
-        
 
     def set_helo(self, h):
         self._helo = h
 
     def set_host(self, h):
         self._host = h
 
@@ -453,35 +437,35 @@
         self._port = p
 
     def set_auth_user(self, s):
         self._auth_user = s
 
     def set_user_pass(self, s):
         self._user_pass = s
-    
+
     def set_mail_from(self, s):
-        self._mail_from = s if s != None else ''
-    
+        self._mail_from = s if s is not None else ''
+
     def set_mail_to(self, s):
-        self._mail_to = s if s != None else ''
-    
+        self._mail_to = s if s is not None else ''
+
     def set_mail_cc(self, s):
-        self._mail_cc = s if s != None else ''
+        self._mail_cc = s if s is not None else ''
 
     def set_mail_bcc(self, s):
-        self._mail_bcc = s if s != None else ''
-        
+        self._mail_bcc = s if s is not None else ''
+
     def set_content_from(self, s):
-        self._content_from = s if s != None else ''
-    
+        self._content_from = s if s is not None else ''
+
     def set_content_to(self, s):
-        self._content_to = s if s != None else ''
+        self._content_to = s if s is not None else ''
 
     def set_content_cc(self, s):
-        self._content_cc = s if s != None else ''
+        self._content_cc = s if s is not None else ''
 
     def set_mail_subject(self, s):
         self._mail_subject = s
 
     def set_mail_content(self, s):
         self._mail_content = s
 
@@ -489,358 +473,378 @@
         self._mail_attach = filelist
 
     def set_is_html(self, b):
         self._is_html = b
 
     def set_time_out(self, t):
         self._time_out = t
-        
+
     @property
     def helo(self):
         return self._helo
+
     @helo.setter
     def helo(self, h):
         self._helo = h
 
     @property
     def host(self):
         return self._host
+
     @host.setter
     def host(self, h):
         self._host = h
 
     @property
     def port(self):
         return self._port
+
     @port.setter
     def port(self, p):
         self._port = p
 
     @property
     def auth_user(self):
         return self._auth_user
+
     @auth_user.setter
     def auth_user(self, s):
         self._auth_user = s
 
     @property
     def user_pass(self):
         return self._user_pass
+
     @user_pass.setter
     def user_pass(self, s):
         self._user_pass = s
 
     @property
     def mail_from(self):
         return self._mail_from
+
     @mail_from.setter
     def mail_from(self, s):
-        self._mail_from = s if s != None else ''
+        self._mail_from = s if s is not None else ''
 
     @property
     def mail_to(self):
         return self._mail_to
+
     @mail_to.setter
     def mail_to(self, s):
-        self._mail_to = s if s != None else ''
+        self._mail_to = s if s is not None else ''
 
     @property
     def mail_cc(self):
         return self._mail_cc
+
     @mail_cc.setter
     def mail_cc(self, s):
-        self._mail_cc = s if s != None else ''
+        self._mail_cc = s if s is not None else ''
 
     @property
     def mail_bcc(self):
         return self._mail_bcc
+
     @mail_bcc.setter
     def mail_bcc(self, s):
-        self._mail_bcc = s if s != None else ''
+        self._mail_bcc = s if s is not None else ''
 
     @property
     def content_from(self):
         return self._content_from
+
     @content_from.setter
     def content_from(self, s):
-        self._content_from = s if s != None else ''
+        self._content_from = s if s is not None else ''
 
     @property
     def content_to(self):
         return self._content_to
+
     @content_to.setter
     def content_to(self, s):
-        self._content_to = s if s != None else ''
+        self._content_to = s if s is not None else ''
 
     @property
     def content_cc(self):
         return self._content_cc
+
     @content_cc.setter
     def content_cc(self, s):
-        self._content_cc = s if s != None else ''
+        self._content_cc = s if s is not None else ''
 
     @property
     def mail_subject(self):
         return self._mail_subject
+
     @mail_subject.setter
     def mail_subject(self, s):
         self._mail_subject = s
 
     @property
     def mail_content(self):
         return self._mail_content
+
     @mail_content.setter
     def mail_content(self, s):
         self._mail_content = s
 
     @property
     def mail_attach(self):
         return self._mail_attach
+
     @mail_attach.setter
     def mail_attach(self, filelist):
         self._mail_attach = filelist
-    
+
     @property
     def is_html(self):
         return self._is_html
+
     @is_html.setter
     def is_html(self, b):
         self._is_html = b
-        
+
     @property
     def time_out(self):
         return self._time_out
+
     @time_out.setter
     def time_out(self, t):
         self._time_out = t
-        
+
     def _get_fromdomain(self):
         if '@' in self._mail_from:
             return self._mail_from.strip('>').split('@')[1]
         return 'QuickEmail.local'
 
-    def _format_addr(self, s):
+    @staticmethod
+    def _format_addr(s):
         # input RCPT TO string '一二三<123@test.com>'
 
         name, addr = parseaddr(s)
-        return formataddr(( \
-            Header(name, 'utf-8').encode(), addr))
+        return formataddr((Header(name, 'utf-8').encode(), addr))
 
-    def _mailto_rebuild(self, toaddr):
+    @staticmethod
+    def _mailto_rebuild(toaddr):
         # input RCPT TO 
         # string    # '一二三<123@test.com>,中语言C<abc@test.com>,AA高丽A<a@test.com>' 
         # output format encode mail object
 
         msg_to = []
 
         for s in toaddr.split(","):
             name, addr = parseaddr(s)
-            if name.strip(' ') == '' or name == None:
+            if name.strip(' ') == '' or name is None:
                 msg_to.append('<' + addr + '>')
             else:
-                msg_to.append((
-                    '"=?utf-8?B?' + base64.b64encode(name.encode("utf-8")).decode("utf-8") + '?="') + ' <' + addr + '>')
+                msg_to.append(('"=?utf-8?B?' + base64.b64encode(name.encode("utf-8")).decode(
+                                  "utf-8") + '?="') + ' <' + addr + '>')
 
         return ','.join(msg_to)
 
     def creatmsg(self):
         # 邮件信体处理
-        
-        if self._is_html == True:
+
+        if self._is_html:
             html_plain = 'html'
         else:
             html_plain = 'plain'
-        
-        if self._mail_attach != None:
+
+        if self._mail_attach is not None:
             msg = MIMEMultipart('mixed')
         else:
             msg = MIMEMultipart('alternative')
-            
+
         msg['X-Client'] = "QuickEmail"
         msg['Subject'] = self.mail_subject
-        
-        if self.content_from == None:
+
+        if self.content_from is None:
             msg['From'] = self._mailto_rebuild(self.mail_from)
         else:
             msg['From'] = self._mailto_rebuild(self.content_from)
 
-        if self.content_to == None:
+        if self.content_to is None:
             msg['To'] = self._mailto_rebuild(self.mail_to)
         else:
             msg['To'] = self._mailto_rebuild(self.content_to)
-        
-        
-        if self.mail_cc != None or self.content_cc != None:
-            if self.content_cc == None:
-                msg['CC'] = self.mailto_rebuild(self.mail_cc)
+
+        if self.mail_cc is not None or self.content_cc is not None:
+            if self.content_cc is None:
+                msg['CC'] = self._mailto_rebuild(self.mail_cc)
             else:
-                msg['CC'] = self.mailto_rebuild(self.content_cc)
-                
+                msg['CC'] = self._mailto_rebuild(self.content_cc)
+
         msg['Message-ID'] = '<QuickEmail.{}.{}@{}>'.format(time.time(), random.randint(1, 1000), self._get_fromdomain())
-        
+
         msg['Date'] = formatdate(localtime=True)
 
-        msg_html_content = MIMEText(self.mail_content,html_plain,_charset='utf-8')
+        msg_html_content = MIMEText(self.mail_content, html_plain, _charset='utf-8')
         msg.attach(msg_html_content)
 
-        if self.mail_attach != None:
+        if self.mail_attach is not None:
             for attach_file in self.mail_attach:
                 file_name = os.path.basename(attach_file)
                 file_type = file_name.split('.')[-1]
 
                 if os.path.isfile(attach_file):
 
                     fp = open(attach_file, 'rb')
 
                     contype = self._content_type.get(file_type)
-                    if contype == None:
+                    if contype is None:
                         maintype, subtype = "application", "octet-stream"
                     else:
                         maintype, subtype = contype.split('/', 1)
 
-                    att = MIMEBase(maintype, subtype, name= \
-                        "=?utf-8?B?" + base64.b64encode(file_name.encode("utf-8")).decode("utf-8") + "?=")
+                    att = MIMEBase(maintype, subtype, name="=?utf-8?B?" + base64.b64encode(file_name.encode("utf-8"))
+                                   .decode("utf-8") + "?=")
                     # 加上必要的头信息:
-                    att.add_header('Content-Disposition', 'attachment', filename= \
-                        "=?utf-8?B?" + base64.b64encode(file_name.encode("utf-8")).decode("utf-8") + "?=")
+                    att.add_header('Content-Disposition', 'attachment', filename="=?utf-8?B?" + base64.b64encode(
+                        file_name.encode("utf-8")).decode("utf-8") + "?=")
                     # att.add_header('Content-ID', '<0>')
                     # att.add_header('X-Attachment-Id', '0')
                     # 把附件的内容读进来:
                     att.set_payload(fp.read())
                     # 用Base64编码:
                     encoders.encode_base64(att)
                     # 添加到MIMEMultipart:
                     msg.attach(att)
                     fp.close()
-        self.msg = msg.as_string()
+        self._msg = msg.as_string()
         return msg.as_string()
 
     def send(self, msgdata=None):
         """
         # from must be a string
         # rcptto must be list
         """
         if msgdata is None:
             self.creatmsg()
             msgdata = self._msg
         smtpfrom = self.mail_from
 
-        if self.mail_cc != None and self._mail_cc != '':
+        if self.mail_cc is not None and self._mail_cc != '':
             smtpto = self.mail_to + "," + self.mail_cc
         else:
             smtpto = self.mail_to
 
-        if self.mail_bcc != None and self.mail_bcc != '':
+        if self.mail_bcc is not None and self.mail_bcc != '':
             smtpto = smtpto + "," + self.mail_bcc
 
-        if smtpto == None or smtpto == '':
+        if smtpto is None or smtpto == '':
             return """Must set_mail_to()"""
 
         if self.port == 465:
             return "Anonymous send must use port 25"
 
         send_err = ''
         try:
             smtphandle = smtplib.SMTP(host=self.host, port=self.port, timeout=self.time_out)
-            #smtphandle.connect(self.host, self.port)
+            # smtphandle.connect(self.host, self.port)
             smtphandle.set_debuglevel = self._debuglevel
             smtphandle.helo(self._helo)
-            smtphandle.sendmail(smtpfrom,smtpto.split(','),msgdata)
+            smtphandle.sendmail(smtpfrom, smtpto.split(','), msgdata)
             smtphandle.quit()
             smtphandle.close()
         except Exception as e:
             if hasattr(e, 'args'):
-                for i in  e.args:
+                for i in e.args:
                     if not i:
                         continue
                     if isinstance(i, int):
                         send_err += str(i) + ' '
                         continue
                     if isinstance(i, bytes):
                         send_err += i.decode('utf-8') + ' '
                         continue
                     send_err += str(i)
             else:
                 send_err = str(e)
         if send_err:
-            return send_err
+            if self.debug:
+                raise send_err
+            return False
         return True
-        
+
     def authsend(self, msgdata=None):
         """
         # from must be a string
         # rcptto must be list
         """
-        if self.auth_user == None or self.user_pass == None:
+        if self.auth_user is None or self.user_pass is None:
             return """Must set mailuser and password : 
                 auth_user('username')
                 user_pass('password')"""
         if msgdata is None:
             self.creatmsg()
             msgdata = self._msg
         smtpfrom = self.mail_from
 
-        if self.mail_cc != None and self.mail_cc != '':
+        if self.mail_cc is not None and self.mail_cc != '':
             smtpto = self.mail_to + "," + self.mail_cc
         else:
             smtpto = self._mail_to
 
-        if self.mail_bcc != None and self.mail_bcc != '':
+        if self.mail_bcc is not None and self.mail_bcc != '':
             smtpto = smtpto + "," + self.mail_bcc
 
-        if smtpto == None or smtpto == '':
+        if smtpto is None or smtpto == '':
             return """Must mail_to()"""
 
         send_err = ''
         try:
             if self.port == 465:
-                smtphandle = smtplib.SMTP_SSL(host=self.host, port=self.port, timeout=self.time_out)
+                smtp_handle = smtplib.SMTP_SSL(host=self.host, port=self.port, timeout=self.time_out)
             else:
-                smtphandle = smtplib.SMTP(host=self.host, port=self.port, timeout=self.time_out)
-            #smtphandle.connect(self.host, self.port)
-            smtphandle.set_debuglevel = self._debuglevel
-            smtphandle.ehlo(self._helo)
-            smtphandle.login(self.auth_user, self.user_pass)
-            smtphandle.sendmail(smtpfrom,smtpto.split(','),msgdata)
-            smtphandle.quit()
-            smtphandle.close()
+                smtp_handle = smtplib.SMTP(host=self.host, port=self.port, timeout=self.time_out)
+            # smtp_handle.connect(self.host, self.port)
+            smtp_handle.set_debuglevel = self._debuglevel
+            smtp_handle.ehlo(self._helo)
+            smtp_handle.login(self.auth_user, self.user_pass)
+            smtp_handle.sendmail(smtpfrom, smtpto.split(','), msgdata)
+            smtp_handle.quit()
+            smtp_handle.close()
         except Exception as e:
             if hasattr(e, 'args'):
-                for i in  e.args:
+                for i in e.args:
                     if not i:
                         continue
                     if isinstance(i, int):
                         send_err += str(i) + ' '
                         continue
                     if isinstance(i, bytes):
                         send_err += i.decode('utf-8') + ' '
                         continue
                     send_err += str(i)
             else:
                 send_err = str(e)
         if send_err:
-            return send_err
+            if self.debug:
+                raise send_err
+            return False
         return True
-    
+
+
 if __name__ == '__main__':
 
     quicksend = QuickEmail('127.0.0.1', 25)
     quicksend.auth_user = 'abc'
     quicksend.user_pass = 'test'
-    quicksend.mail_from = '<a@99.com>'
+    quicksend.mail_from = '<a@test.com>'
     quicksend.mail_to = '一二三 <123@test.com>,abc@test.com,<a@test.com>'
     quicksend.mail_bcc = '张三<b@test.com>'
     quicksend.mail_subject = 'mY subject还有中文!'
     quicksend.mail_content = '<font color=red>red content一段中文</font>'
     quicksend.mail_attach = ['C:\\Users\\Administrator\\Pictures\\163.com.png']
     quicksend.is_html = True
-    # quicksend.content_from = '假发件人<a@a.com>'
-    # quicksend.content_cc = '假抄送人<abc@a.com>'
+    quicksend.content_from = '假发件人<a@a.com>'
+    quicksend.content_cc = '假抄送人<abc@a.com>'
 
-    
-    msg = quicksend.creatmsg()
+    # msg = quicksend.creatmsg()
     # print(msg)
     print(quicksend.auth_user, quicksend.user_pass)
-    do_send = quicksend.authsend(msg)
-    if do_send != True:
+    do_send = quicksend.authsend()
+    if not do_send:
         print(do_send)
-
```

## Comparing `quickemail-0.2.4.dist-info/METADATA` & `quickemail-0.2.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickemail
-Version: 0.2.4
+Version: 0.2.5
 Summary: Quick send email use python3.
 Home-page: http://clayboy.cn
 Author: Clayboy
 Author-email: clayboy@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 
@@ -35,84 +35,84 @@
 ::
 
     from quickemail import QuickEmail
 
 1. 发信前先定义发信要素：
 
     - 指定主机和端口，必须参数：
-
+    
     ::
-
+    
         quicksend = QuickEmail('mail.test.com', 25)    # SMTP发信端口，默认是25 SSL链接使用465
 
     - 定义HELO主机名，参数可省略：
-
+    
     ::
-
+    
         quicksend.helo = 'QuickEmail'                 # HELO主机名不能使用有空格的字符串
 
     - 认证用户名和密码，authsend()必须的参数：
-
+    
     ::
-
+    
         quicksend.mail_user = 'a'                     # 认证用户名
         quicksend.user_pass = 'test'                  # 认证用户的密码
 
     - 发信人、收信人为必须参数：
-
+    
     ::
-
+    
         quicksend.mail_from = 'AA高丽A<a@test.com>'    # 发信人地址，格式为:   FullName<email address>
         quicksend.mail_to = '一二三<123@test.com>,ABC<abc@test.com>'    # 格式同上，多地址使用逗号","分隔
 
     - 抄送人，可省略：
-
+    
     ::
-
+    
         quicksend.mail_cc = '一二三<123@test.com>,中语言C<abc@test.com>,AA高丽A<a@test.com>'
 
     - 邮件主题、内容，支持使用HTML：
-
+    
     ::
-
+    
         quicksend.mail_subject = 'mY subject还有中文!'
         quicksend.mail_content = '<font color=red>red content一段中文</font>'
         quicksend.is_html = True
 
     - 添加附件，可省略：
-
+    
     ::
-
+    
         quicksend.mail_attach = ['abc.jpg']           # 添加附件 类型为list
-
+        
     - 高级定制，可省略：
-
+    
     ::
-
+    
         quicksend.content_from = '邮件显示的假发件人<from@test.com>'      # 定制邮件信体显示的发件人，一般为来隐藏实际的mail_from。
         quicksend.content_to = '邮件显示的假收件人<to@test.com>'      # 定制邮件信体显示的收件人，一般为来隐藏实际的mail_to。
         quicksend.content_cc = '邮件显示的假抄送人<cc@test.com>'      # 定制邮件信体显示的抄送人，一般为来隐藏实际的mail_cc。
 
 2. 使用creatmsg()建立邮件信体内容。(可以忽略)
 
     ::
-
+    
         msg = quicksend.creatmsg()
 
 3. 使用authsend()或者send()发送邮件。，参数msg可忽略。
 
     ::
-
+    
         quicksend.authsend(msg)     # 认证发信
         quicksend.send(msg)     # 不认证发信
 
 4. 错误显示(成功返回True，失败返回错误说明字符串)
 
     ::
-
+    
         result = quicksend.authsend(msg)
         if result != True:
             print(result)
 
         result = quicksend.send(msg)
         if result != True:
             print(result)
```

