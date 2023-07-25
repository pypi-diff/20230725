# Comparing `tmp/dcentralab_qa_infra_automation-1.0.6.tar.gz` & `tmp/dcentralab_qa_infra_automation-1.0.7.tar.gz`

## Comparing `dcentralab_qa_infra_automation-1.0.6.tar` & `dcentralab_qa_infra_automation-1.0.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/BasePage.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/CreatePasswordPage.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/MetamaskInstallCompletedPage.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0     9684 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     7775 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/CreatePasswordPage.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/MetamaskInstallCompletedPage.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-1.0.7/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-1.0.6/.idea/workspace.xml` & `dcentralab_qa_infra_automation-1.0.7/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `dcentralab_qa_infra_automation-1.0.6/.idea/workspace.xml` & `dcentralab_qa_infra_automation-1.0.7/.idea/workspace.xml`

```diff
@@ -1,14 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="ce720036-d8eb-462b-9d8d-e560b75fc3e8" name="Changes" comment="add infra developments">
       <change afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/__init__.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/data/read_data.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/data/read_data.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/BasePage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/BasePage.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py" afterDir="false"/>
```

### Comparing `dcentralab_qa_infra_automation-1.0.6/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-1.0.7/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,24 +34,29 @@
 def initBraveDriver():
     """
     init brave driver, using ChromeDriverManager for chromeDriver installation
     :return: driver - driver instance
     """
     options = webdriver.ChromeOptions()
     options.binary_location = addBraveToChrome()
-
-    chrome_service = Service(executable_path=ChromeDriverManager().install())
+    if pytest.data_driven.get("OS") == "mac":
+        chrome_service = Service(executable_path=ChromeDriverManager(pytest.data_driven.get("chrome_driver_version")).install())
+    else:
+        chrome_service = Service(executable_path=ChromeDriverManager().install())
     driver = webdriver.Chrome(service=chrome_service, options=options)
     return driver
 
 
 def initBraveDriverWithExtension():
     """
     init brave driver with CRX extension, using ChromeDriverManager for chromeDriver installation
     :return: driver - driver instance
     """
     options = webdriver.ChromeOptions()
     options.binary_location = addBraveToChrome()
     options.add_extension(addExtensionToChrome())
-    chrome_service = Service(executable_path=ChromeDriverManager().install())
+    if pytest.data_driven.get("OS") == "mac":
+        chrome_service = Service(executable_path=ChromeDriverManager(pytest.data_driven.get("chrome_driver_version")).install())
+    else:
+        chrome_service = Service(executable_path=ChromeDriverManager().install())
     driver = webdriver.Chrome(service=chrome_service, options=options)
     return driver
```

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,22 +14,28 @@
 
 def initChromeDriver():
     """
     init chrome driver, using ChromeDriverManager for chromeDriver installation
     :return: driver - driver instance
     """
     pytest.logger.info("chrome driver type injected, initialize chrome browser")
-    chrome_service = Service(executable_path=ChromeDriverManager().install())
+    if pytest.data_driven.get("OS") == "mac":
+        chrome_service = Service(executable_path=ChromeDriverManager(pytest.data_driven.get("chrome_driver_version")).install())
+    else:
+        chrome_service = Service(executable_path=ChromeDriverManager().install())
     driver = webdriver.Chrome(service=chrome_service)
     return driver
 
 
 def initChromeDriverWithExtension():
     """
     init chrome driver with CRX extension, using ChromeDriverManager for chromeDriver installation
     :return: driver - driver instance
     """
     options = webdriver.ChromeOptions()
     options.add_extension(addExtensionToChrome())
-    chrome_service = Service(executable_path=ChromeDriverManager().install())
+    if pytest.data_driven.get("OS") == "mac":
+        chrome_service = Service(executable_path=ChromeDriverManager(pytest.data_driven.get("chrome_driver_version")).install())
+    else:
+        chrome_service = Service(executable_path=ChromeDriverManager().install())
     driver = webdriver.Chrome(service=chrome_service, options=options)
     return driver
```

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/BasePage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/BasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/CreatePasswordPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/MetamaskInstallCompletedPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/MetamaskInstallCompletedPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/ConnectWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/CreateAccountPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/ImportSeedPhrasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/NamiBasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/SignPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/SuccessfullyCreatedWalletPage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/pages/namiPages/WelcomePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py` & `dcentralab_qa_infra_automation-1.0.7/src/dcentralab_qa_infra_automation/walletsActions/NamiActions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/LICENSE` & `dcentralab_qa_infra_automation-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-1.0.6/pyproject.toml` & `dcentralab_qa_infra_automation-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-1.0.6/PKG-INFO` & `dcentralab_qa_infra_automation-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 1.0.6
+Version: 1.0.7
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

