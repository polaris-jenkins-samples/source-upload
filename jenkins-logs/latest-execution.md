# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Source_Upload/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 5 min 26 sec and counting
- **Timestamp:** 2025-11-13 14:19:37 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 40d74a396e0e7e5758230b6b970dbf6934c3a2fb
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/ithub_Polaris_Source_Upload_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/polaris-jenkins-samples/source-upload.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2 # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/source-upload.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/source-upload.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision 40d74a396e0e7e5758230b6b970dbf6934c3a2fb (main)
Commit message: "Polaris Source Upload"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/source-upload.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 40d74a396e0e7e5758230b6b970dbf6934c3a2fb # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Polaris_Source_Upload/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 14s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 35 moderate, 57 high, 36 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (polaris-source-upload)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Source_Upload
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [POLARIS]
[Security Scan] INFO: Parameters for polaris:
[Security Scan] INFO:  --- polaris_waitForScan = true
[Security Scan] INFO:  --- polaris_server_url = https://poc.polaris.blackduck.com
[Security Scan] INFO:  --- polaris_assessment_types = SAST,SCA
[Security Scan] INFO:  --- polaris_access_token = ******************************************************************************
[Security Scan] INFO:  --- polaris_test_sca_location = remote
[Security Scan] INFO:  --- polaris_test_sast_location = remote
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Polaris parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Source_Upload
[Security Scan] INFO: Polaris Application Name: source-upload
[Security Scan] INFO: Polaris Project Name: source-upload
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Source_Upload
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2/polaris_input4800120650740509948.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 14:14:39.4466 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 14:14:39.4541 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 14:14:40.7357 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 14:14:40.7358 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 14:14:40.7358 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 14:14:40.7358 IST [Bridge CLI] INFO: network.airgap = false [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7358 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7358 IST [Bridge CLI] INFO: polaris.application.name = source-upload [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7358 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7359 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7359 IST [Bridge CLI] INFO: polaris.project.name = source-upload [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7359 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7359 IST [Bridge CLI] INFO: polaris.test.sast.location = remote [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7359 IST [Bridge CLI] INFO: polaris.test.sca.location = remote [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7359 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input4800120650740509948.json]
2025-11-13 14:14:40.7359 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 14:14:40.7359 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 14:14:40.7375 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 14:14:40.7375 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 14:14:40.7375 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 14:14:40.7375 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 14:14:40.8251 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 14:14:40.8288 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 14:14:40.8290 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 14:14:40.8290 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 14:14:40.8322 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 14:14:40.8323 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 14:14:40.8325 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 14:14:42.9224 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 14:14:42.9227 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 14:14:42.9230 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 14:14:42.9244 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 14:14:42.9246 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 14:14:42.9249 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 14:14:42.9356 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 14:14:42.9739 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 14:14:42.9742 IST [Check pull request] INFO: Adapter finished
2025-11-13 14:14:43.0253 IST [Bridge CLI] INFO: Starting adapters for stage source-zipper
2025-11-13 14:14:43.0253 IST [Bridge CLI] INFO: Starting adapters for stage polaris-source-upload
2025-11-13 14:14:43.0253 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 14:14:43.0259 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 14:14:43.0259 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 14:14:43.0259 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 14:14:43.0259 IST [Bridge CLI] INFO: Starting Adapter: Polaris Source Test Creator
2025-11-13 14:14:43.0259 IST [Bridge CLI] INFO: Starting Adapter: Project Source Zipper
2025-11-13 14:14:43.0261 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 14:14:43.4754 IST [Project Source Zipper] INFO: Creating source zip of "/Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2/nodejs-npm" directory
2025-11-13 14:14:48.5912 IST [Project Source Zipper] INFO: Successfully created source zip at "/Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2/nodejs-npm/.bridge/project_source_zipper/source.zip"
2025-11-13 14:14:48.5978 IST [Project Source Zipper] INFO: Provided value for resource 'project.source.archive'
2025-11-13 14:14:48.5980 IST [Project Source Zipper] INFO: Adapter finished
2025-11-13 14:14:50.3452 IST [Polaris Source Test Creator] INFO: Uploading zip archive "/Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2/nodejs-npm/.bridge/project_source_zipper/source.zip"
2025-11-13 14:14:51.0255 IST [Polaris Source Test Creator] INFO: Uploading Progress: 0%  16384/39717231
2025-11-13 14:14:54.9692 IST [Polaris Source Test Creator] INFO: Uploading Progress: 25%  9945088/39717231
2025-11-13 14:14:58.0491 IST [Polaris Source Test Creator] INFO: Uploading Progress: 50%  19873792/39717231
2025-11-13 14:15:00.9157 IST [Polaris Source Test Creator] INFO: Uploading Progress: 75%  29802496/39717231
2025-11-13 14:15:03.9370 IST [Polaris Source Test Creator] INFO: Uploading Progress: 100%  39717231/39717231
2025-11-13 14:15:04.4685 IST [Polaris Source Test Creator] INFO: Successfully uploaded zip archive "/Users/madhusud/Jenkins_Testing/Nodes/workspace/ithub_Polaris_Source_Upload_main@2/nodejs-npm/.bridge/project_source_zipper/source.zip"
2025-11-13 14:15:04.4686 IST [Polaris Source Test Creator] INFO: Creating test for "SAST" assessment with default scan type "SAST_FULL"
2025-11-13 14:15:04.4686 IST [Polaris Source Test Creator] INFO: Creating test for "SCA" assessment with default scan type "SCA-PACKAGE"
2025-11-13 14:15:05.1772 IST [Polaris Source Test Creator] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "V2LHTCV"
2025-11-13 14:15:05.2058 IST [Polaris Source Test Creator] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "RVT9WU3"
2025-11-13 14:15:05.2337 IST [Polaris Source Test Creator] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 14:15:05.2343 IST [Polaris Source Test Creator] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 14:15:05.2349 IST [Polaris Source Test Creator] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 14:15:05.2351 IST [Polaris Source Test Creator] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 14:15:05.2352 IST [Polaris Source Test Creator] INFO: Provided value for resource 'project.source.uploadSuccessful'
2025-11-13 14:15:05.2356 IST [Polaris Source Test Creator] INFO: Adapter finished
2025-11-13 14:15:05.2823 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "f79af25c-c753-44ac-9a87-bed0ac5df15c"
2025-11-13 14:15:05.2827 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "27328912-1258-4a9b-a2b1-dc668fae9b10"
2025-11-13 14:15:06.0558 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "f79af25c-c753-44ac-9a87-bed0ac5df15c" is "New"
2025-11-13 14:15:06.0559 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "27328912-1258-4a9b-a2b1-dc668fae9b10" is "New"
2025-11-13 14:17:20.0695 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "f79af25c-c753-44ac-9a87-bed0ac5df15c" is "Queuing"
2025-11-13 14:17:20.0823 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "27328912-1258-4a9b-a2b1-dc668fae9b10" is "Queuing"
2025-11-13 14:18:01.3079 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "f79af25c-c753-44ac-9a87-bed0ac5df15c" is "Scanning"
2025-11-13 14:18:01.3252 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "27328912-1258-4a9b-a2b1-dc668fae9b10" is "Scanning & Publishing"
2025-11-13 14:18:32.1969 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "f79af25c-c753-44ac-9a87-bed0ac5df15c" completed successfully
2025-11-13 14:19:23.8257 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "27328912-1258-4a9b-a2b1-dc668fae9b10" is "In Progress"
2025-11-13 14:19:34.1338 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "27328912-1258-4a9b-a2b1-dc668fae9b10" completed successfully
2025-11-13 14:19:34.1599 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 14:19:34.1603 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 14:19:34.1610 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 14:19:34.2273 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 14:19:34.2279 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 14:19:35.2487 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "f79af25c-c753-44ac-9a87-bed0ac5df15c"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 12
}
2025-11-13 14:19:35.3222 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "27328912-1258-4a9b-a2b1-dc668fae9b10"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 14:19:35.3485 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.informational'
2025-11-13 14:19:35.3487 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.critical'
2025-11-13 14:19:35.3489 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.low'
2025-11-13 14:19:35.3490 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.medium'
2025-11-13 14:19:35.3492 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.issues.high'
2025-11-13 14:19:35.3493 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.medium'
2025-11-13 14:19:35.3495 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.critical'
2025-11-13 14:19:35.3496 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.high'
2025-11-13 14:19:35.3498 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.informational'
2025-11-13 14:19:35.3499 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.issues.low'
2025-11-13 14:19:35.3503 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 14:19:35.4049 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 14:19:35.4059 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 14:19:36.3197 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 14:19:36.3436 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 14:19:36.4002 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "f79af25c-c753-44ac-9a87-bed0ac5df15c" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/508d0195-980f-49ce-a87e-cf5befda4ac6/projects/9dd1f837-628e-4a91-b647-6f4a8844ae74/tests/f79af25c-c753-44ac-9a87-bed0ac5df15c/detected-issues
2025-11-13 14:19:36.4008 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "27328912-1258-4a9b-a2b1-dc668fae9b10" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/508d0195-980f-49ce-a87e-cf5befda4ac6/projects/9dd1f837-628e-4a91-b647-6f4a8844ae74/tests/27328912-1258-4a9b-a2b1-dc668fae9b10/detected-issues
2025-11-13 14:19:36.4009 IST [Polaris Status Provider] INFO: Polaris issues view for project "source-upload", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/508d0195-980f-49ce-a87e-cf5befda4ac6/projects/9dd1f837-628e-4a91-b647-6f4a8844ae74/issues?branchId=f449671a-b934-4213-885b-2d20a6c5a087
2025-11-13 14:19:36.4084 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 14:19:36.4085 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 14:19:36.4087 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 14:19:36.4088 IST [Polaris Status Provider] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 302
[Security Scan] INFO: Security Scan execution is successful
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:polaris-jenkins-samples, repoName:source-upload, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Polaris_Source_Upload/main
[Pipeline] echo
Build Number: 2
[Pipeline] echo
GitHub Organization: polaris-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: source-upload
[Pipeline] echo
Target repository: polaris-jenkins-samples/source-upload
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*