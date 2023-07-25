# Comparing `tmp/hwi-2.2.1.tar.gz` & `tmp/hwi-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwi-2.2.1.tar", max compression
+gzip compressed data, was "hwi-2.3.0.tar", max compression
```

## Comparing `hwi-2.2.1.tar` & `hwi-2.3.0.tar`

### file list

```diff
@@ -1,123 +1,800 @@
--rw-r--r--   0        0        0     1068 2019-01-01 00:00:00.000000 hwi-2.2.1/LICENSE
--rw-r--r--   0        0        0     3409 2019-01-01 00:00:00.000000 hwi-2.2.1/README.md
--rwxr-xr-x   0        0        0      175 2019-01-01 00:00:00.000000 hwi-2.2.1/hwi-qt.py
--rwxr-xr-x   0        0        0      210 2019-01-01 00:00:00.000000 hwi-2.2.1/hwi.py
--rw-r--r--   0        0        0       22 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/__init__.py
--rw-r--r--   0        0        0     3934 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/_base58.py
--rw-r--r--   0        0        0     5720 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/_bech32.py
--rw-r--r--   0        0        0    16112 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/_cli.py
--rw-r--r--   0        0        0    19956 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/_gui.py
--rw-r--r--   0        0        0     4193 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/_script.py
--rw-r--r--   0        0        0     6526 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/_serialize.py
--rw-r--r--   0        0        0    23812 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/commands.py
--rw-r--r--   0        0        0     2232 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/common.py
--rw-r--r--   0        0        0    22494 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/descriptor.py
--rw-r--r--   0        0        0      121 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/__init__.py
--rw-r--r--   0        0        0    34897 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/bitbox02.py
--rw-r--r--   0        0        0      384 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ckcc/README.md
--rw-r--r--   0        0        0       74 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ckcc/__init__.py
--rw-r--r--   0        0        0    13669 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ckcc/client.py
--rw-r--r--   0        0        0     2997 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ckcc/constants.py
--rw-r--r--   0        0        0     9877 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ckcc/protocol.py
--rw-r--r--   0        0        0     1807 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ckcc/sigheader.py
--rw-r--r--   0        0        0     3470 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ckcc/utils.py
--rw-r--r--   0        0        0    14527 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/coldcard.py
--rw-r--r--   0        0        0    27321 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/digitalbitbox.py
--rw-r--r--   0        0        0    25700 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/jade.py
--rw-r--r--   0        0        0      320 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/jadepy/README.md
--rw-r--r--   0        0        0       83 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/jadepy/__init__.py
--rw-r--r--   0        0        0    65564 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/jadepy/jade.py
--rw-r--r--   0        0        0      655 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/jadepy/jade_error.py
--rw-r--r--   0        0        0     1719 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/jadepy/jade_serial.py
--rw-r--r--   0        0        0     1701 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/jadepy/jade_tcp.py
--rw-r--r--   0        0        0     9295 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/keepkey.py
--rw-r--r--   0        0        0    23039 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger.py
--rw-r--r--   0        0        0     1265 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/README.md
--rw-r--r--   0        0        0      327 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/__init__.py
--rw-r--r--   0        0        0      488 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/README.md
--rw-r--r--   0        0        0      855 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/__init__.py
--rw-r--r--   0        0        0     4874 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/bitcoinTransaction.py
--rw-r--r--   0        0        0     2025 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/bitcoinVarint.py
--rw-r--r--   0        0        0    16449 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/btchip.py
--rw-r--r--   0        0        0     1020 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/btchipException.py
--rw-r--r--   0        0        0     2713 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/btchipHelpers.py
--rw-r--r--   0        0        0     3416 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/btchipUtils.py
--rw-r--r--   0        0        0     3224 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/ledgerWrapper.py
--rw-r--r--   0        0        0    11666 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/client.py
--rw-r--r--   0        0        0     8168 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/client_base.py
--rw-r--r--   0        0        0    12284 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/client_command.py
--rw-r--r--   0        0        0    13915 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/client_legacy.py
--rw-r--r--   0        0        0     6437 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/command_builder.py
--rw-r--r--   0        0        0     8188 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/errors.py
--rw-r--r--   0        0        0      806 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/exception/__init__.py
--rw-r--r--   0        0        0     1251 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/exception/device_exception.py
--rw-r--r--   0        0        0      652 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/exception/errors.py
--rw-r--r--   0        0        0      576 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/README.md
--rw-r--r--   0        0        0      107 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/__init__.py
--rw-r--r--   0        0        0       36 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__init__.py
--rw-r--r--   0        0        0      922 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/comm.py
--rw-r--r--   0        0        0     5086 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/hid_device.py
--rw-r--r--   0        0        0     2997 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/tcp_client.py
--rw-r--r--   0        0        0       84 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/log.py
--rw-r--r--   0        0        0     7019 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/transport.py
--rw-r--r--   0        0        0     8430 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/merkle.py
--rw-r--r--   0        0        0     4547 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/ledger_bitcoin/wallet.py
--rw-r--r--   0        0        0    36772 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezor.py
--rw-r--r--   0        0        0      628 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/README.md
--rw-r--r--   0        0        0      704 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/__init__.py
--rw-r--r--   0        0        0    13203 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/btc.py
--rw-r--r--   0        0        0    18854 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/client.py
--rw-r--r--   0        0        0    25872 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/debuglink.py
--rw-r--r--   0        0        0     7081 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/device.py
--rw-r--r--   0        0        0     1601 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/exceptions.py
--rw-r--r--   0        0        0    16038 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/firmware.py
--rw-r--r--   0        0        0     2260 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/log.py
--rw-r--r--   0        0        0     3499 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/mapping.py
--rw-r--r--   0        0        0    72766 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/messages.py
--rw-r--r--   0        0        0      935 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/models.py
--rw-r--r--   0        0        0    20415 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/protobuf.py
--rw-r--r--   0        0        0    10087 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/tools.py
--rw-r--r--   0        0        0     4913 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/transport/__init__.py
--rw-r--r--   0        0        0     5374 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/transport/hid.py
--rw-r--r--   0        0        0     5372 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/transport/protocol.py
--rw-r--r--   0        0        0     4881 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/transport/udp.py
--rw-r--r--   0        0        0     5315 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/devices/trezorlib/transport/webusb.py
--rw-r--r--   0        0        0     7048 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/errors.py
--rw-r--r--   0        0        0     9167 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/hwwclient.py
--rw-r--r--   0        0        0    14015 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/key.py
--rw-r--r--   0        0        0    46452 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/psbt.py
--rw-r--r--   0        0        0        0 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/py.typed
--rw-r--r--   0        0        0     9191 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/tx.py
--rw-r--r--   0        0        0     1756 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/20-hw1.rules
--rw-r--r--   0        0        0      310 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/51-coinkite.rules
--rw-r--r--   0        0        0      119 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/51-hid-digitalbitbox.rules
--rw-r--r--   0        0        0      980 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/51-trezor.rules
--rw-r--r--   0        0        0      769 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/51-usb-keepkey.rules
--rw-r--r--   0        0        0      142 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/52-hid-digitalbitbox.rules
--rw-r--r--   0        0        0      125 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/53-hid-bitbox02.rules
--rw-r--r--   0        0        0      147 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/54-hid-bitbox02.rules
--rw-r--r--   0        0        0      340 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/55-usb-jade.rules
--rw-r--r--   0        0        0     1158 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udev/README.md
--rw-r--r--   0        0        0     3416 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/udevinstaller.py
--rw-r--r--   0        0        0     2687 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/bitbox02pairing.ui
--rw-r--r--   0        0        0     5382 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/displayaddressdialog.ui
--rw-r--r--   0        0        0     6167 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/getkeypooloptionsdialog.ui
--rw-r--r--   0        0        0     2872 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/getxpubdialog.ui
--rw-r--r--   0        0        0      196 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/hwiqt.pyproject
--rw-r--r--   0        0        0     7628 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/mainwindow.ui
--rw-r--r--   0        0        0     4431 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/sendpindialog.ui
--rw-r--r--   0        0        0     2117 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/setpassphrasedialog.ui
--rw-r--r--   0        0        0     4378 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/signmessagedialog.ui
--rw-r--r--   0        0        0     5516 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/signpsbtdialog.ui
--rw-r--r--   0        0        0     2545 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_bitbox02pairing.py
--rw-r--r--   0        0        0     5435 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_displayaddressdialog.py
--rw-r--r--   0        0        0     5724 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_getkeypooloptionsdialog.py
--rw-r--r--   0        0        0     3151 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_getxpubdialog.py
--rw-r--r--   0        0        0     8994 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_mainwindow.py
--rw-r--r--   0        0        0     4729 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_sendpindialog.py
--rw-r--r--   0        0        0     2057 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_setpassphrasedialog.py
--rw-r--r--   0        0        0     4017 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_signmessagedialog.py
--rw-r--r--   0        0        0     4679 2019-01-01 00:00:00.000000 hwi-2.2.1/hwilib/ui/ui_signpsbtdialog.py
--rw-r--r--   0        0        0     1193 2019-01-01 00:00:00.000000 hwi-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     5126 1970-01-01 00:00:00.000000 hwi-2.2.1/setup.py
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 hwi-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2019-01-01 00:00:00.000000 hwi-2.3.0/LICENSE
+-rw-r--r--   0        0        0     3409 2019-01-01 00:00:00.000000 hwi-2.3.0/README.md
+-rwxr-xr-x   0        0        0      175 2019-01-01 00:00:00.000000 hwi-2.3.0/hwi-qt.py
+-rwxr-xr-x   0        0        0      210 2019-01-01 00:00:00.000000 hwi-2.3.0/hwi.py
+-rw-r--r--   0        0        0       22 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/__init__.py
+-rw-r--r--   0        0        0     4438 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/_base58.py
+-rw-r--r--   0        0        0     5720 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/_bech32.py
+-rw-r--r--   0        0        0    16112 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/_cli.py
+-rw-r--r--   0        0        0    22326 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/_gui.py
+-rw-r--r--   0        0        0     4193 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/_script.py
+-rw-r--r--   0        0        0     6526 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/_serialize.py
+-rw-r--r--   0        0        0    23812 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/commands.py
+-rw-r--r--   0        0        0     2242 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/common.py
+-rw-r--r--   0        0        0    22494 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/descriptor.py
+-rw-r--r--   0        0        0      121 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__init__.py
+-rw-r--r--   0        0        0      258 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      241 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      235 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      251 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      229 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    43230 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/bitbox02.cpython-311.pyc
+-rw-r--r--   0        0        0    22802 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/bitbox02.cpython-36.pyc
+-rw-r--r--   0        0        0    22805 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/bitbox02.cpython-37.pyc
+-rw-r--r--   0        0        0    23049 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/bitbox02.cpython-38.pyc
+-rw-r--r--   0        0        0    24165 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/bitbox02.cpython-39.pyc
+-rw-r--r--   0        0        0    22562 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/coldcard.cpython-311.pyc
+-rw-r--r--   0        0        0    11842 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/coldcard.cpython-36.pyc
+-rw-r--r--   0        0        0    11842 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/coldcard.cpython-37.pyc
+-rw-r--r--   0        0        0    11640 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/coldcard.cpython-38.pyc
+-rw-r--r--   0        0        0    12083 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/coldcard.cpython-39.pyc
+-rw-r--r--   0        0        0    38978 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/digitalbitbox.cpython-311.pyc
+-rw-r--r--   0        0        0    20835 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/digitalbitbox.cpython-36.pyc
+-rw-r--r--   0        0        0    20834 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/digitalbitbox.cpython-37.pyc
+-rw-r--r--   0        0        0    20426 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/digitalbitbox.cpython-38.pyc
+-rw-r--r--   0        0        0    20679 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/digitalbitbox.cpython-39.pyc
+-rw-r--r--   0        0        0    29134 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/jade.cpython-311.pyc
+-rw-r--r--   0        0        0    15591 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/jade.cpython-39.pyc
+-rw-r--r--   0        0        0    12729 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/keepkey.cpython-311.pyc
+-rw-r--r--   0        0        0     6281 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/keepkey.cpython-36.pyc
+-rw-r--r--   0        0        0     6269 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/keepkey.cpython-37.pyc
+-rw-r--r--   0        0        0     6355 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/keepkey.cpython-38.pyc
+-rw-r--r--   0        0        0     6725 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/keepkey.cpython-39.pyc
+-rw-r--r--   0        0        0    29850 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/ledger.cpython-311.pyc
+-rw-r--r--   0        0        0    12862 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/ledger.cpython-36.pyc
+-rw-r--r--   0        0        0    12801 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/ledger.cpython-37.pyc
+-rw-r--r--   0        0        0    12603 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/ledger.cpython-38.pyc
+-rw-r--r--   0        0        0    16524 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/ledger.cpython-39.pyc
+-rw-r--r--   0        0        0    46082 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/trezor.cpython-311.pyc
+-rw-r--r--   0        0        0    21149 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/trezor.cpython-36.pyc
+-rw-r--r--   0        0        0    21069 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/trezor.cpython-37.pyc
+-rw-r--r--   0        0        0    20857 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/trezor.cpython-38.pyc
+-rw-r--r--   0        0        0    23219 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/__pycache__/trezor.cpython-39.pyc
+-rw-r--r--   0        0        0    34922 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02.py
+-rw-r--r--   0        0        0    11432 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/LICENSE
+-rw-r--r--   0        0        0      613 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/README.md
+-rw-r--r--   0        0        0        0 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/__init__.py
+-rw-r--r--   0        0        0      160 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8254 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     1642 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/__init__.py
+-rw-r--r--   0        0        0     1176 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    28639 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-39.pyc
+-rw-r--r--   0        0        0     6631 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-39.pyc
+-rw-r--r--   0        0        0     1950 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-39.pyc
+-rw-r--r--   0        0        0    43441 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/bitbox02.py
+-rw-r--r--   0        0        0     7359 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/bootloader.py
+-rw-r--r--   0        0        0        0 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/py.typed
+-rw-r--r--   0        0        0     2371 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/bitbox02/secp256k1.py
+-rw-r--r--   0        0        0     1030 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/__init__.py
+-rw-r--r--   0        0        0      694 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    24452 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-39.pyc
+-rw-r--r--   0        0        0     2082 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-39.pyc
+-rw-r--r--   0        0        0     4760 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-39.pyc
+-rw-r--r--   0        0        0    27806 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/bitbox_api_protocol.py
+-rw-r--r--   0        0        0     1669 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/communication.py
+-rw-r--r--   0        0        0     4666 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/devices.py
+-rw-r--r--   0        0        0        0 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__init__.py
+-rw-r--r--   0        0        0      184 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1138 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1530 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1885 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     6642 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     4370 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1257 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     4317 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     4339 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1021 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1131 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1162 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1009 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1401 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.py
+-rw-r--r--   0        0        0     1638 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.pyi
+-rw-r--r--   0        0        0     2102 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.py
+-rw-r--r--   0        0        0     3851 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.pyi
+-rw-r--r--   0        0        0     2699 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.py
+-rw-r--r--   0        0        0     5248 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.pyi
+-rw-r--r--   0        0        0    10516 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.py
+-rw-r--r--   0        0        0    33375 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.pyi
+-rw-r--r--   0        0        0     6703 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.py
+-rw-r--r--   0        0        0    18628 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.pyi
+-rw-r--r--   0        0        0     1664 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.py
+-rw-r--r--   0        0        0     3152 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.pyi
+-rw-r--r--   0        0        0     6698 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.py
+-rw-r--r--   0        0        0    19589 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.pyi
+-rw-r--r--   0        0        0     5757 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.py
+-rw-r--r--   0        0        0    13514 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.pyi
+-rw-r--r--   0        0        0     1205 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.py
+-rw-r--r--   0        0        0     1308 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.pyi
+-rw-r--r--   0        0        0     1386 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.py
+-rw-r--r--   0        0        0     1541 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.pyi
+-rw-r--r--   0        0        0     1444 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.py
+-rw-r--r--   0        0        0     1990 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.pyi
+-rw-r--r--   0        0        0     1186 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.py
+-rw-r--r--   0        0        0     1394 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.pyi
+-rw-r--r--   0        0        0        0 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/py.typed
+-rw-r--r--   0        0        0      709 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__init__.py
+-rw-r--r--   0        0        0      365 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4462 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-39.pyc
+-rw-r--r--   0        0        0     5793 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/communication/u2fhid/u2fhid.py
+-rw-r--r--   0        0        0        0 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/py.typed
+-rw-r--r--   0        0        0     8035 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/bitbox02_lib/util.py
+-rw-r--r--   0        0        0     1012 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     1016 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1020 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1020 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5062 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/bitcoinTransaction.cpython-36.pyc
+-rw-r--r--   0        0        0     5064 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/bitcoinTransaction.cpython-37.pyc
+-rw-r--r--   0        0        0     5029 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/bitcoinTransaction.cpython-38.pyc
+-rw-r--r--   0        0        0     5029 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/bitcoinTransaction.cpython-39.pyc
+-rw-r--r--   0        0        0     2072 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/bitcoinVarint.cpython-36.pyc
+-rw-r--r--   0        0        0     2076 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/bitcoinVarint.cpython-37.pyc
+-rw-r--r--   0        0        0     2065 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/bitcoinVarint.cpython-38.pyc
+-rw-r--r--   0        0        0     2065 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/bitcoinVarint.cpython-39.pyc
+-rw-r--r--   0        0        0    12118 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchip.cpython-36.pyc
+-rw-r--r--   0        0        0    12112 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchip.cpython-37.pyc
+-rw-r--r--   0        0        0    12146 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchip.cpython-38.pyc
+-rw-r--r--   0        0        0    12191 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchip.cpython-39.pyc
+-rw-r--r--   0        0        0     5532 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipComm.cpython-36.pyc
+-rw-r--r--   0        0        0     5536 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipComm.cpython-37.pyc
+-rw-r--r--   0        0        0     5568 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipComm.cpython-38.pyc
+-rw-r--r--   0        0        0     5558 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipComm.cpython-39.pyc
+-rw-r--r--   0        0        0     1485 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipException.cpython-36.pyc
+-rw-r--r--   0        0        0     1489 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipException.cpython-37.pyc
+-rw-r--r--   0        0        0     1505 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipException.cpython-38.pyc
+-rw-r--r--   0        0        0     1505 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipException.cpython-39.pyc
+-rw-r--r--   0        0        0     2910 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipHelpers.cpython-36.pyc
+-rw-r--r--   0        0        0     2914 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipHelpers.cpython-37.pyc
+-rw-r--r--   0        0        0     2915 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipHelpers.cpython-38.pyc
+-rw-r--r--   0        0        0     2915 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipHelpers.cpython-39.pyc
+-rw-r--r--   0        0        0     3420 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipUtils.cpython-36.pyc
+-rw-r--r--   0        0        0     3419 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipUtils.cpython-37.pyc
+-rw-r--r--   0        0        0     3423 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipUtils.cpython-38.pyc
+-rw-r--r--   0        0        0     3436 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/btchipUtils.cpython-39.pyc
+-rw-r--r--   0        0        0     2557 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/ledgerWrapper.cpython-36.pyc
+-rw-r--r--   0        0        0     2561 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/ledgerWrapper.cpython-37.pyc
+-rw-r--r--   0        0        0     2559 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/ledgerWrapper.cpython-38.pyc
+-rw-r--r--   0        0        0     2559 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/btchip/__pycache__/ledgerWrapper.cpython-39.pyc
+-rw-r--r--   0        0        0      384 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/README.md
+-rw-r--r--   0        0        0       74 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__init__.py
+-rw-r--r--   0        0        0      249 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      215 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      219 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      223 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      223 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    16928 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     8951 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/client.cpython-36.pyc
+-rw-r--r--   0        0        0     8989 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/client.cpython-37.pyc
+-rw-r--r--   0        0        0     9006 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/client.cpython-38.pyc
+-rw-r--r--   0        0        0     8584 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/client.cpython-39.pyc
+-rw-r--r--   0        0        0     2626 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0     1553 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/constants.cpython-36.pyc
+-rw-r--r--   0        0        0     1537 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/constants.cpython-37.pyc
+-rw-r--r--   0        0        0     1543 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/constants.cpython-38.pyc
+-rw-r--r--   0        0        0     1541 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/constants.cpython-39.pyc
+-rw-r--r--   0        0        0    15195 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/protocol.cpython-311.pyc
+-rw-r--r--   0        0        0    10008 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/protocol.cpython-36.pyc
+-rw-r--r--   0        0        0     9978 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/protocol.cpython-37.pyc
+-rw-r--r--   0        0        0    10101 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/protocol.cpython-38.pyc
+-rw-r--r--   0        0        0    10045 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/protocol.cpython-39.pyc
+-rw-r--r--   0        0        0     4457 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     2512 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0        0        0     2491 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0        0        0     2503 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2475 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0    13206 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/client.py
+-rw-r--r--   0        0        0     2997 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/constants.py
+-rw-r--r--   0        0        0     9877 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/protocol.py
+-rw-r--r--   0        0        0     1807 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/sigheader.py
+-rw-r--r--   0        0        0     3470 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ckcc/utils.py
+-rw-r--r--   0        0        0    14527 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/coldcard.py
+-rw-r--r--   0        0        0    27321 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/digitalbitbox.py
+-rw-r--r--   0        0        0    25736 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jade.py
+-rw-r--r--   0        0        0      320 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/README.md
+-rw-r--r--   0        0        0       83 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__init__.py
+-rw-r--r--   0        0        0      309 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      260 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    72688 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/jade.cpython-311.pyc
+-rw-r--r--   0        0        0    57994 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/jade.cpython-39.pyc
+-rw-r--r--   0        0        0     1423 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/jade_error.cpython-311.pyc
+-rw-r--r--   0        0        0     1056 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/jade_error.cpython-39.pyc
+-rw-r--r--   0        0        0     2680 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-311.pyc
+-rw-r--r--   0        0        0     1528 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-39.pyc
+-rw-r--r--   0        0        0     3165 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-311.pyc
+-rw-r--r--   0        0        0     1762 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-39.pyc
+-rw-r--r--   0        0        0    65325 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/jade.py
+-rw-r--r--   0        0        0      655 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/jade_error.py
+-rw-r--r--   0        0        0     1719 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/jade_serial.py
+-rw-r--r--   0        0        0     1701 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/jadepy/jade_tcp.py
+-rw-r--r--   0        0        0     9295 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/keepkey.py
+-rw-r--r--   0        0        0    23039 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger.py
+-rw-r--r--   0        0        0     1265 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/README.md
+-rw-r--r--   0        0        0      327 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__init__.py
+-rw-r--r--   0        0        0      616 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      507 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    17245 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     9543 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-39.pyc
+-rw-r--r--   0        0        0    12613 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-311.pyc
+-rw-r--r--   0        0        0     9546 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-39.pyc
+-rw-r--r--   0        0        0    21274 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-311.pyc
+-rw-r--r--   0        0        0    13498 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-39.pyc
+-rw-r--r--   0        0        0    17594 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-311.pyc
+-rw-r--r--   0        0        0     8719 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-39.pyc
+-rw-r--r--   0        0        0    10967 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-311.pyc
+-rw-r--r--   0        0        0     6747 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-39.pyc
+-rw-r--r--   0        0        0    13767 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-311.pyc
+-rw-r--r--   0        0        0     8892 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-39.pyc
+-rw-r--r--   0        0        0     8621 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-311.pyc
+-rw-r--r--   0        0        0     5040 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-39.pyc
+-rw-r--r--   0        0        0      488 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/README.md
+-rw-r--r--   0        0        0      855 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__init__.py
+-rw-r--r--   0        0        0     1062 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1035 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9118 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-311.pyc
+-rw-r--r--   0        0        0     5044 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-39.pyc
+-rw-r--r--   0        0        0     3159 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-311.pyc
+-rw-r--r--   0        0        0     2080 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-39.pyc
+-rw-r--r--   0        0        0    25380 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-311.pyc
+-rw-r--r--   0        0        0    12184 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-39.pyc
+-rw-r--r--   0        0        0     1708 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-311.pyc
+-rw-r--r--   0        0        0     1520 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-39.pyc
+-rw-r--r--   0        0        0     5349 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-311.pyc
+-rw-r--r--   0        0        0     2930 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-39.pyc
+-rw-r--r--   0        0        0     6231 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-311.pyc
+-rw-r--r--   0        0        0     3451 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-39.pyc
+-rw-r--r--   0        0        0     4874 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/bitcoinTransaction.py
+-rw-r--r--   0        0        0     2025 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/bitcoinVarint.py
+-rw-r--r--   0        0        0    16449 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/btchip.py
+-rw-r--r--   0        0        0     1020 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/btchipException.py
+-rw-r--r--   0        0        0     2713 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/btchipHelpers.py
+-rw-r--r--   0        0        0     3416 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/btchipUtils.py
+-rw-r--r--   0        0        0     3224 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/ledgerWrapper.py
+-rw-r--r--   0        0        0    11666 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/client.py
+-rw-r--r--   0        0        0     8168 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/client_base.py
+-rw-r--r--   0        0        0    12284 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/client_command.py
+-rw-r--r--   0        0        0    13915 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/client_legacy.py
+-rw-r--r--   0        0        0     6437 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/command_builder.py
+-rw-r--r--   0        0        0     8188 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/errors.py
+-rw-r--r--   0        0        0      806 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/__init__.py
+-rw-r--r--   0        0        0      814 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      641 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1838 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-311.pyc
+-rw-r--r--   0        0        0     1305 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-39.pyc
+-rw-r--r--   0        0        0     2683 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     1959 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     1251 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/device_exception.py
+-rw-r--r--   0        0        0      652 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/errors.py
+-rw-r--r--   0        0        0      576 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/README.md
+-rw-r--r--   0        0        0      107 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/__init__.py
+-rw-r--r--   0        0        0      341 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      299 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      329 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/log.cpython-311.pyc
+-rw-r--r--   0        0        0      266 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     9498 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-311.pyc
+-rw-r--r--   0        0        0     6971 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-39.pyc
+-rw-r--r--   0        0        0       36 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__init__.py
+-rw-r--r--   0        0        0      245 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      225 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1869 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-311.pyc
+-rw-r--r--   0        0        0     1449 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-39.pyc
+-rw-r--r--   0        0        0     7897 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-311.pyc
+-rw-r--r--   0        0        0     4845 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-39.pyc
+-rw-r--r--   0        0        0     5058 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-311.pyc
+-rw-r--r--   0        0        0     3502 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-39.pyc
+-rw-r--r--   0        0        0      922 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/comm.py
+-rw-r--r--   0        0        0     5086 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/hid_device.py
+-rw-r--r--   0        0        0     2997 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/tcp_client.py
+-rw-r--r--   0        0        0       84 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/log.py
+-rw-r--r--   0        0        0     7019 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/transport.py
+-rw-r--r--   0        0        0     8430 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/merkle.py
+-rw-r--r--   0        0        0     4547 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/ledger_bitcoin/wallet.py
+-rw-r--r--   0        0        0    36772 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezor.py
+-rw-r--r--   0        0        0      628 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/README.md
+-rw-r--r--   0        0        0      704 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__init__.py
+-rw-r--r--   0        0        0      198 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      273 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      257 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      263 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      179 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    17114 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/btc.cpython-311.pyc
+-rw-r--r--   0        0        0     7038 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/btc.cpython-36.pyc
+-rw-r--r--   0        0        0     7054 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/btc.cpython-37.pyc
+-rw-r--r--   0        0        0     7171 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/btc.cpython-38.pyc
+-rw-r--r--   0        0        0     9425 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/btc.cpython-39.pyc
+-rw-r--r--   0        0        0    24117 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0    13324 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/client.cpython-36.pyc
+-rw-r--r--   0        0        0    13291 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/client.cpython-37.pyc
+-rw-r--r--   0        0        0    13439 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/client.cpython-38.pyc
+-rw-r--r--   0        0        0    15090 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/client.cpython-39.pyc
+-rw-r--r--   0        0        0    41481 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-311.pyc
+-rw-r--r--   0        0        0    22121 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-36.pyc
+-rw-r--r--   0        0        0    22115 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-37.pyc
+-rw-r--r--   0        0        0    22370 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-38.pyc
+-rw-r--r--   0        0        0    24671 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-39.pyc
+-rw-r--r--   0        0        0     9640 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/device.cpython-311.pyc
+-rw-r--r--   0        0        0     3979 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/device.cpython-36.pyc
+-rw-r--r--   0        0        0     3966 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/device.cpython-37.pyc
+-rw-r--r--   0        0        0     4018 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/device.cpython-38.pyc
+-rw-r--r--   0        0        0     5012 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/device.cpython-39.pyc
+-rw-r--r--   0        0        0     2652 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     1573 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-36.pyc
+-rw-r--r--   0        0        0     1577 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-37.pyc
+-rw-r--r--   0        0        0     1577 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-38.pyc
+-rw-r--r--   0        0        0     1707 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0        0        0     3420 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/log.cpython-311.pyc
+-rw-r--r--   0        0        0     1589 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/log.cpython-36.pyc
+-rw-r--r--   0        0        0     1619 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/log.cpython-37.pyc
+-rw-r--r--   0        0        0     1635 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/log.cpython-38.pyc
+-rw-r--r--   0        0        0     1924 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     4283 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/mapping.cpython-311.pyc
+-rw-r--r--   0        0        0     1799 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/mapping.cpython-36.pyc
+-rw-r--r--   0        0        0     1803 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/mapping.cpython-37.pyc
+-rw-r--r--   0        0        0     1841 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/mapping.cpython-38.pyc
+-rw-r--r--   0        0        0     2872 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/mapping.cpython-39.pyc
+-rw-r--r--   0        0        0    94388 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/messages.cpython-311.pyc
+-rw-r--r--   0        0        0    55088 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/messages.cpython-39.pyc
+-rw-r--r--   0        0        0     1735 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     1182 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0    30471 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-311.pyc
+-rw-r--r--   0        0        0    15475 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-36.pyc
+-rw-r--r--   0        0        0    15477 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-37.pyc
+-rw-r--r--   0        0        0    15513 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-38.pyc
+-rw-r--r--   0        0        0    16023 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-39.pyc
+-rw-r--r--   0        0        0    15555 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/tools.cpython-311.pyc
+-rw-r--r--   0        0        0     7634 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/tools.cpython-36.pyc
+-rw-r--r--   0        0        0     7603 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/tools.cpython-37.pyc
+-rw-r--r--   0        0        0     7658 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/tools.cpython-38.pyc
+-rw-r--r--   0        0        0     9175 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/__pycache__/tools.cpython-39.pyc
+-rw-r--r--   0        0        0    13203 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/btc.py
+-rw-r--r--   0        0        0    18854 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/client.py
+-rw-r--r--   0        0        0    25872 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/debuglink.py
+-rw-r--r--   0        0        0     7081 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/device.py
+-rw-r--r--   0        0        0     1601 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/exceptions.py
+-rw-r--r--   0        0        0    16038 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/firmware.py
+-rw-r--r--   0        0        0     2260 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/log.py
+-rw-r--r--   0        0        0     3499 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/mapping.py
+-rw-r--r--   0        0        0      908 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Address.cpython-36.pyc
+-rw-r--r--   0        0        0      912 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Address.cpython-37.pyc
+-rw-r--r--   0        0        0      934 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Address.cpython-38.pyc
+-rw-r--r--   0        0        0      930 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Address.cpython-39.pyc
+-rw-r--r--   0        0        0      375 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/AmountUnit.cpython-36.pyc
+-rw-r--r--   0        0        0      432 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/AmountUnit.cpython-37.pyc
+-rw-r--r--   0        0        0      436 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/AmountUnit.cpython-38.pyc
+-rw-r--r--   0        0        0      434 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/AmountUnit.cpython-39.pyc
+-rw-r--r--   0        0        0      914 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ApplyFlags.cpython-36.pyc
+-rw-r--r--   0        0        0      918 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ApplyFlags.cpython-37.pyc
+-rw-r--r--   0        0        0      942 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ApplyFlags.cpython-38.pyc
+-rw-r--r--   0        0        0      938 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ApplyFlags.cpython-39.pyc
+-rw-r--r--   0        0        0     1660 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ApplySettings.cpython-36.pyc
+-rw-r--r--   0        0        0     1644 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ApplySettings.cpython-37.pyc
+-rw-r--r--   0        0        0     1630 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ApplySettings.cpython-38.pyc
+-rw-r--r--   0        0        0     1628 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ApplySettings.cpython-39.pyc
+-rw-r--r--   0        0        0     1695 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/AuthorizeCoinJoin.cpython-36.pyc
+-rw-r--r--   0        0        0     1664 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/AuthorizeCoinJoin.cpython-37.pyc
+-rw-r--r--   0        0        0     1661 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/AuthorizeCoinJoin.cpython-38.pyc
+-rw-r--r--   0        0        0     1659 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/AuthorizeCoinJoin.cpython-39.pyc
+-rw-r--r--   0        0        0      547 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/BackupDevice.cpython-36.pyc
+-rw-r--r--   0        0        0      551 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/BackupDevice.cpython-37.pyc
+-rw-r--r--   0        0        0      559 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/BackupDevice.cpython-38.pyc
+-rw-r--r--   0        0        0      557 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/BackupDevice.cpython-39.pyc
+-rw-r--r--   0        0        0      348 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/BackupType.cpython-36.pyc
+-rw-r--r--   0        0        0      396 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/BackupType.cpython-37.pyc
+-rw-r--r--   0        0        0      400 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/BackupType.cpython-38.pyc
+-rw-r--r--   0        0        0      398 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/BackupType.cpython-39.pyc
+-rw-r--r--   0        0        0      541 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonAck.cpython-36.pyc
+-rw-r--r--   0        0        0      545 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonAck.cpython-37.pyc
+-rw-r--r--   0        0        0      553 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonAck.cpython-38.pyc
+-rw-r--r--   0        0        0      551 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonAck.cpython-39.pyc
+-rw-r--r--   0        0        0     1378 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonRequest.cpython-36.pyc
+-rw-r--r--   0        0        0     1192 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonRequest.cpython-37.pyc
+-rw-r--r--   0        0        0     1119 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonRequest.cpython-38.pyc
+-rw-r--r--   0        0        0     1115 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonRequest.cpython-39.pyc
+-rw-r--r--   0        0        0      941 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonRequestType.cpython-36.pyc
+-rw-r--r--   0        0        0     1142 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonRequestType.cpython-37.pyc
+-rw-r--r--   0        0        0     1146 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonRequestType.cpython-38.pyc
+-rw-r--r--   0        0        0     1144 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ButtonRequestType.cpython-39.pyc
+-rw-r--r--   0        0        0      535 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Cancel.cpython-36.pyc
+-rw-r--r--   0        0        0      539 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Cancel.cpython-37.pyc
+-rw-r--r--   0        0        0      547 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Cancel.cpython-38.pyc
+-rw-r--r--   0        0        0      545 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Cancel.cpython-39.pyc
+-rw-r--r--   0        0        0      732 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Capability.cpython-36.pyc
+-rw-r--r--   0        0        0      906 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Capability.cpython-37.pyc
+-rw-r--r--   0        0        0      910 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Capability.cpython-38.pyc
+-rw-r--r--   0        0        0      908 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Capability.cpython-39.pyc
+-rw-r--r--   0        0        0      909 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ChangePin.cpython-36.pyc
+-rw-r--r--   0        0        0      913 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ChangePin.cpython-37.pyc
+-rw-r--r--   0        0        0      937 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ChangePin.cpython-38.pyc
+-rw-r--r--   0        0        0      933 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ChangePin.cpython-39.pyc
+-rw-r--r--   0        0        0     1415 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkDecision.cpython-36.pyc
+-rw-r--r--   0        0        0     1389 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkDecision.cpython-37.pyc
+-rw-r--r--   0        0        0     1379 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkDecision.cpython-38.pyc
+-rw-r--r--   0        0        0     1377 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkDecision.cpython-39.pyc
+-rw-r--r--   0        0        0      953 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkEraseSdCard.cpython-36.pyc
+-rw-r--r--   0        0        0      957 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkEraseSdCard.cpython-37.pyc
+-rw-r--r--   0        0        0      981 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkEraseSdCard.cpython-38.pyc
+-rw-r--r--   0        0        0      977 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkEraseSdCard.cpython-39.pyc
+-rw-r--r--   0        0        0      951 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkFlashErase.cpython-36.pyc
+-rw-r--r--   0        0        0      955 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkFlashErase.cpython-37.pyc
+-rw-r--r--   0        0        0      979 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkFlashErase.cpython-38.pyc
+-rw-r--r--   0        0        0      975 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkFlashErase.cpython-39.pyc
+-rw-r--r--   0        0        0     1081 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkGetState.cpython-36.pyc
+-rw-r--r--   0        0        0     1085 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkGetState.cpython-37.pyc
+-rw-r--r--   0        0        0     1101 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkGetState.cpython-38.pyc
+-rw-r--r--   0        0        0     1099 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkGetState.cpython-39.pyc
+-rw-r--r--   0        0        0      935 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemory.cpython-36.pyc
+-rw-r--r--   0        0        0      939 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemory.cpython-37.pyc
+-rw-r--r--   0        0        0      963 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemory.cpython-38.pyc
+-rw-r--r--   0        0        0      959 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemory.cpython-39.pyc
+-rw-r--r--   0        0        0     1013 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemoryRead.cpython-36.pyc
+-rw-r--r--   0        0        0     1017 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemoryRead.cpython-37.pyc
+-rw-r--r--   0        0        0     1036 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemoryRead.cpython-38.pyc
+-rw-r--r--   0        0        0     1034 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemoryRead.cpython-39.pyc
+-rw-r--r--   0        0        0     1109 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemoryWrite.cpython-36.pyc
+-rw-r--r--   0        0        0     1113 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemoryWrite.cpython-37.pyc
+-rw-r--r--   0        0        0     1129 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemoryWrite.cpython-38.pyc
+-rw-r--r--   0        0        0     1127 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkMemoryWrite.cpython-39.pyc
+-rw-r--r--   0        0        0      969 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkRecordScreen.cpython-36.pyc
+-rw-r--r--   0        0        0      973 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkRecordScreen.cpython-37.pyc
+-rw-r--r--   0        0        0      997 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkRecordScreen.cpython-38.pyc
+-rw-r--r--   0        0        0      993 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkRecordScreen.cpython-39.pyc
+-rw-r--r--   0        0        0      958 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkReseedRandom.cpython-36.pyc
+-rw-r--r--   0        0        0      962 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkReseedRandom.cpython-37.pyc
+-rw-r--r--   0        0        0      986 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkReseedRandom.cpython-38.pyc
+-rw-r--r--   0        0        0      982 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkReseedRandom.cpython-39.pyc
+-rw-r--r--   0        0        0     1234 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowText.cpython-36.pyc
+-rw-r--r--   0        0        0     1238 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowText.cpython-37.pyc
+-rw-r--r--   0        0        0     1251 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowText.cpython-38.pyc
+-rw-r--r--   0        0        0     1249 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowText.cpython-39.pyc
+-rw-r--r--   0        0        0     1191 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowTextItem.cpython-36.pyc
+-rw-r--r--   0        0        0     1145 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowTextItem.cpython-37.pyc
+-rw-r--r--   0        0        0     1137 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowTextItem.cpython-38.pyc
+-rw-r--r--   0        0        0     1135 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowTextItem.cpython-39.pyc
+-rw-r--r--   0        0        0      423 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowTextStyle.cpython-36.pyc
+-rw-r--r--   0        0        0      498 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowTextStyle.cpython-37.pyc
+-rw-r--r--   0        0        0      502 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowTextStyle.cpython-38.pyc
+-rw-r--r--   0        0        0      500 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkShowTextStyle.cpython-39.pyc
+-rw-r--r--   0        0        0     1851 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkState.cpython-36.pyc
+-rw-r--r--   0        0        0     1855 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkState.cpython-37.pyc
+-rw-r--r--   0        0        0     1841 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkState.cpython-38.pyc
+-rw-r--r--   0        0        0     1839 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkState.cpython-39.pyc
+-rw-r--r--   0        0        0      549 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkStop.cpython-36.pyc
+-rw-r--r--   0        0        0      553 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkStop.cpython-37.pyc
+-rw-r--r--   0        0        0      561 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkStop.cpython-38.pyc
+-rw-r--r--   0        0        0      559 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkStop.cpython-39.pyc
+-rw-r--r--   0        0        0      952 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkWatchLayout.cpython-36.pyc
+-rw-r--r--   0        0        0      956 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkWatchLayout.cpython-37.pyc
+-rw-r--r--   0        0        0      980 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkWatchLayout.cpython-38.pyc
+-rw-r--r--   0        0        0      976 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugLinkWatchLayout.cpython-39.pyc
+-rw-r--r--   0        0        0      361 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugSwipeDirection.cpython-36.pyc
+-rw-r--r--   0        0        0      418 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugSwipeDirection.cpython-37.pyc
+-rw-r--r--   0        0        0      422 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugSwipeDirection.cpython-38.pyc
+-rw-r--r--   0        0        0      420 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DebugSwipeDirection.cpython-39.pyc
+-rw-r--r--   0        0        0      581 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Deprecated_PassphraseStateAck.cpython-36.pyc
+-rw-r--r--   0        0        0      585 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Deprecated_PassphraseStateAck.cpython-37.pyc
+-rw-r--r--   0        0        0      593 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Deprecated_PassphraseStateAck.cpython-38.pyc
+-rw-r--r--   0        0        0      591 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Deprecated_PassphraseStateAck.cpython-39.pyc
+-rw-r--r--   0        0        0     1006 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Deprecated_PassphraseStateRequest.cpython-36.pyc
+-rw-r--r--   0        0        0     1010 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Deprecated_PassphraseStateRequest.cpython-37.pyc
+-rw-r--r--   0        0        0     1034 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Deprecated_PassphraseStateRequest.cpython-38.pyc
+-rw-r--r--   0        0        0     1030 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Deprecated_PassphraseStateRequest.cpython-39.pyc
+-rw-r--r--   0        0        0      553 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DoPreauthorized.cpython-36.pyc
+-rw-r--r--   0        0        0      557 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DoPreauthorized.cpython-37.pyc
+-rw-r--r--   0        0        0      565 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DoPreauthorized.cpython-38.pyc
+-rw-r--r--   0        0        0      563 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/DoPreauthorized.cpython-39.pyc
+-rw-r--r--   0        0        0      543 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EndSession.cpython-36.pyc
+-rw-r--r--   0        0        0      547 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EndSession.cpython-37.pyc
+-rw-r--r--   0        0        0      555 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EndSession.cpython-38.pyc
+-rw-r--r--   0        0        0      553 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EndSession.cpython-39.pyc
+-rw-r--r--   0        0        0      908 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Entropy.cpython-36.pyc
+-rw-r--r--   0        0        0      912 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Entropy.cpython-37.pyc
+-rw-r--r--   0        0        0      934 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Entropy.cpython-38.pyc
+-rw-r--r--   0        0        0      930 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Entropy.cpython-39.pyc
+-rw-r--r--   0        0        0      916 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EntropyAck.cpython-36.pyc
+-rw-r--r--   0        0        0      920 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EntropyAck.cpython-37.pyc
+-rw-r--r--   0        0        0      944 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EntropyAck.cpython-38.pyc
+-rw-r--r--   0        0        0      940 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EntropyAck.cpython-39.pyc
+-rw-r--r--   0        0        0      551 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EntropyRequest.cpython-36.pyc
+-rw-r--r--   0        0        0      555 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EntropyRequest.cpython-37.pyc
+-rw-r--r--   0        0        0      563 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EntropyRequest.cpython-38.pyc
+-rw-r--r--   0        0        0      561 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/EntropyRequest.cpython-39.pyc
+-rw-r--r--   0        0        0     1327 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Failure.cpython-36.pyc
+-rw-r--r--   0        0        0     1186 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Failure.cpython-37.pyc
+-rw-r--r--   0        0        0     1133 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Failure.cpython-38.pyc
+-rw-r--r--   0        0        0     1131 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Failure.cpython-39.pyc
+-rw-r--r--   0        0        0      772 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FailureType.cpython-36.pyc
+-rw-r--r--   0        0        0      928 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FailureType.cpython-37.pyc
+-rw-r--r--   0        0        0      932 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FailureType.cpython-38.pyc
+-rw-r--r--   0        0        0      930 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FailureType.cpython-39.pyc
+-rw-r--r--   0        0        0     4014 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Features.cpython-36.pyc
+-rw-r--r--   0        0        0     3814 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Features.cpython-37.pyc
+-rw-r--r--   0        0        0     3631 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Features.cpython-38.pyc
+-rw-r--r--   0        0        0     3629 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Features.cpython-39.pyc
+-rw-r--r--   0        0        0      927 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareErase.cpython-36.pyc
+-rw-r--r--   0        0        0      931 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareErase.cpython-37.pyc
+-rw-r--r--   0        0        0      955 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareErase.cpython-38.pyc
+-rw-r--r--   0        0        0      951 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareErase.cpython-39.pyc
+-rw-r--r--   0        0        0      996 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareRequest.cpython-36.pyc
+-rw-r--r--   0        0        0     1000 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareRequest.cpython-37.pyc
+-rw-r--r--   0        0        0     1019 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareRequest.cpython-38.pyc
+-rw-r--r--   0        0        0     1017 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareRequest.cpython-39.pyc
+-rw-r--r--   0        0        0      999 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareUpload.cpython-36.pyc
+-rw-r--r--   0        0        0     1003 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareUpload.cpython-37.pyc
+-rw-r--r--   0        0        0     1029 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareUpload.cpython-38.pyc
+-rw-r--r--   0        0        0     1027 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/FirmwareUpload.cpython-39.pyc
+-rw-r--r--   0        0        0     1555 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetAddress.cpython-36.pyc
+-rw-r--r--   0        0        0     1529 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetAddress.cpython-37.pyc
+-rw-r--r--   0        0        0     1514 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetAddress.cpython-38.pyc
+-rw-r--r--   0        0        0     1512 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetAddress.cpython-39.pyc
+-rw-r--r--   0        0        0      917 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetEntropy.cpython-36.pyc
+-rw-r--r--   0        0        0      921 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetEntropy.cpython-37.pyc
+-rw-r--r--   0        0        0      943 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetEntropy.cpython-38.pyc
+-rw-r--r--   0        0        0      939 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetEntropy.cpython-39.pyc
+-rw-r--r--   0        0        0      545 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetFeatures.cpython-36.pyc
+-rw-r--r--   0        0        0      549 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetFeatures.cpython-37.pyc
+-rw-r--r--   0        0        0      557 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetFeatures.cpython-38.pyc
+-rw-r--r--   0        0        0      555 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetFeatures.cpython-39.pyc
+-rw-r--r--   0        0        0     1420 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetOwnershipId.cpython-36.pyc
+-rw-r--r--   0        0        0     1394 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetOwnershipId.cpython-37.pyc
+-rw-r--r--   0        0        0     1385 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetOwnershipId.cpython-38.pyc
+-rw-r--r--   0        0        0     1383 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetOwnershipId.cpython-39.pyc
+-rw-r--r--   0        0        0     1700 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetOwnershipProof.cpython-36.pyc
+-rw-r--r--   0        0        0     1674 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetOwnershipProof.cpython-37.pyc
+-rw-r--r--   0        0        0     1656 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetOwnershipProof.cpython-38.pyc
+-rw-r--r--   0        0        0     1654 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetOwnershipProof.cpython-39.pyc
+-rw-r--r--   0        0        0     1516 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetPublicKey.cpython-36.pyc
+-rw-r--r--   0        0        0     1485 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetPublicKey.cpython-37.pyc
+-rw-r--r--   0        0        0     1470 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetPublicKey.cpython-38.pyc
+-rw-r--r--   0        0        0     1468 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/GetPublicKey.cpython-39.pyc
+-rw-r--r--   0        0        0     1055 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/HDNodePathType.cpython-36.pyc
+-rw-r--r--   0        0        0     1059 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/HDNodePathType.cpython-37.pyc
+-rw-r--r--   0        0        0     1085 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/HDNodePathType.cpython-38.pyc
+-rw-r--r--   0        0        0     1083 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/HDNodePathType.cpython-39.pyc
+-rw-r--r--   0        0        0     1200 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/HDNodeType.cpython-36.pyc
+-rw-r--r--   0        0        0     1204 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/HDNodeType.cpython-37.pyc
+-rw-r--r--   0        0        0     1238 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/HDNodeType.cpython-38.pyc
+-rw-r--r--   0        0        0     1236 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/HDNodeType.cpython-39.pyc
+-rw-r--r--   0        0        0      919 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Initialize.cpython-36.pyc
+-rw-r--r--   0        0        0      923 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Initialize.cpython-37.pyc
+-rw-r--r--   0        0        0      947 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Initialize.cpython-38.pyc
+-rw-r--r--   0        0        0      943 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Initialize.cpython-39.pyc
+-rw-r--r--   0        0        0      424 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/InputScriptType.cpython-36.pyc
+-rw-r--r--   0        0        0      490 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/InputScriptType.cpython-37.pyc
+-rw-r--r--   0        0        0      494 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/InputScriptType.cpython-38.pyc
+-rw-r--r--   0        0        0      492 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/InputScriptType.cpython-39.pyc
+-rw-r--r--   0        0        0     1512 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/LoadDevice.cpython-36.pyc
+-rw-r--r--   0        0        0     1516 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/LoadDevice.cpython-37.pyc
+-rw-r--r--   0        0        0     1512 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/LoadDevice.cpython-38.pyc
+-rw-r--r--   0        0        0     1510 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/LoadDevice.cpython-39.pyc
+-rw-r--r--   0        0        0      543 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/LockDevice.cpython-36.pyc
+-rw-r--r--   0        0        0      547 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/LockDevice.cpython-37.pyc
+-rw-r--r--   0        0        0      555 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/LockDevice.cpython-38.pyc
+-rw-r--r--   0        0        0      553 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/LockDevice.cpython-39.pyc
+-rw-r--r--   0        0        0     1022 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MessageSignature.cpython-36.pyc
+-rw-r--r--   0        0        0     1026 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MessageSignature.cpython-37.pyc
+-rw-r--r--   0        0        0     1045 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MessageSignature.cpython-38.pyc
+-rw-r--r--   0        0        0     1043 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MessageSignature.cpython-39.pyc
+-rw-r--r--   0        0        0     2471 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MessageType.cpython-36.pyc
+-rw-r--r--   0        0        0     3077 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MessageType.cpython-37.pyc
+-rw-r--r--   0        0        0     3081 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MessageType.cpython-38.pyc
+-rw-r--r--   0        0        0     3079 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MessageType.cpython-39.pyc
+-rw-r--r--   0        0        0     1390 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MultisigRedeemScriptType.cpython-36.pyc
+-rw-r--r--   0        0        0     1394 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MultisigRedeemScriptType.cpython-37.pyc
+-rw-r--r--   0        0        0     1426 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MultisigRedeemScriptType.cpython-38.pyc
+-rw-r--r--   0        0        0     1424 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/MultisigRedeemScriptType.cpython-39.pyc
+-rw-r--r--   0        0        0      466 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OutputScriptType.cpython-36.pyc
+-rw-r--r--   0        0        0      541 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OutputScriptType.cpython-37.pyc
+-rw-r--r--   0        0        0      545 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OutputScriptType.cpython-38.pyc
+-rw-r--r--   0        0        0      543 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OutputScriptType.cpython-39.pyc
+-rw-r--r--   0        0        0      929 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OwnershipId.cpython-36.pyc
+-rw-r--r--   0        0        0      933 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OwnershipId.cpython-37.pyc
+-rw-r--r--   0        0        0      955 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OwnershipId.cpython-38.pyc
+-rw-r--r--   0        0        0      951 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OwnershipId.cpython-39.pyc
+-rw-r--r--   0        0        0     1003 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OwnershipProof.cpython-36.pyc
+-rw-r--r--   0        0        0     1007 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OwnershipProof.cpython-37.pyc
+-rw-r--r--   0        0        0     1027 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OwnershipProof.cpython-38.pyc
+-rw-r--r--   0        0        0     1025 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/OwnershipProof.cpython-39.pyc
+-rw-r--r--   0        0        0     1088 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PassphraseAck.cpython-36.pyc
+-rw-r--r--   0        0        0     1092 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PassphraseAck.cpython-37.pyc
+-rw-r--r--   0        0        0     1108 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PassphraseAck.cpython-38.pyc
+-rw-r--r--   0        0        0     1106 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PassphraseAck.cpython-39.pyc
+-rw-r--r--   0        0        0      945 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PassphraseRequest.cpython-36.pyc
+-rw-r--r--   0        0        0      949 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PassphraseRequest.cpython-37.pyc
+-rw-r--r--   0        0        0      973 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PassphraseRequest.cpython-38.pyc
+-rw-r--r--   0        0        0      969 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PassphraseRequest.cpython-39.pyc
+-rw-r--r--   0        0        0      924 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixAck.cpython-36.pyc
+-rw-r--r--   0        0        0      928 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixAck.cpython-37.pyc
+-rw-r--r--   0        0        0      950 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixAck.cpython-38.pyc
+-rw-r--r--   0        0        0      946 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixAck.cpython-39.pyc
+-rw-r--r--   0        0        0     1096 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixRequest.cpython-36.pyc
+-rw-r--r--   0        0        0     1060 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixRequest.cpython-37.pyc
+-rw-r--r--   0        0        0     1062 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixRequest.cpython-38.pyc
+-rw-r--r--   0        0        0     1058 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixRequest.cpython-39.pyc
+-rw-r--r--   0        0        0      424 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixRequestType.cpython-36.pyc
+-rw-r--r--   0        0        0      490 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixRequestType.cpython-37.pyc
+-rw-r--r--   0        0        0      494 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixRequestType.cpython-38.pyc
+-rw-r--r--   0        0        0      492 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PinMatrixRequestType.cpython-39.pyc
+-rw-r--r--   0        0        0      980 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Ping.cpython-36.pyc
+-rw-r--r--   0        0        0      984 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Ping.cpython-37.pyc
+-rw-r--r--   0        0        0     1003 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Ping.cpython-38.pyc
+-rw-r--r--   0        0        0     1001 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Ping.cpython-39.pyc
+-rw-r--r--   0        0        0      563 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PreauthorizedRequest.cpython-36.pyc
+-rw-r--r--   0        0        0      567 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PreauthorizedRequest.cpython-37.pyc
+-rw-r--r--   0        0        0      575 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PreauthorizedRequest.cpython-38.pyc
+-rw-r--r--   0        0        0      573 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PreauthorizedRequest.cpython-39.pyc
+-rw-r--r--   0        0        0     1101 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PublicKey.cpython-36.pyc
+-rw-r--r--   0        0        0     1105 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PublicKey.cpython-37.pyc
+-rw-r--r--   0        0        0     1121 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PublicKey.cpython-38.pyc
+-rw-r--r--   0        0        0     1119 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/PublicKey.cpython-39.pyc
+-rw-r--r--   0        0        0     1599 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RecoveryDevice.cpython-36.pyc
+-rw-r--r--   0        0        0     1588 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RecoveryDevice.cpython-37.pyc
+-rw-r--r--   0        0        0     1579 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RecoveryDevice.cpython-38.pyc
+-rw-r--r--   0        0        0     1577 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RecoveryDevice.cpython-39.pyc
+-rw-r--r--   0        0        0      323 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RecoveryDeviceType.cpython-36.pyc
+-rw-r--r--   0        0        0      362 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RecoveryDeviceType.cpython-37.pyc
+-rw-r--r--   0        0        0      366 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RecoveryDeviceType.cpython-38.pyc
+-rw-r--r--   0        0        0      364 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RecoveryDeviceType.cpython-39.pyc
+-rw-r--r--   0        0        0      466 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RequestType.cpython-36.pyc
+-rw-r--r--   0        0        0      550 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RequestType.cpython-37.pyc
+-rw-r--r--   0        0        0      554 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RequestType.cpython-38.pyc
+-rw-r--r--   0        0        0      552 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/RequestType.cpython-39.pyc
+-rw-r--r--   0        0        0     1684 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ResetDevice.cpython-36.pyc
+-rw-r--r--   0        0        0     1673 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ResetDevice.cpython-37.pyc
+-rw-r--r--   0        0        0     1654 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ResetDevice.cpython-38.pyc
+-rw-r--r--   0        0        0     1652 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/ResetDevice.cpython-39.pyc
+-rw-r--r--   0        0        0      357 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SafetyCheckLevel.cpython-36.pyc
+-rw-r--r--   0        0        0      405 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SafetyCheckLevel.cpython-37.pyc
+-rw-r--r--   0        0        0      409 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SafetyCheckLevel.cpython-38.pyc
+-rw-r--r--   0        0        0      407 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SafetyCheckLevel.cpython-39.pyc
+-rw-r--r--   0        0        0      908 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SelfTest.cpython-36.pyc
+-rw-r--r--   0        0        0      912 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SelfTest.cpython-37.pyc
+-rw-r--r--   0        0        0      936 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SelfTest.cpython-38.pyc
+-rw-r--r--   0        0        0      932 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SelfTest.cpython-39.pyc
+-rw-r--r--   0        0        0     1378 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SignMessage.cpython-36.pyc
+-rw-r--r--   0        0        0     1347 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SignMessage.cpython-37.pyc
+-rw-r--r--   0        0        0     1355 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SignMessage.cpython-38.pyc
+-rw-r--r--   0        0        0     1353 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SignMessage.cpython-39.pyc
+-rw-r--r--   0        0        0     1734 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SignTx.cpython-36.pyc
+-rw-r--r--   0        0        0     1718 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SignTx.cpython-37.pyc
+-rw-r--r--   0        0        0     1745 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SignTx.cpython-38.pyc
+-rw-r--r--   0        0        0     1743 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/SignTx.cpython-39.pyc
+-rw-r--r--   0        0        0      904 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Success.cpython-36.pyc
+-rw-r--r--   0        0        0      908 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Success.cpython-37.pyc
+-rw-r--r--   0        0        0      932 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Success.cpython-38.pyc
+-rw-r--r--   0        0        0      928 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/Success.cpython-39.pyc
+-rw-r--r--   0        0        0     1971 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TransactionType.cpython-36.pyc
+-rw-r--r--   0        0        0     1975 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TransactionType.cpython-37.pyc
+-rw-r--r--   0        0        0     1958 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TransactionType.cpython-38.pyc
+-rw-r--r--   0        0        0     1956 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TransactionType.cpython-39.pyc
+-rw-r--r--   0        0        0      919 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxAck.cpython-36.pyc
+-rw-r--r--   0        0        0      923 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxAck.cpython-37.pyc
+-rw-r--r--   0        0        0      945 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxAck.cpython-38.pyc
+-rw-r--r--   0        0        0      941 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxAck.cpython-39.pyc
+-rw-r--r--   0        0        0     2018 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxInputType.cpython-36.pyc
+-rw-r--r--   0        0        0     1992 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxInputType.cpython-37.pyc
+-rw-r--r--   0        0        0     2014 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxInputType.cpython-38.pyc
+-rw-r--r--   0        0        0     2012 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxInputType.cpython-39.pyc
+-rw-r--r--   0        0        0     1066 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxOutputBinType.cpython-36.pyc
+-rw-r--r--   0        0        0     1070 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxOutputBinType.cpython-37.pyc
+-rw-r--r--   0        0        0     1098 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxOutputBinType.cpython-38.pyc
+-rw-r--r--   0        0        0     1096 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxOutputBinType.cpython-39.pyc
+-rw-r--r--   0        0        0     1665 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxOutputType.cpython-36.pyc
+-rw-r--r--   0        0        0     1629 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxOutputType.cpython-37.pyc
+-rw-r--r--   0        0        0     1640 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxOutputType.cpython-38.pyc
+-rw-r--r--   0        0        0     1638 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxOutputType.cpython-39.pyc
+-rw-r--r--   0        0        0     1328 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequest.cpython-36.pyc
+-rw-r--r--   0        0        0     1277 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequest.cpython-37.pyc
+-rw-r--r--   0        0        0     1261 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequest.cpython-38.pyc
+-rw-r--r--   0        0        0     1259 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequest.cpython-39.pyc
+-rw-r--r--   0        0        0     1149 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequestDetailsType.cpython-36.pyc
+-rw-r--r--   0        0        0     1153 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequestDetailsType.cpython-37.pyc
+-rw-r--r--   0        0        0     1166 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequestDetailsType.cpython-38.pyc
+-rw-r--r--   0        0        0     1164 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequestDetailsType.cpython-39.pyc
+-rw-r--r--   0        0        0     1094 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequestSerializedType.cpython-36.pyc
+-rw-r--r--   0        0        0     1098 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequestSerializedType.cpython-37.pyc
+-rw-r--r--   0        0        0     1114 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequestSerializedType.cpython-38.pyc
+-rw-r--r--   0        0        0     1112 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/TxRequestSerializedType.cpython-39.pyc
+-rw-r--r--   0        0        0     1140 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/VerifyMessage.cpython-36.pyc
+-rw-r--r--   0        0        0     1144 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/VerifyMessage.cpython-37.pyc
+-rw-r--r--   0        0        0     1174 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/VerifyMessage.cpython-38.pyc
+-rw-r--r--   0        0        0     1172 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/VerifyMessage.cpython-39.pyc
+-rw-r--r--   0        0        0      543 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WipeDevice.cpython-36.pyc
+-rw-r--r--   0        0        0      547 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WipeDevice.cpython-37.pyc
+-rw-r--r--   0        0        0      555 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WipeDevice.cpython-38.pyc
+-rw-r--r--   0        0        0      553 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WipeDevice.cpython-39.pyc
+-rw-r--r--   0        0        0      905 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordAck.cpython-36.pyc
+-rw-r--r--   0        0        0      909 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordAck.cpython-37.pyc
+-rw-r--r--   0        0        0      931 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordAck.cpython-38.pyc
+-rw-r--r--   0        0        0      927 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordAck.cpython-39.pyc
+-rw-r--r--   0        0        0     1021 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordRequest.cpython-36.pyc
+-rw-r--r--   0        0        0     1010 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordRequest.cpython-37.pyc
+-rw-r--r--   0        0        0     1022 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordRequest.cpython-38.pyc
+-rw-r--r--   0        0        0     1018 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordRequest.cpython-39.pyc
+-rw-r--r--   0        0        0      340 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordRequestType.cpython-36.pyc
+-rw-r--r--   0        0        0      388 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordRequestType.cpython-37.pyc
+-rw-r--r--   0        0        0      392 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordRequestType.cpython-38.pyc
+-rw-r--r--   0        0        0      390 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/WordRequestType.cpython-39.pyc
+-rw-r--r--   0        0        0     3468 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     3472 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     3476 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3476 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    72766 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/messages.py
+-rw-r--r--   0        0        0      935 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/models.py
+-rw-r--r--   0        0        0    20415 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/protobuf.py
+-rw-r--r--   0        0        0    10087 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/tools.py
+-rw-r--r--   0        0        0     4913 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__init__.py
+-rw-r--r--   0        0        0     7846 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4936 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     4941 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     5008 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4998 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8593 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-311.pyc
+-rw-r--r--   0        0        0     4696 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-36.pyc
+-rw-r--r--   0        0        0     4700 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-37.pyc
+-rw-r--r--   0        0        0     4725 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-38.pyc
+-rw-r--r--   0        0        0     4725 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-39.pyc
+-rw-r--r--   0        0        0     8879 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-311.pyc
+-rw-r--r--   0        0        0     6090 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-36.pyc
+-rw-r--r--   0        0        0     6094 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-37.pyc
+-rw-r--r--   0        0        0     6109 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-38.pyc
+-rw-r--r--   0        0        0     6107 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-39.pyc
+-rw-r--r--   0        0        0     8135 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-311.pyc
+-rw-r--r--   0        0        0     4245 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-36.pyc
+-rw-r--r--   0        0        0     4249 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-37.pyc
+-rw-r--r--   0        0        0     4294 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-38.pyc
+-rw-r--r--   0        0        0     4290 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-39.pyc
+-rw-r--r--   0        0        0     8657 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-311.pyc
+-rw-r--r--   0        0        0     4791 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-36.pyc
+-rw-r--r--   0        0        0     4800 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-37.pyc
+-rw-r--r--   0        0        0     4828 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-38.pyc
+-rw-r--r--   0        0        0     4794 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-39.pyc
+-rw-r--r--   0        0        0     5374 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/hid.py
+-rw-r--r--   0        0        0     5372 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/protocol.py
+-rw-r--r--   0        0        0     4881 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/udp.py
+-rw-r--r--   0        0        0     5315 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/devices/trezorlib/transport/webusb.py
+-rw-r--r--   0        0        0     7048 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/errors.py
+-rw-r--r--   0        0        0     9167 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/hwwclient.py
+-rw-r--r--   0        0        0    14015 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/key.py
+-rw-r--r--   0        0        0    46452 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/psbt.py
+-rw-r--r--   0        0        0        0 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/py.typed
+-rw-r--r--   0        0        0     9191 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/tx.py
+-rw-r--r--   0        0        0     1756 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/20-hw1.rules
+-rw-r--r--   0        0        0      310 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/51-coinkite.rules
+-rw-r--r--   0        0        0      119 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/51-hid-digitalbitbox.rules
+-rw-r--r--   0        0        0      980 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/51-trezor.rules
+-rw-r--r--   0        0        0      769 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/51-usb-keepkey.rules
+-rw-r--r--   0        0        0      142 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/52-hid-digitalbitbox.rules
+-rw-r--r--   0        0        0      125 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/53-hid-bitbox02.rules
+-rw-r--r--   0        0        0      147 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/54-hid-bitbox02.rules
+-rw-r--r--   0        0        0      340 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/55-usb-jade.rules
+-rw-r--r--   0        0        0     1158 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udev/README.md
+-rw-r--r--   0        0        0     3416 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/udevinstaller.py
+-rw-r--r--   0        0        0     1919 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_bitbox02pairing.cpython-39.pyc
+-rw-r--r--   0        0        0     3060 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_displayaddressdialog.cpython-39.pyc
+-rw-r--r--   0        0        0     3104 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_getkeypooloptionsdialog.cpython-39.pyc
+-rw-r--r--   0        0        0     2052 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_getxpubdialog.cpython-39.pyc
+-rw-r--r--   0        0        0     4349 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_mainwindow.cpython-39.pyc
+-rw-r--r--   0        0        0     2690 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_sendpindialog.cpython-39.pyc
+-rw-r--r--   0        0        0     1503 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_setpassphrasedialog.cpython-39.pyc
+-rw-r--r--   0        0        0     2451 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_signmessagedialog.cpython-39.pyc
+-rw-r--r--   0        0        0     3023 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/__pycache__/ui_signpsbtdialog.cpython-39.pyc
+-rw-r--r--   0        0        0     2687 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/bitbox02pairing.ui
+-rw-r--r--   0        0        0     5382 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/displayaddressdialog.ui
+-rw-r--r--   0        0        0     6167 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/getkeypooloptionsdialog.ui
+-rw-r--r--   0        0        0     2872 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/getxpubdialog.ui
+-rw-r--r--   0        0        0      196 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/hwiqt.pyproject
+-rw-r--r--   0        0        0     7628 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/mainwindow.ui
+-rw-r--r--   0        0        0     4431 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/sendpindialog.ui
+-rw-r--r--   0        0        0     2117 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/setpassphrasedialog.ui
+-rw-r--r--   0        0        0     4378 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/signmessagedialog.ui
+-rw-r--r--   0        0        0     6092 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/signpsbtdialog.ui
+-rw-r--r--   0        0        0     2545 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_bitbox02pairing.py
+-rw-r--r--   0        0        0     5435 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_displayaddressdialog.py
+-rw-r--r--   0        0        0     5724 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_getkeypooloptionsdialog.py
+-rw-r--r--   0        0        0     3151 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_getxpubdialog.py
+-rw-r--r--   0        0        0     8994 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_mainwindow.py
+-rw-r--r--   0        0        0     4729 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_sendpindialog.py
+-rw-r--r--   0        0        0     2057 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_setpassphrasedialog.py
+-rw-r--r--   0        0        0     4017 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_signmessagedialog.py
+-rw-r--r--   0        0        0     5419 2019-01-01 00:00:00.000000 hwi-2.3.0/hwilib/ui/ui_signpsbtdialog.py
+-rw-r--r--   0        0        0     1283 2019-01-01 00:00:00.000000 hwi-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5414 1970-01-01 00:00:00.000000 hwi-2.3.0/setup.py
+-rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 hwi-2.3.0/PKG-INFO
```

### Comparing `hwi-2.2.1/LICENSE` & `hwi-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/README.md` & `hwi-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/_base58.py` & `hwi-2.3.0/hwilib/_base58.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,34 @@
     for c in s[:-1]:
         if c == b58_digits[0]:
             pad += 1
         else:
             break
     return b'\x00' * pad + res
 
+def decode_check(s: str) -> bytes:
+    """
+    Decode a Base58Check encoded string, returning bytes
+
+    :param s: Base58 string to decode
+    :return: Bytes encoded by ``s``
+    """
+    data = decode(s)
+    payload = data[:-4]
+    checksum = data[-4:]
+    calc_checksum = hash256(payload)
+    if checksum != calc_checksum:
+        raise ValueError("Invalid checksum")
+    return payload
+
+def encode_check(b: bytes) -> str:
+    checksum = hash256(b)[0:4]
+    data = b + checksum
+    return encode(data)
+
 def get_xpub_fingerprint(s: str) -> bytes:
     """
     Get the parent fingerprint from an extended public key
 
     :param s: The extended pubkey
     :return: The parent fingerprint bytes
     """
```

### Comparing `hwi-2.2.1/hwilib/_bech32.py` & `hwi-2.3.0/hwilib/_bech32.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/_cli.py` & `hwi-2.3.0/hwilib/_cli.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/_gui.py` & `hwi-2.3.0/hwilib/_gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #! /usr/bin/env python3
 
+import base64
 import json
 import logging
 import sys
 import time
 from typing import Callable
 
 from . import commands, __version__
@@ -22,19 +23,17 @@
     from .ui.ui_signmessagedialog import Ui_SignMessageDialog
     from .ui.ui_signpsbtdialog import Ui_SignPSBTDialog
 except ImportError:
     print('Could not import UI files, did you run contrib/generate-ui.sh')
     exit(-1)
 
 from PySide2.QtGui import QRegExpValidator
-from PySide2.QtWidgets import QApplication, QDialog, QDialogButtonBox, QLineEdit, QMessageBox, QMainWindow
+from PySide2.QtWidgets import QApplication, QDialog, QDialogButtonBox, QFileDialog, QLineEdit, QMessageBox, QMainWindow, QMenu
 from PySide2.QtCore import QCoreApplication, QRegExp, Signal, Slot
 
-import bitbox02.util
-
 def do_command(f, *args, **kwargs):
     result = {}
     with handle_errors(result=result):
         result = f(*args, **kwargs)
     if 'error' in result:
         msg = 'Error: {}\nCode:{}'.format(result['error'], result['code'])
         QMessageBox.critical(None, "An Error Occurred", msg)
@@ -123,14 +122,60 @@
         self.client = client
 
         self.ui.psbt_in_textedit.setFocus()
 
         self.ui.sign_psbt_button.clicked.connect(self.sign_psbt_button_clicked)
         self.ui.buttonBox.clicked.connect(self.accept)
 
+        menu = QMenu()
+        self.ui.import_toolbutton.setMenu(menu)
+        menu = self.ui.import_toolbutton.menu()
+        menu.addAction("From binary").triggered.connect(self.import_binary_clicked)
+        menu.addAction("From base64").triggered.connect(self.import_base64_clicked)
+
+        menu = QMenu()
+        self.ui.export_toolbutton.setMenu(menu)
+        menu = self.ui.export_toolbutton.menu()
+        menu.addAction("To binary").triggered.connect(self.export_binary_clicked)
+        menu.addAction("To base64").triggered.connect(self.export_base64_clicked)
+
+    @Slot()
+    def import_base64_clicked(self):
+        filename, _ = QFileDialog.getOpenFileName(self, 'Open file')
+        if filename:
+            with open(filename, 'r', encoding='utf-8') as f:
+                b64 = f.read()
+                self.ui.psbt_in_textedit.setPlainText(b64)
+
+    @Slot()
+    def import_binary_clicked(self):
+        filename, _ = QFileDialog.getOpenFileName(self, 'Open file', "", "PSBT (*.psbt)")
+        if filename:
+            with open(filename, 'rb') as f:
+                bin = f.read()
+                b64 = base64.b64encode(bin).decode()
+                self.ui.psbt_in_textedit.setPlainText(b64)
+
+    @Slot()
+    def export_base64_clicked(self):
+        filename, _ = QFileDialog.getSaveFileName(self, 'Save file')
+        if filename:
+            with open(filename, 'w') as f:
+                b64 = self.ui.psbt_out_textedit.toPlainText()
+                f.write(b64)
+
+    @Slot()
+    def export_binary_clicked(self):
+        filename, _ = QFileDialog.getSaveFileName(self, 'Save file', "untitled.psbt")
+        if filename:
+            with open(filename, 'wb') as f:
+                b64 = self.ui.psbt_out_textedit.toPlainText()
+                bin = base64.b64decode(b64.encode())
+                f.write(bin)
+
     @Slot()
     def sign_psbt_button_clicked(self):
         psbt_str = self.ui.psbt_in_textedit.toPlainText()
         res = do_command(commands.signtx, self.client, psbt_str)
         self.ui.psbt_out_textedit.setPlainText(res['psbt'])
 
 class SignMessageDialog(QDialog):
@@ -218,60 +263,69 @@
         if checked:
             self.ui.path_lineedit.setEnabled(False)
             self.ui.account_spinbox.setEnabled(True)
         else:
             self.ui.path_lineedit.setEnabled(True)
             self.ui.account_spinbox.setEnabled(False)
 
-class BitBox02PairingDialog(QDialog):
-    def __init__(self, pairing_code: str, device_response: Callable[[], bool]):
-        super(BitBox02PairingDialog, self).__init__()
-        self.ui = Ui_BitBox02PairingDialog()
-        self.ui.setupUi(self)
-        self.setWindowTitle('Verify BitBox02 pairing code')
-        self.ui.pairingCode.setText(pairing_code.replace("\n", "<br>"))
-        self.ui.buttonBox.setEnabled(False)
-        self.device_response = device_response
-        self.painted = False
-
-    def paintEvent(self, ev):
-        super().paintEvent(ev)
-        self.painted = True
-
-    def enable_buttons(self):
-        self.ui.buttonBox.setEnabled(True)
-
-class BitBox02NoiseConfig(bitbox02.util.BitBoxAppNoiseConfig):
-    """ GUI elements to perform the BitBox02 pairing and attestatoin check """
-
-    def show_pairing(self, code: str, device_response: Callable[[], bool]) -> bool:
-        dialog = BitBox02PairingDialog(code, device_response)
-        dialog.show()
-        # render the window since the next operation is blocking
-        while True:
-            QCoreApplication.processEvents()
-            if dialog.painted:
-                break
-            time.sleep(0.1)
-        if not device_response():
-            return False
-        dialog.enable_buttons()
-        dialog.exec_()
-        return dialog.result() == QDialog.Accepted
-
-    def attestation_check(self, result: bool) -> None:
-        if not result:
-            QMessageBox.warning(
-                None,
-                "BitBox02 attestation check",
-                "BitBox02 attestation check failed. Your BitBox02 might not be genuine. Please contact support@shiftcrypto.ch if the problem persists.",
-            )
+try:
+    # Try to import bitbox02 things
+    # Not all dependencies may be available, in which case just ignore these two classes
+    # The code that needs this should already be (implicitly) guarded by bitbox02_lib imports working
+    # so these classes will not be referenced in that case.
+    from .devices.bitbox02_lib.util import BitBoxAppNoiseConfig
+
+    class BitBox02PairingDialog(QDialog):
+        def __init__(self, pairing_code: str, device_response: Callable[[], bool]):
+            super(BitBox02PairingDialog, self).__init__()
+            self.ui = Ui_BitBox02PairingDialog()
+            self.ui.setupUi(self)
+            self.setWindowTitle('Verify BitBox02 pairing code')
+            self.ui.pairingCode.setText(pairing_code.replace("\n", "<br>"))
+            self.ui.buttonBox.setEnabled(False)
+            self.device_response = device_response
+            self.painted = False
+
+        def paintEvent(self, ev):
+            super().paintEvent(ev)
+            self.painted = True
+
+        def enable_buttons(self):
+            self.ui.buttonBox.setEnabled(True)
+
+    class BitBox02NoiseConfig(BitBoxAppNoiseConfig):
+        """ GUI elements to perform the BitBox02 pairing and attestatoin check """
+
+        def show_pairing(self, code: str, device_response: Callable[[], bool]) -> bool:
+            dialog = BitBox02PairingDialog(code, device_response)
+            dialog.show()
+            # render the window since the next operation is blocking
+            while True:
+                QCoreApplication.processEvents()
+                if dialog.painted:
+                    break
+                time.sleep(0.1)
+            if not device_response():
+                return False
+            dialog.enable_buttons()
+            dialog.exec_()
+            return dialog.result() == QDialog.Accepted
+
+        def attestation_check(self, result: bool) -> None:
+            if not result:
+                QMessageBox.warning(
+                    None,
+                    "BitBox02 attestation check",
+                    "BitBox02 attestation check failed. Your BitBox02 might not be genuine. Please contact support@shiftcrypto.ch if the problem persists.",
+                )
+except ImportError:
+    pass
 
 class HWIQt(QMainWindow):
-    def __init__(self, passphrase='', chain=Chain.MAIN):
+    def __init__(self, passphrase=None, chain=Chain.MAIN):
         super(HWIQt, self).__init__()
         self.ui = Ui_MainWindow()
         self.ui.setupUi(self)
         self.setWindowTitle('HWI Qt')
 
         self.devices = []
         self.client = None
@@ -462,15 +516,15 @@
     def toggle_passphrase(self):
         do_command(commands.toggle_passphrase, self.client)
         if self.device_info['model'] == "keepkey":
             self.show_sendpindialog(prompt_pin=False)
 
 def process_gui_commands(cli_args):
     parser = HWIArgumentParser(description='Hardware Wallet Interface Qt, version {}.\nInteractively access and send commands to a hardware wallet device with a GUI. Responses are in JSON format.'.format(__version__))
-    parser.add_argument('--password', '-p', help='Device password if it has one (e.g. DigitalBitbox)', default='')
+    parser.add_argument('--password', '-p', help='Device password if it has one (e.g. DigitalBitbox)', default=None)
     parser.add_argument('--chain', help='Select chain to work with', type=Chain.argparse, choices=list(Chain), default=Chain.MAIN)
     parser.add_argument('--debug', help='Print debug statements', action='store_true')
     parser.add_argument('--version', action='version', version='%(prog)s {}'.format(__version__))
 
     # Parse arguments again for anything entered over stdin
     args = parser.parse_args(cli_args)
```

### Comparing `hwi-2.2.1/hwilib/_script.py` & `hwi-2.3.0/hwilib/_script.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/_serialize.py` & `hwi-2.3.0/hwilib/_serialize.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/commands.py` & `hwi-2.3.0/hwilib/commands.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/common.py` & `hwi-2.3.0/hwilib/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     MAIN = 0 #: Bitcoin Main network
     TEST = 1 #: Bitcoin Test network
     REGTEST = 2 #: Bitcoin Core Regression Test network
     SIGNET = 3 #: Bitcoin Signet
 
     def __str__(self) -> str:
-        return self.name.lower()
+        return str(self.name).lower()
 
     def __repr__(self) -> str:
         return str(self)
 
     @staticmethod
     def argparse(s: str) -> Union['Chain', str]:
         try:
@@ -39,15 +39,15 @@
     """
     LEGACY = 1 #: Legacy address type. P2PKH for single sig, P2SH for scripts.
     WIT = 2 #: Native segwit v0 address type. P2WPKH for single sig, P2WPSH for scripts.
     SH_WIT = 3 #: Nested segwit v0 address type. P2SH-P2WPKH for single sig, P2SH-P2WPSH for scripts.
     TAP = 4 #: Segwit v1 Taproot address type. P2TR always.
 
     def __str__(self) -> str:
-        return self.name.lower()
+        return str(self.name).lower()
 
     def __repr__(self) -> str:
         return str(self)
 
     @staticmethod
     def argparse(s: str) -> Union['AddressType', str]:
         try:
```

### Comparing `hwi-2.2.1/hwilib/descriptor.py` & `hwi-2.3.0/hwilib/descriptor.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/bitbox02.py` & `hwi-2.3.0/hwilib/devices/bitbox02.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
     TypeVar,
 )
 import base64
 import builtins
 import sys
 from functools import wraps
 
-import base58
-
+from .._base58 import decode_check, encode_check
 from ..descriptor import MultisigDescriptor
 from ..hwwclient import HardwareWalletClient
 from ..key import ExtendedKey
 from .._script import (
     is_p2pkh,
     is_p2wpkh,
     is_p2wsh,
@@ -58,27 +57,27 @@
 from ..common import (
     AddressType,
     Chain,
 )
 
 import hid
 
-from bitbox02 import util
-from bitbox02 import bitbox02
-from bitbox02.communication import (
+from .bitbox02_lib import util
+from .bitbox02_lib import bitbox02
+from .bitbox02_lib.communication import (
     devices,
     u2fhid,
     FirmwareVersionOutdatedException,
     Bitbox02Exception,
     UserAbortException,
     HARDENED,
     ERR_GENERIC,
 )
 
-from bitbox02.communication.bitbox_api_protocol import (
+from .bitbox02_lib.communication.bitbox_api_protocol import (
     Platform,
     BitBox02Edition,
     BitBoxNoiseConfig,
 )
 
 class BitBox02Error(UnavailableActionError):
     def __init__(self, msg: str):
@@ -419,15 +418,15 @@
         our_account_keypath = None
 
         xpubs: List[bytes] = []
         for i, (xpub, keyinfo) in builtins.enumerate(origin_infos.items()):
             xpubs.append(xpub)
             if device_fingerprint == keyinfo.fingerprint and keyinfo.path:
                 if _xpubs_equal_ignoring_version(
-                    base58.b58decode_check(self._get_xpub(keyinfo.path)), xpub
+                    decode_check(self._get_xpub(keyinfo.path)), xpub
                 ):
                     our_xpub_index = i
                     our_account_keypath = keyinfo.path
 
         if our_xpub_index is None:
             raise BadArgumentError("This BitBox02 is not one of the cosigners")
         assert our_account_keypath
@@ -437,15 +436,15 @@
 
         return (
             xpubs[our_xpub_index],
             bitbox02.btc.BTCScriptConfigWithKeypath(
                 script_config=bitbox02.btc.BTCScriptConfig(
                     multisig=bitbox02.btc.BTCScriptConfig.Multisig(
                         threshold=threshold,
-                        xpubs=[util.parse_xpub(base58.b58encode_check(xpub).decode()) for xpub in xpubs],
+                        xpubs=[util.parse_xpub(encode_check(xpub)) for xpub in xpubs],
                         our_xpub_index=our_xpub_index,
                         script_type=script_type,
                     )
                 ),
                 keypath=our_account_keypath,
             ),
         )
```

### Comparing `hwi-2.2.1/hwilib/devices/ckcc/client.py` & `hwi-2.3.0/hwilib/devices/ckcc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,26 +244,14 @@
         self.master_xpub = str(xpub, 'ascii')
         self.master_fingerprint = fingerprint
 
         #print('sess key = %s' % b2a_hex(self.session_key))
         self.aes_setup(self.session_key)
 
     def mitm_verify(self, sig, expected_xpub):
-        # First try with Pycoin
-        try:
-            from pycoin.key.BIP32Node import BIP32Node
-            from pycoin.contrib.msg_signing import verify_message
-            from pycoin.encoding  import from_bytes_32
-            from base64 import b64encode
-
-            mk = BIP32Node.from_wallet_key(expected_xpub)
-            return verify_message(mk, b64encode(sig), msg_hash=from_bytes_32(self.session_key))
-        except ImportError:
-            pass
-
         # If Pycoin is not available, do it using ecdsa
         from ecdsa import BadSignatureError, SECP256k1, VerifyingKey
         # of the returned (pubkey, chaincode) tuple, chaincode is not used
         pubkey, _ = decode_xpub(expected_xpub)
         vk = VerifyingKey.from_string(get_pubkey_string(pubkey), curve=SECP256k1)
         try:
             ok = vk.verify_digest(sig[1:], self.session_key)
```

### Comparing `hwi-2.2.1/hwilib/devices/ckcc/constants.py` & `hwi-2.3.0/hwilib/devices/ckcc/constants.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ckcc/protocol.py` & `hwi-2.3.0/hwilib/devices/ckcc/protocol.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ckcc/sigheader.py` & `hwi-2.3.0/hwilib/devices/ckcc/sigheader.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ckcc/utils.py` & `hwi-2.3.0/hwilib/devices/ckcc/utils.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/coldcard.py` & `hwi-2.3.0/hwilib/devices/coldcard.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/digitalbitbox.py` & `hwi-2.3.0/hwilib/devices/digitalbitbox.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/jade.py` & `hwi-2.3.0/hwilib/devices/jade.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 import logging
 import semver
 import os
 
 # The test emulator port
 SIMULATOR_PATH = 'tcp:127.0.0.1:30121'
 
-JADE_DEVICE_IDS = [(0x10c4, 0xea60), (0x1a86, 0x55d4)]
+JADE_DEVICE_IDS = [(0x10c4, 0xea60), (0x1a86, 0x55d4), (0x0403, 0x6001), (0x1a86, 0x7523)]
 HAS_NETWORKING = hasattr(jade, '_http_request')
 
 py_enumerate = enumerate # To use the enumerate built-in, since the name is overridden below
 
 def jade_exception(f: Callable[..., Any]) -> Any:
     @wraps(f)
     def func(*args: Any, **kwargs: Any) -> Any:
```

### Comparing `hwi-2.2.1/hwilib/devices/jadepy/jade.py` & `hwi-2.3.0/hwilib/devices/jadepy/jade.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,14 @@
 from .jade_serial import JadeSerialImpl
 from .jade_tcp import JadeTCPImpl
 
 # 'jade' logger
 logger = logging.getLogger('jade')
 device_logger = logging.getLogger('jade-device')
 
-# BLE comms backend is optional
-# It relies on the BLE dependencies being available
-try:
-    from .jade_ble import JadeBleImpl
-except ImportError as e:
-    logger.warn(e)
-    logger.warn('BLE scanning/connectivity will not be available')
-
 
 # Default serial connection
 DEFAULT_SERIAL_DEVICE = '/dev/ttyUSB0'
 DEFAULT_BAUD_RATE = 115200
 DEFAULT_SERIAL_TIMEOUT = 120
 
 # Default BLE connection
```

### Comparing `hwi-2.2.1/hwilib/devices/jadepy/jade_error.py` & `hwi-2.3.0/hwilib/devices/jadepy/jade_error.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/jadepy/jade_serial.py` & `hwi-2.3.0/hwilib/devices/jadepy/jade_serial.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/jadepy/jade_tcp.py` & `hwi-2.3.0/hwilib/devices/jadepy/jade_tcp.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/keepkey.py` & `hwi-2.3.0/hwilib/devices/keepkey.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger.py` & `hwi-2.3.0/hwilib/devices/ledger.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/README.md` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/README.md`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/__init__.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/bitcoinTransaction.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/bitcoinTransaction.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/bitcoinVarint.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/bitcoinVarint.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/btchip.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/btchip.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/btchipException.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/btchipException.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/btchipHelpers.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/btchipHelpers.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/btchipUtils.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/btchipUtils.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/btchip/ledgerWrapper.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/btchip/ledgerWrapper.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/client.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/client.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/client_base.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/client_base.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/client_command.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/client_command.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/client_legacy.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/client_legacy.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/command_builder.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/command_builder.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/errors.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/errors.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/exception/__init__.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/exception/device_exception.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/device_exception.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/exception/errors.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/exception/errors.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/README.md` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/README.md`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/comm.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/comm.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/hid_device.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/hid_device.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/tcp_client.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/tcp_client.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/ledgercomm/transport.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/ledgercomm/transport.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/merkle.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/merkle.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/ledger_bitcoin/wallet.py` & `hwi-2.3.0/hwilib/devices/ledger_bitcoin/wallet.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezor.py` & `hwi-2.3.0/hwilib/devices/trezor.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/README.md` & `hwi-2.3.0/hwilib/devices/trezorlib/README.md`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/__init__.py` & `hwi-2.3.0/hwilib/devices/trezorlib/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/btc.py` & `hwi-2.3.0/hwilib/devices/trezorlib/btc.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/client.py` & `hwi-2.3.0/hwilib/devices/trezorlib/client.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/debuglink.py` & `hwi-2.3.0/hwilib/devices/trezorlib/debuglink.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/device.py` & `hwi-2.3.0/hwilib/devices/trezorlib/device.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/exceptions.py` & `hwi-2.3.0/hwilib/devices/trezorlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/firmware.py` & `hwi-2.3.0/hwilib/devices/trezorlib/firmware.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/log.py` & `hwi-2.3.0/hwilib/devices/trezorlib/log.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/mapping.py` & `hwi-2.3.0/hwilib/devices/trezorlib/mapping.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/messages.py` & `hwi-2.3.0/hwilib/devices/trezorlib/messages.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/models.py` & `hwi-2.3.0/hwilib/devices/trezorlib/models.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/protobuf.py` & `hwi-2.3.0/hwilib/devices/trezorlib/protobuf.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/tools.py` & `hwi-2.3.0/hwilib/devices/trezorlib/tools.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/transport/__init__.py` & `hwi-2.3.0/hwilib/devices/trezorlib/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/transport/hid.py` & `hwi-2.3.0/hwilib/devices/trezorlib/transport/hid.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/transport/protocol.py` & `hwi-2.3.0/hwilib/devices/trezorlib/transport/protocol.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/transport/udp.py` & `hwi-2.3.0/hwilib/devices/trezorlib/transport/udp.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/devices/trezorlib/transport/webusb.py` & `hwi-2.3.0/hwilib/devices/trezorlib/transport/webusb.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/errors.py` & `hwi-2.3.0/hwilib/errors.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/hwwclient.py` & `hwi-2.3.0/hwilib/hwwclient.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/key.py` & `hwi-2.3.0/hwilib/key.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/psbt.py` & `hwi-2.3.0/hwilib/psbt.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/tx.py` & `hwi-2.3.0/hwilib/tx.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/udev/20-hw1.rules` & `hwi-2.3.0/hwilib/udev/20-hw1.rules`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/udev/51-trezor.rules` & `hwi-2.3.0/hwilib/udev/51-trezor.rules`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/udev/51-usb-keepkey.rules` & `hwi-2.3.0/hwilib/udev/51-usb-keepkey.rules`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/udev/README.md` & `hwi-2.3.0/hwilib/udev/README.md`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/udevinstaller.py` & `hwi-2.3.0/hwilib/udevinstaller.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/bitbox02pairing.ui` & `hwi-2.3.0/hwilib/ui/bitbox02pairing.ui`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/displayaddressdialog.ui` & `hwi-2.3.0/hwilib/ui/displayaddressdialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/getkeypooloptionsdialog.ui` & `hwi-2.3.0/hwilib/ui/getkeypooloptionsdialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/getxpubdialog.ui` & `hwi-2.3.0/hwilib/ui/getxpubdialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/mainwindow.ui` & `hwi-2.3.0/hwilib/ui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/sendpindialog.ui` & `hwi-2.3.0/hwilib/ui/sendpindialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/setpassphrasedialog.ui` & `hwi-2.3.0/hwilib/ui/setpassphrasedialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/signmessagedialog.ui` & `hwi-2.3.0/hwilib/ui/signmessagedialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/signpsbtdialog.ui` & `hwi-2.3.0/hwilib/ui/signpsbtdialog.ui`

 * *Files 7% similar despite different names*

#### Comparing `hwi-2.2.1/hwilib/ui/signpsbtdialog.ui` & `hwi-2.3.0/hwilib/ui/signpsbtdialog.ui`

```diff
@@ -51,28 +51,58 @@
               </property>
               <property name="wordWrap">
                 <bool>true</bool>
               </property>
             </widget>
           </item>
           <item>
+            <widget class="QToolButton" name="import_toolbutton">
+              <property name="text">
+                <string>Import PSBT</string>
+              </property>
+              <property name="popupMode">
+                <enum>QToolButton::InstantPopup</enum>
+              </property>
+            </widget>
+          </item>
+          <item>
             <spacer name="verticalSpacer">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
               <property name="sizeHint" stdset="0">
                 <size>
                   <width>20</width>
                   <height>40</height>
                 </size>
               </property>
             </spacer>
           </item>
         </layout>
       </item>
+      <item row="1" column="2">
+        <widget class="QPlainTextEdit" name="psbt_in_textedit">
+          <property name="minimumSize">
+            <size>
+              <width>300</width>
+              <height>120</height>
+            </size>
+          </property>
+        </widget>
+      </item>
+      <item row="4" column="2">
+        <widget class="QDialogButtonBox" name="buttonBox">
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+          <property name="standardButtons">
+            <set>QDialogButtonBox::Close</set>
+          </property>
+        </widget>
+      </item>
       <item row="3" column="0">
         <layout class="QVBoxLayout" name="verticalLayout">
           <item>
             <spacer name="verticalSpacer_3">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
@@ -91,38 +121,38 @@
               </property>
               <property name="wordWrap">
                 <bool>true</bool>
               </property>
             </widget>
           </item>
           <item>
+            <widget class="QToolButton" name="export_toolbutton">
+              <property name="text">
+                <string>Export PSBT</string>
+              </property>
+              <property name="popupMode">
+                <enum>QToolButton::InstantPopup</enum>
+              </property>
+            </widget>
+          </item>
+          <item>
             <spacer name="verticalSpacer_4">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
               <property name="sizeHint" stdset="0">
                 <size>
                   <width>20</width>
                   <height>40</height>
                 </size>
               </property>
             </spacer>
           </item>
         </layout>
       </item>
-      <item row="1" column="2">
-        <widget class="QPlainTextEdit" name="psbt_in_textedit">
-          <property name="minimumSize">
-            <size>
-              <width>300</width>
-              <height>120</height>
-            </size>
-          </property>
-        </widget>
-      </item>
       <item row="3" column="2">
         <widget class="QPlainTextEdit" name="psbt_out_textedit">
           <property name="minimumSize">
             <size>
               <width>300</width>
               <height>120</height>
             </size>
@@ -171,24 +201,14 @@
                   <height>20</height>
                 </size>
               </property>
             </spacer>
           </item>
         </layout>
       </item>
-      <item row="4" column="2">
-        <widget class="QDialogButtonBox" name="buttonBox">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="standardButtons">
-            <set>QDialogButtonBox::Close</set>
-          </property>
-        </widget>
-      </item>
     </layout>
   </widget>
   <resources/>
   <connections>
     <connection>
       <sender>buttonBox</sender>
       <signal>accepted()</signal>
```

### Comparing `hwi-2.2.1/hwilib/ui/ui_bitbox02pairing.py` & `hwi-2.3.0/hwilib/ui/ui_bitbox02pairing.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/ui_displayaddressdialog.py` & `hwi-2.3.0/hwilib/ui/ui_displayaddressdialog.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/ui_getkeypooloptionsdialog.py` & `hwi-2.3.0/hwilib/ui/ui_getkeypooloptionsdialog.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/ui_getxpubdialog.py` & `hwi-2.3.0/hwilib/ui/ui_getxpubdialog.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/ui_mainwindow.py` & `hwi-2.3.0/hwilib/ui/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/ui_sendpindialog.py` & `hwi-2.3.0/hwilib/ui/ui_sendpindialog.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/ui_setpassphrasedialog.py` & `hwi-2.3.0/hwilib/ui/ui_setpassphrasedialog.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/ui_signmessagedialog.py` & `hwi-2.3.0/hwilib/ui/ui_signmessagedialog.py`

 * *Files identical despite different names*

### Comparing `hwi-2.2.1/hwilib/ui/ui_signpsbtdialog.py` & `hwi-2.3.0/hwilib/ui/ui_signpsbtdialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,46 +30,65 @@
 
         self.label = QLabel(SignPSBTDialog)
         self.label.setObjectName(u"label")
         self.label.setWordWrap(True)
 
         self.verticalLayout_2.addWidget(self.label)
 
+        self.import_toolbutton = QToolButton(SignPSBTDialog)
+        self.import_toolbutton.setObjectName(u"import_toolbutton")
+        self.import_toolbutton.setPopupMode(QToolButton.InstantPopup)
+
+        self.verticalLayout_2.addWidget(self.import_toolbutton)
+
         self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_2.addItem(self.verticalSpacer)
 
 
         self.gridLayout.addLayout(self.verticalLayout_2, 1, 0, 1, 1)
 
+        self.psbt_in_textedit = QPlainTextEdit(SignPSBTDialog)
+        self.psbt_in_textedit.setObjectName(u"psbt_in_textedit")
+        self.psbt_in_textedit.setMinimumSize(QSize(300, 120))
+
+        self.gridLayout.addWidget(self.psbt_in_textedit, 1, 2, 1, 1)
+
+        self.buttonBox = QDialogButtonBox(SignPSBTDialog)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Close)
+
+        self.gridLayout.addWidget(self.buttonBox, 4, 2, 1, 1)
+
         self.verticalLayout = QVBoxLayout()
         self.verticalLayout.setObjectName(u"verticalLayout")
         self.verticalSpacer_3 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout.addItem(self.verticalSpacer_3)
 
         self.label_2 = QLabel(SignPSBTDialog)
         self.label_2.setObjectName(u"label_2")
         self.label_2.setWordWrap(True)
 
         self.verticalLayout.addWidget(self.label_2)
 
+        self.export_toolbutton = QToolButton(SignPSBTDialog)
+        self.export_toolbutton.setObjectName(u"export_toolbutton")
+        self.export_toolbutton.setPopupMode(QToolButton.InstantPopup)
+
+        self.verticalLayout.addWidget(self.export_toolbutton)
+
         self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout.addItem(self.verticalSpacer_4)
 
 
         self.gridLayout.addLayout(self.verticalLayout, 3, 0, 1, 1)
 
-        self.psbt_in_textedit = QPlainTextEdit(SignPSBTDialog)
-        self.psbt_in_textedit.setObjectName(u"psbt_in_textedit")
-        self.psbt_in_textedit.setMinimumSize(QSize(300, 120))
-
-        self.gridLayout.addWidget(self.psbt_in_textedit, 1, 2, 1, 1)
-
         self.psbt_out_textedit = QPlainTextEdit(SignPSBTDialog)
         self.psbt_out_textedit.setObjectName(u"psbt_out_textedit")
         self.psbt_out_textedit.setMinimumSize(QSize(300, 120))
         self.psbt_out_textedit.setTextInteractionFlags(Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
 
         self.gridLayout.addWidget(self.psbt_out_textedit, 3, 2, 1, 1)
 
@@ -88,32 +107,27 @@
         self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout.addItem(self.horizontalSpacer_2)
 
 
         self.gridLayout.addLayout(self.horizontalLayout, 2, 2, 1, 1)
 
-        self.buttonBox = QDialogButtonBox(SignPSBTDialog)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Close)
-
-        self.gridLayout.addWidget(self.buttonBox, 4, 2, 1, 1)
-
 
         self.retranslateUi(SignPSBTDialog)
         self.buttonBox.accepted.connect(SignPSBTDialog.accept)
         self.buttonBox.rejected.connect(SignPSBTDialog.reject)
 
         self.sign_psbt_button.setDefault(True)
 
 
         QMetaObject.connectSlotsByName(SignPSBTDialog)
     # setupUi
 
     def retranslateUi(self, SignPSBTDialog):
         SignPSBTDialog.setWindowTitle(QCoreApplication.translate("SignPSBTDialog", u"Dialog", None))
         self.label.setText(QCoreApplication.translate("SignPSBTDialog", u"PSBT To Sign", None))
+        self.import_toolbutton.setText(QCoreApplication.translate("SignPSBTDialog", u"Import PSBT", None))
         self.label_2.setText(QCoreApplication.translate("SignPSBTDialog", u"PSBT Result", None))
+        self.export_toolbutton.setText(QCoreApplication.translate("SignPSBTDialog", u"Export PSBT", None))
         self.sign_psbt_button.setText(QCoreApplication.translate("SignPSBTDialog", u"Sign PSBT", None))
     # retranslateUi
```

### Comparing `hwi-2.2.1/pyproject.toml` & `hwi-2.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hwi"
-version = "2.2.1"
+version = "2.3.0"
 description = "A library for working with Bitcoin hardware wallets"
 authors = ["Andrew Chow <andrew@achow101.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bitcoin-core/HWI"
 homepage = "https://github.com/bitcoin-core/HWI"
 exclude = ["docs/", "test/"]
@@ -13,25 +13,27 @@
     { include = "hwi.py" },
     { include = "hwi-qt.py" },
     { include = "hwilib" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7,<3.12"
-hidapi = "~0"
+hidapi = ">=0.14.0"
 ecdsa = "~0"
 pyaes = "^1.6"
 mnemonic = "~0"
 typing-extensions = "^4.4"
 libusb1 = ">=1.7,<3"
 pyside2 = { version = "^5.14.0", optional = true, python = "<3.10" }
-bitbox02 = ">=6.1.0,<7.0.0"
 cbor = "^1.0.0"
 pyserial = "^3.5"
 dataclasses = {version = "^0.8", python = ">=3.6,<3.7"}
+semver = "^3.0.1"
+noiseprotocol = "^0.3.1"
+protobuf = "^4.23.3"
 
 [tool.poetry.extras]
 qt = ["pyside2"]
 
 [tool.poetry.dev-dependencies]
 pyinstaller = "^5.3"
 autopep8 = "~1"
@@ -44,7 +46,10 @@
 [tool.poetry.scripts]
 hwi = 'hwilib._cli:main'
 hwi-qt = 'hwilib._gui:main'
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
+
+[tool.poetry.build]
+generate-setup-file = true
```

### Comparing `hwi-2.2.1/setup.py` & `hwi-2.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['hwilib',
  'hwilib.devices',
+ 'hwilib.devices.bitbox02_lib',
+ 'hwilib.devices.bitbox02_lib.bitbox02',
+ 'hwilib.devices.bitbox02_lib.communication',
+ 'hwilib.devices.bitbox02_lib.communication.generated',
+ 'hwilib.devices.bitbox02_lib.communication.u2fhid',
  'hwilib.devices.ckcc',
  'hwilib.devices.jadepy',
  'hwilib.devices.ledger_bitcoin',
  'hwilib.devices.ledger_bitcoin.btchip',
  'hwilib.devices.ledger_bitcoin.exception',
  'hwilib.devices.ledger_bitcoin.ledgercomm',
  'hwilib.devices.ledger_bitcoin.ledgercomm.interfaces',
@@ -17,34 +22,36 @@
 
 package_data = \
 {'': ['*'], 'hwilib': ['udev/*']}
 
 modules = \
 ['hwi', 'hwi-qt']
 install_requires = \
-['bitbox02>=6.1.0,<7.0.0',
- 'cbor>=1.0.0,<2.0.0',
+['cbor>=1.0.0,<2.0.0',
  'ecdsa>=0,<1',
- 'hidapi>=0,<1',
+ 'hidapi>=0.14.0',
  'libusb1>=1.7,<3',
  'mnemonic>=0,<1',
+ 'noiseprotocol>=0.3.1,<0.4.0',
+ 'protobuf>=4.23.3,<5.0.0',
  'pyaes>=1.6,<2.0',
  'pyserial>=3.5,<4.0',
+ 'semver>=3.0.1,<4.0.0',
  'typing-extensions>=4.4,<5.0']
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.8,<0.9'],
  'qt:python_version < "3.10"': ['pyside2>=5.14.0,<6.0.0']}
 
 entry_points = \
 {'console_scripts': ['hwi = hwilib._cli:main', 'hwi-qt = hwilib._gui:main']}
 
 setup_kwargs = {
     'name': 'hwi',
-    'version': '2.2.1',
+    'version': '2.3.0',
     'description': 'A library for working with Bitcoin hardware wallets',
     'long_description': "# Bitcoin Hardware Wallet Interface\n\n[![Build Status](https://api.cirrus-ci.com/github/bitcoin-core/HWI.svg)](https://cirrus-ci.com/github/bitcoin-core/HWI)\n[![Documentation Status](https://readthedocs.org/projects/hwi/badge/?version=latest)](https://hwi.readthedocs.io/en/latest/?badge=latest)\n\nThe Bitcoin Hardware Wallet Interface is a Python library and command line tool for interacting with hardware wallets.\nIt provides a standard way for software to work with hardware wallets without needing to implement device specific drivers.\nPython software can use the provided library (`hwilib`). Software in other languages can execute the `hwi` tool.\n\nCaveat emptor: Inclusion of a specific hardware wallet vendor does not imply any endorsement of quality or security.\n\n## Prerequisites\n\nPython 3 is required. The libraries and [udev rules](hwilib/udev/README.md) for each device must also be installed. Some libraries will need to be installed\n\nFor Ubuntu/Debian:\n```\nsudo apt install libusb-1.0-0-dev libudev-dev python3-dev\n```\n\nFor Centos:\n```\nsudo yum -y install python3-devel libusbx-devel systemd-devel\n```\n\nFor macOS:\n```\nbrew install libusb\n```\n\n## Install\n\n```\ngit clone https://github.com/bitcoin-core/HWI.git\ncd HWI\npoetry install # or 'pip3 install .' or 'python3 setup.py install'\n```\n\nThis project uses the [Poetry](https://github.com/sdispater/poetry) dependency manager. HWI and its dependencies can be installed via poetry by executing the following in the root source directory:\n\n```\npoetry install\n```\n\nPip can also be used to automatically install HWI and its dependencies using the `setup.py` file (which is usually in sync with `pyproject.toml`):\n\n```\npip3 install .\n```\n\nThe `setup.py` file can be used to install HWI and its dependencies so long as `setuptools` is also installed:\n\n```\npip3 install -U setuptools\npython3 setup.py install\n```\n\n## Dependencies\n\nSee `pyproject.toml` for all dependencies. Dependencies under `[tool.poetry.dependencies]` are user dependencies, and `[tool.poetry.dev-dependencies]` for development based dependencies. These dependencies will be installed with any of the three above installation methods.\n\n## Usage\n\nTo use, first enumerate all devices and find the one that you want to use with\n\n```\n./hwi.py enumerate\n```\n\nOnce the device type and device path is known, issue commands to it like so:\n\n```\n./hwi.py -t <type> -d <path> <command> <command args>\n```\n\nAll output will be in JSON form and sent to `stdout`.\nAdditional information or prompts will be sent to `stderr` and will not necessarily be in JSON.\nThis additional information is for debugging purposes.\n\nTo see a complete list of available commands and global parameters, run\n`./hwi.py --help`.  To see options specific to a particular command,\npass the `--help` parameter after the command name; for example:\n\n```\n./hwi.py getdescriptors --help\n```\n\n## Documentation\n\nDocumentation for HWI can be found on [readthedocs.io](https://hwi.readthedocs.io/).\n\n### Device Support\n\nFor documentation on devices supported and how they are supported, please check the [device support page](https://hwi.readthedocs.io/en/latest/devices/index.html#support-matrix)\n\n### Using with Bitcoin Core\n\nSee [Using Bitcoin Core with Hardware Wallets](https://hwi.readthedocs.io/en/latest/examples/bitcoin-core-usage.html).\n\n## License\n\nThis project is available under the MIT License, Copyright Andrew Chow.\n",
     'author': 'Andrew Chow',
     'author_email': 'andrew@achow101.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bitcoin-core/HWI',
```

### Comparing `hwi-2.2.1/PKG-INFO` & `hwi-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: hwi
-Version: 2.2.1
+Version: 2.3.0
 Summary: A library for working with Bitcoin hardware wallets
 Home-page: https://github.com/bitcoin-core/HWI
 License: MIT
 Author: Andrew Chow
 Author-email: andrew@achow101.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: qt
-Requires-Dist: bitbox02 (>=6.1.0,<7.0.0)
 Requires-Dist: cbor (>=1.0.0,<2.0.0)
 Requires-Dist: dataclasses (>=0.8,<0.9) ; python_version >= "3.6" and python_version < "3.7"
 Requires-Dist: ecdsa (>=0,<1)
-Requires-Dist: hidapi (>=0,<1)
+Requires-Dist: hidapi (>=0.14.0)
 Requires-Dist: libusb1 (>=1.7,<3)
 Requires-Dist: mnemonic (>=0,<1)
+Requires-Dist: noiseprotocol (>=0.3.1,<0.4.0)
+Requires-Dist: protobuf (>=4.23.3,<5.0.0)
 Requires-Dist: pyaes (>=1.6,<2.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
 Requires-Dist: pyside2 (>=5.14.0,<6.0.0) ; (python_version < "3.10") and (extra == "qt")
+Requires-Dist: semver (>=3.0.1,<4.0.0)
 Requires-Dist: typing-extensions (>=4.4,<5.0)
 Project-URL: Repository, https://github.com/bitcoin-core/HWI
 Description-Content-Type: text/markdown
 
 # Bitcoin Hardware Wallet Interface
 
 [![Build Status](https://api.cirrus-ci.com/github/bitcoin-core/HWI.svg)](https://cirrus-ci.com/github/bitcoin-core/HWI)
```

