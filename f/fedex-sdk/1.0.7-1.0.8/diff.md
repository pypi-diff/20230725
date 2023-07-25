# Comparing `tmp/fedex-sdk-1.0.7.tar.gz` & `tmp/fedex-sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedex-sdk-1.0.7.tar", last modified: Mon Jul 24 10:34:58 2023, max compression
+gzip compressed data, was "fedex-sdk-1.0.8.tar", last modified: Tue Jul 25 06:27:54 2023, max compression
```

## Comparing `fedex-sdk-1.0.7.tar` & `fedex-sdk-1.0.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 10:34:58.734795 fedex-sdk-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-24 10:34:58.595795 fedex-sdk-1.0.7/FedexSDK/
--rw-rw-rw-   0        0        0     4086 2023-07-24 07:14:21.000000 fedex-sdk-1.0.7/FedexSDK/FedExSDK.py
--rw-rw-rw-   0        0        0       66 2023-07-24 10:34:51.000000 fedex-sdk-1.0.7/FedexSDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:34:58.614796 fedex-sdk-1.0.7/FedexSDK/models/
--rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-1.0.7/FedexSDK/models/AccountNumber.py
--rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-1.0.7/FedexSDK/models/Address.py
--rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-1.0.7/FedexSDK/models/Contact.py
--rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-1.0.7/FedexSDK/models/Recipient.py
--rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-1.0.7/FedexSDK/models/Request.py
--rw-rw-rw-   0        0        0     6760 2023-07-24 09:23:13.000000 fedex-sdk-1.0.7/FedexSDK/models/RequestedShipment.py
--rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-1.0.7/FedexSDK/models/Shipper.py
--rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-1.0.7/FedexSDK/models/SoldTo.py
--rw-rw-rw-   0        0        0      683 2023-07-24 08:42:54.000000 fedex-sdk-1.0.7/FedexSDK/models/Tin.py
--rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-1.0.7/FedexSDK/models/TotalDeclaredValue.py
--rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-1.0.7/FedexSDK/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:34:58.646798 fedex-sdk-1.0.7/FedexSDK/models/label/
--rw-rw-rw-   0        0        0      309 2023-07-22 12:20:00.000000 fedex-sdk-1.0.7/FedexSDK/models/label/Barcode.py
--rw-rw-rw-   0        0        0      290 2023-07-22 12:39:45.000000 fedex-sdk-1.0.7/FedexSDK/models/label/CompletedEtdDetail.py
--rw-rw-rw-   0        0        0      383 2023-07-24 07:25:50.000000 fedex-sdk-1.0.7/FedexSDK/models/label/CompletedPackageDetail.py
--rw-rw-rw-   0        0        0      881 2023-07-22 12:41:04.000000 fedex-sdk-1.0.7/FedexSDK/models/label/CompletedShipmentDetail.py
--rw-rw-rw-   0        0        0      266 2023-07-22 13:26:59.000000 fedex-sdk-1.0.7/FedexSDK/models/label/DocumentRequirements.py
--rw-rw-rw-   0        0        0      231 2023-07-22 12:38:12.000000 fedex-sdk-1.0.7/FedexSDK/models/label/GenerationDetail.py
--rw-rw-rw-   0        0        0      149 2023-07-22 12:37:18.000000 fedex-sdk-1.0.7/FedexSDK/models/label/MasterTrackingId.py
--rw-rw-rw-   0        0        0      110 2023-07-22 12:34:22.000000 fedex-sdk-1.0.7/FedexSDK/models/label/Name.py
--rw-rw-rw-   0        0        0     1037 2023-07-22 12:42:38.000000 fedex-sdk-1.0.7/FedexSDK/models/label/OperationalDetail.py
--rw-rw-rw-   0        0        0      107 2023-07-22 12:37:39.000000 fedex-sdk-1.0.7/FedexSDK/models/label/OperationalInsturaction.py
--rw-rw-rw-   0        0        0      154 2023-07-22 12:14:51.000000 fedex-sdk-1.0.7/FedexSDK/models/label/PackageDocument.py
--rw-rw-rw-   0        0        0      109 2023-07-22 12:12:51.000000 fedex-sdk-1.0.7/FedexSDK/models/label/Part.py
--rw-rw-rw-   0        0        0      450 2023-07-22 12:15:21.000000 fedex-sdk-1.0.7/FedexSDK/models/label/PieceResponse.py
--rw-rw-rw-   0        0        0      737 2023-07-22 13:20:13.000000 fedex-sdk-1.0.7/FedexSDK/models/label/Response.py
--rw-rw-rw-   0        0        0      308 2023-07-22 13:26:49.000000 fedex-sdk-1.0.7/FedexSDK/models/label/ServiceDescription.py
--rw-rw-rw-   0        0        0      523 2023-07-22 12:14:35.000000 fedex-sdk-1.0.7/FedexSDK/models/label/ShipmentDocument.py
--rw-rw-rw-   0        0        0      129 2023-07-22 12:19:27.000000 fedex-sdk-1.0.7/FedexSDK/models/label/TrackingId.py
--rw-rw-rw-   0        0        0      131 2023-07-22 12:39:11.000000 fedex-sdk-1.0.7/FedexSDK/models/label/UploadDocumentReferenceDetail.py
--rw-rw-rw-   0        0        0        0 2023-07-24 07:14:11.000000 fedex-sdk-1.0.7/FedexSDK/models/label/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:34:58.684796 fedex-sdk-1.0.7/FedexSDK/models/tracking/
--rw-rw-rw-   0        0        0      127 2023-07-22 07:14:07.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/AdditionalTrackingInfo.py
--rw-rw-rw-   0        0        0      214 2023-07-22 07:04:34.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/Address.py
--rw-rw-rw-   0        0        0       97 2023-07-22 08:23:17.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/DateAndTime.py
--rw-rw-rw-   0        0        0      119 2023-07-22 08:29:51.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/DelayDetail.py
--rw-rw-rw-   0        0        0      328 2023-07-22 09:24:39.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/DeliveryDetails.py
--rw-rw-rw-   0        0        0      124 2023-07-22 08:21:44.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/DeliveryOptionEligiblityDetail.py
--rw-rw-rw-   0        0        0      385 2023-07-22 07:04:54.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/Destination.py
--rw-rw-rw-   0        0        0      333 2023-07-22 09:23:39.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/LatestStatusDetail.py
--rw-rw-rw-   0        0        0      131 2023-07-22 07:04:47.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/LocationContactAndAddress.py
--rw-rw-rw-   0        0        0      213 2023-07-22 07:05:30.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/OriginLocation.py
--rw-rw-rw-   0        0        0      387 2023-07-22 08:28:05.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/PackageDetails.py
--rw-rw-rw-   0        0        0      183 2023-07-22 08:17:51.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/RecipientInformation.py
--rw-rw-rw-   0        0        0      481 2023-07-22 06:57:13.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/ScanEvent.py
--rw-rw-rw-   0        0        0      355 2023-07-22 08:29:12.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/ScanLocation.py
--rw-rw-rw-   0        0        0      105 2023-07-22 08:22:58.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/ServiceCommitMessage.py
--rw-rw-rw-   0        0        0      131 2023-07-22 07:02:59.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/ServiceDetail.py
--rw-rw-rw-   0        0        0      199 2023-07-22 07:01:06.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/ShipmentDetails.py
--rw-rw-rw-   0        0        0      181 2023-07-22 08:27:55.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/ShipperInformation.py
--rw-rw-rw-   0        0        0      126 2023-07-22 08:22:37.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/SpecialHandling.py
--rw-rw-rw-   0        0        0     2150 2023-07-22 09:25:14.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/TrackResult.py
--rw-rw-rw-   0        0        0      150 2023-07-22 07:13:21.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/TrackingNumberInfo.py
--rw-rw-rw-   0        0        0      339 2023-07-24 10:34:46.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/WeightAndDimensions.py
--rw-rw-rw-   0        0        0      271 2023-07-24 10:34:19.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/Window.py
--rw-rw-rw-   0        0        0        0 2023-07-22 06:48:10.000000 fedex-sdk-1.0.7/FedexSDK/models/tracking/__init__.py
--rw-rw-rw-   0        0        0      326 2023-07-24 10:34:58.733803 fedex-sdk-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 10:34:58.731799 fedex-sdk-1.0.7/fedex_sdk.egg-info/
--rw-rw-rw-   0        0        0      326 2023-07-24 10:34:57.000000 fedex-sdk-1.0.7/fedex_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2343 2023-07-24 10:34:58.000000 fedex-sdk-1.0.7/fedex_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 10:34:58.000000 fedex-sdk-1.0.7/fedex_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 10:34:58.000000 fedex-sdk-1.0.7/fedex_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 10:34:58.735796 fedex-sdk-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:27:54.305587 fedex-sdk-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:27:54.013689 fedex-sdk-1.0.8/FedexSDK/
+-rw-rw-rw-   0        0        0     4086 2023-07-24 07:14:21.000000 fedex-sdk-1.0.8/FedexSDK/FedExSDK.py
+-rw-rw-rw-   0        0        0       66 2023-07-25 06:27:16.000000 fedex-sdk-1.0.8/FedexSDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:27:54.193587 fedex-sdk-1.0.8/FedexSDK/models/
+-rw-rw-rw-   0        0        0       79 2023-07-20 14:07:03.000000 fedex-sdk-1.0.8/FedexSDK/models/AccountNumber.py
+-rw-rw-rw-   0        0        0     1400 2023-07-20 14:15:22.000000 fedex-sdk-1.0.8/FedexSDK/models/Address.py
+-rw-rw-rw-   0        0        0     2163 2023-07-20 13:11:54.000000 fedex-sdk-1.0.8/FedexSDK/models/Contact.py
+-rw-rw-rw-   0        0        0      297 2023-07-20 14:00:52.000000 fedex-sdk-1.0.8/FedexSDK/models/Recipient.py
+-rw-rw-rw-   0        0        0     1345 2023-07-20 14:16:51.000000 fedex-sdk-1.0.8/FedexSDK/models/Request.py
+-rw-rw-rw-   0        0        0     6760 2023-07-24 09:23:13.000000 fedex-sdk-1.0.8/FedexSDK/models/RequestedShipment.py
+-rw-rw-rw-   0        0        0      263 2023-07-20 13:49:03.000000 fedex-sdk-1.0.8/FedexSDK/models/Shipper.py
+-rw-rw-rw-   0        0        0      316 2023-07-20 14:00:05.000000 fedex-sdk-1.0.8/FedexSDK/models/SoldTo.py
+-rw-rw-rw-   0        0        0      683 2023-07-24 08:42:54.000000 fedex-sdk-1.0.8/FedexSDK/models/Tin.py
+-rw-rw-rw-   0        0        0      300 2023-07-20 13:07:32.000000 fedex-sdk-1.0.8/FedexSDK/models/TotalDeclaredValue.py
+-rw-rw-rw-   0        0        0      969 2023-07-21 08:43:43.000000 fedex-sdk-1.0.8/FedexSDK/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:27:54.249587 fedex-sdk-1.0.8/FedexSDK/models/label/
+-rw-rw-rw-   0        0        0      309 2023-07-22 12:20:00.000000 fedex-sdk-1.0.8/FedexSDK/models/label/Barcode.py
+-rw-rw-rw-   0        0        0      290 2023-07-22 12:39:45.000000 fedex-sdk-1.0.8/FedexSDK/models/label/CompletedEtdDetail.py
+-rw-rw-rw-   0        0        0      383 2023-07-24 07:25:50.000000 fedex-sdk-1.0.8/FedexSDK/models/label/CompletedPackageDetail.py
+-rw-rw-rw-   0        0        0      881 2023-07-22 12:41:04.000000 fedex-sdk-1.0.8/FedexSDK/models/label/CompletedShipmentDetail.py
+-rw-rw-rw-   0        0        0      266 2023-07-22 13:26:59.000000 fedex-sdk-1.0.8/FedexSDK/models/label/DocumentRequirements.py
+-rw-rw-rw-   0        0        0      231 2023-07-22 12:38:12.000000 fedex-sdk-1.0.8/FedexSDK/models/label/GenerationDetail.py
+-rw-rw-rw-   0        0        0      149 2023-07-22 12:37:18.000000 fedex-sdk-1.0.8/FedexSDK/models/label/MasterTrackingId.py
+-rw-rw-rw-   0        0        0      110 2023-07-22 12:34:22.000000 fedex-sdk-1.0.8/FedexSDK/models/label/Name.py
+-rw-rw-rw-   0        0        0     1037 2023-07-22 12:42:38.000000 fedex-sdk-1.0.8/FedexSDK/models/label/OperationalDetail.py
+-rw-rw-rw-   0        0        0      107 2023-07-22 12:37:39.000000 fedex-sdk-1.0.8/FedexSDK/models/label/OperationalInsturaction.py
+-rw-rw-rw-   0        0        0      154 2023-07-22 12:14:51.000000 fedex-sdk-1.0.8/FedexSDK/models/label/PackageDocument.py
+-rw-rw-rw-   0        0        0      109 2023-07-22 12:12:51.000000 fedex-sdk-1.0.8/FedexSDK/models/label/Part.py
+-rw-rw-rw-   0        0        0      450 2023-07-22 12:15:21.000000 fedex-sdk-1.0.8/FedexSDK/models/label/PieceResponse.py
+-rw-rw-rw-   0        0        0      737 2023-07-22 13:20:13.000000 fedex-sdk-1.0.8/FedexSDK/models/label/Response.py
+-rw-rw-rw-   0        0        0      308 2023-07-22 13:26:49.000000 fedex-sdk-1.0.8/FedexSDK/models/label/ServiceDescription.py
+-rw-rw-rw-   0        0        0      523 2023-07-22 12:14:35.000000 fedex-sdk-1.0.8/FedexSDK/models/label/ShipmentDocument.py
+-rw-rw-rw-   0        0        0      129 2023-07-22 12:19:27.000000 fedex-sdk-1.0.8/FedexSDK/models/label/TrackingId.py
+-rw-rw-rw-   0        0        0      131 2023-07-22 12:39:11.000000 fedex-sdk-1.0.8/FedexSDK/models/label/UploadDocumentReferenceDetail.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 07:14:11.000000 fedex-sdk-1.0.8/FedexSDK/models/label/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:27:54.292592 fedex-sdk-1.0.8/FedexSDK/models/tracking/
+-rw-rw-rw-   0        0        0      127 2023-07-22 07:14:07.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/AdditionalTrackingInfo.py
+-rw-rw-rw-   0        0        0      214 2023-07-22 07:04:34.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/Address.py
+-rw-rw-rw-   0        0        0       97 2023-07-22 08:23:17.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/DateAndTime.py
+-rw-rw-rw-   0        0        0      119 2023-07-22 08:29:51.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/DelayDetail.py
+-rw-rw-rw-   0        0        0      328 2023-07-22 09:24:39.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/DeliveryDetails.py
+-rw-rw-rw-   0        0        0      124 2023-07-22 08:21:44.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/DeliveryOptionEligiblityDetail.py
+-rw-rw-rw-   0        0        0      424 2023-07-25 06:26:28.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/Destination.py
+-rw-rw-rw-   0        0        0      333 2023-07-22 09:23:39.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/LatestStatusDetail.py
+-rw-rw-rw-   0        0        0      131 2023-07-22 07:04:47.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/LocationContactAndAddress.py
+-rw-rw-rw-   0        0        0      213 2023-07-22 07:05:30.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/OriginLocation.py
+-rw-rw-rw-   0        0        0      387 2023-07-22 08:28:05.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/PackageDetails.py
+-rw-rw-rw-   0        0        0      183 2023-07-22 08:17:51.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/RecipientInformation.py
+-rw-rw-rw-   0        0        0      481 2023-07-22 06:57:13.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/ScanEvent.py
+-rw-rw-rw-   0        0        0      355 2023-07-22 08:29:12.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/ScanLocation.py
+-rw-rw-rw-   0        0        0      105 2023-07-22 08:22:58.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/ServiceCommitMessage.py
+-rw-rw-rw-   0        0        0      131 2023-07-22 07:02:59.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/ServiceDetail.py
+-rw-rw-rw-   0        0        0      199 2023-07-22 07:01:06.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/ShipmentDetails.py
+-rw-rw-rw-   0        0        0      181 2023-07-22 08:27:55.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/ShipperInformation.py
+-rw-rw-rw-   0        0        0      126 2023-07-22 08:22:37.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/SpecialHandling.py
+-rw-rw-rw-   0        0        0     2150 2023-07-22 09:25:14.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/TrackResult.py
+-rw-rw-rw-   0        0        0      150 2023-07-22 07:13:21.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/TrackingNumberInfo.py
+-rw-rw-rw-   0        0        0      339 2023-07-24 10:34:46.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/WeightAndDimensions.py
+-rw-rw-rw-   0        0        0      271 2023-07-24 10:34:19.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/Window.py
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:48:10.000000 fedex-sdk-1.0.8/FedexSDK/models/tracking/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-07-25 06:27:54.304587 fedex-sdk-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 06:27:54.303587 fedex-sdk-1.0.8/fedex_sdk.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-07-25 06:27:53.000000 fedex-sdk-1.0.8/fedex_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2343 2023-07-25 06:27:53.000000 fedex-sdk-1.0.8/fedex_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:27:53.000000 fedex-sdk-1.0.8/fedex_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 06:27:53.000000 fedex-sdk-1.0.8/fedex_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:27:54.305587 fedex-sdk-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-07-21 08:44:20.000000 fedex-sdk-1.0.8/setup.py
```

### Comparing `fedex-sdk-1.0.7/FedexSDK/FedExSDK.py` & `fedex-sdk-1.0.8/FedexSDK/FedExSDK.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/Address.py` & `fedex-sdk-1.0.8/FedexSDK/models/Address.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/Contact.py` & `fedex-sdk-1.0.8/FedexSDK/models/Contact.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/Request.py` & `fedex-sdk-1.0.8/FedexSDK/models/Request.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/RequestedShipment.py` & `fedex-sdk-1.0.8/FedexSDK/models/RequestedShipment.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/Tin.py` & `fedex-sdk-1.0.8/FedexSDK/models/Tin.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/__init__.py` & `fedex-sdk-1.0.8/FedexSDK/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/label/CompletedShipmentDetail.py` & `fedex-sdk-1.0.8/FedexSDK/models/label/CompletedShipmentDetail.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/label/OperationalDetail.py` & `fedex-sdk-1.0.8/FedexSDK/models/label/OperationalDetail.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/label/Response.py` & `fedex-sdk-1.0.8/FedexSDK/models/label/Response.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/label/ShipmentDocument.py` & `fedex-sdk-1.0.8/FedexSDK/models/label/ShipmentDocument.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/FedexSDK/models/tracking/TrackResult.py` & `fedex-sdk-1.0.8/FedexSDK/models/tracking/TrackResult.py`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/fedex_sdk.egg-info/SOURCES.txt` & `fedex-sdk-1.0.8/fedex_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedex-sdk-1.0.7/setup.py` & `fedex-sdk-1.0.8/setup.py`

 * *Files identical despite different names*

