# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Coverity_Buildless_Scan/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 2 min 24 sec and counting
- **Timestamp:** 2025-11-13 19:22:09 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 472defd2c8f52fb628b731043abf0b2b0d0fdf32
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/hub_Coverity_Buildless_Scan_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/.git # timeout=10
 > git config remote.origin.url https://github.com/coverity-cnc-jenkins-samples/buildless-scan.git # timeout=10
Fetching upstream changes from https://github.com/coverity-cnc-jenkins-samples/buildless-scan.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/coverity-cnc-jenkins-samples/buildless-scan.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision 472defd2c8f52fb628b731043abf0b2b0d0fdf32 (main)
Commit message: "Coverity Buildless Scan"
First time build. Skipping changelog.
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 472defd2c8f52fb628b731043abf0b2b0d0fdf32 # timeout=10
 > git rev-list --no-walk 166ceb51b2a82142a333f7e11ce3cbbc69d54e98 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (coverity-buildless-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Buildless_Scan
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [COVERITY]
[Security Scan] INFO: Parameters for coverity:
[Security Scan] INFO:  --- coverity_passphrase = ******************************************************************************
[Security Scan] INFO:  --- coverity_waitForScan = true
[Security Scan] INFO:  --- coverity_url = https://integrations-qa.dev.cnc.duckutil.net
[Security Scan] INFO:  --- coverity_user = admin
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_ssl_trustAll = false
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Coverity parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Buildless_Scan
[Security Scan] INFO: Coverity Project Name: buildless-scan
[Security Scan] INFO: Coverity Stream Name: buildless-scan-main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Buildless_Scan
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage connect --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/coverity_input8060026454002462651.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 19:19:56.1017 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 19:19:56.1076 IST [Bridge CLI] INFO: Found version "3.0.128" in registry for workflow "connect", trying to load it from local cache
2025-11-13 19:19:56.1701 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 19:19:56.1701 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 19:19:56.1701 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 19:19:56.1701 IST [Bridge CLI] INFO: coverity.connect.project.name = buildless-scan [coverity_input8060026454002462651.json]
2025-11-13 19:19:56.1702 IST [Bridge CLI] INFO: coverity.connect.stream.name = buildless-scan-main [coverity_input8060026454002462651.json]
2025-11-13 19:19:56.1702 IST [Bridge CLI] INFO: coverity.connect.url = https://integrations-qa.dev.cnc.duckutil.net [coverity_input8060026454002462651.json]
2025-11-13 19:19:56.1702 IST [Bridge CLI] INFO: coverity.connect.user.name = admin [coverity_input8060026454002462651.json]
2025-11-13 19:19:56.1702 IST [Bridge CLI] INFO: coverity.connect.user.password = ***************************************** [coverity_input8060026454002462651.json]
2025-11-13 19:19:56.1702 IST [Bridge CLI] INFO: coverity.waitForScan = true [coverity_input8060026454002462651.json]
2025-11-13 19:19:56.1702 IST [Bridge CLI] INFO: network.airgap = false [coverity_input8060026454002462651.json]
2025-11-13 19:19:56.1702 IST [Bridge CLI] INFO: network.ssl.trustAll = false [coverity_input8060026454002462651.json]
2025-11-13 19:19:56.1702 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 19:19:56.1703 IST [Bridge CLI] INFO: Starting adapters for stage connect
2025-11-13 19:19:56.1706 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Controller
2025-11-13 19:19:56.1750 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 19:19:56.2041 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 19:19:56.2043 IST [Check pull request] INFO: Adapter finished
2025-11-13 19:19:58.9601 IST [Coverity Connect Controller] INFO: No coverity version is configured, will use the default or latest supported version from the server
2025-11-13 19:19:59.0431 IST [Coverity Connect Controller] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 19:19:59.0432 IST [Bridge CLI] INFO: Starting adapters for stage connect-post-processing
2025-11-13 19:19:59.0432 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-13 19:19:59.0432 IST [Bridge CLI] INFO: Starting adapters for stage connect-scan
2025-11-13 19:19:59.0436 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Scan
2025-11-13 19:19:59.0436 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Post Scan
2025-11-13 19:19:59.0436 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-13 19:19:59.0439 IST [Coverity Connect Controller] INFO: Adapter finished
2025-11-13 19:19:59.0476 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for Set Version for Coverity
2025-11-13 19:19:59.0477 IST [Default Adapter for Set Version for Coverity] INFO: Provided value for resource 'coverity.version'
2025-11-13 19:19:59.0478 IST [Default Adapter for Set Version for Coverity] INFO: Adapter finished
2025-11-13 19:19:59.1252 IST [Coverity Connect Scan] INFO: Identified workflow: Coverity
2025-11-13 19:19:59.1253 IST [Coverity Connect Scan] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity scan --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -o analyze.location=connect -o commit.connect.url=https://integrations-qa.dev.cnc.duckutil.net -o commit.connect.stream=buildless-scan-main -o commit.connect.project=buildless-scan
2025-11-13 19:19:59.1925 IST [Coverity Connect Scan] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 19:19:59.1940 IST [Coverity Connect Scan] WARNING: No setting for 'commit.connect.on-new-cert' specified.
2025-11-13 19:19:59.1940 IST [Coverity Connect Scan] WARNING: Using default value of 'distrust'.
2025-11-13 19:19:59.1940 IST [Coverity Connect Scan] WARNING: This may result in a certificate validation error when uploading defects to Coverity Connect.
2025-11-13 19:19:59.1940 IST [Coverity Connect Scan] WARNING: If you trust the Coverity Connect instance and certificate validation fails, set 'commit.connect.on-new-cert' to 'trust'.
2025-11-13 19:19:59.1940 IST [Coverity Connect Scan] WARNING: If you are unfamiliar with what this means, please talk to your Coverity Connect administrator.
2025-11-13 19:19:59.1968 IST [Coverity Connect Scan] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 19:19:59.1968 IST [Coverity Connect Scan] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 19:19:59.1979 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir create
2025-11-13 19:20:01.7411 IST [Coverity Connect Scan] INFO: Creating project 'buildless-scan'.
2025-11-13 19:20:02.4609 IST [Coverity Connect Scan] INFO: Creating stream 'buildless-scan-main'.
2025-11-13 19:20:03.2306 IST [Coverity Connect Scan] INFO: Cloud analysis is enabled.
2025-11-13 19:20:06.6393 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 19:20:07.5826 IST [Coverity Connect Scan] INFO: Caching is enabled.
2025-11-13 19:20:09.1032 IST [Coverity Connect Scan] INFO: Telemetry is enabled
2025-11-13 19:20:09.1144 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:20:09.1490 IST [Coverity Connect Scan] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 19:20:09.1555 IST [Coverity Connect Scan] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir'
2025-11-13 19:20:09.1557 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 19:20:09.4808 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 19:20:09.7422 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 19:20:09.9955 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 19:20:10.2413 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 19:20:10.4852 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 19:20:10.7270 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 19:20:10.9767 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 19:20:11.2264 IST [Coverity Connect Scan] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 19:20:11.2264 IST [Coverity Connect Scan] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 19:20:11.2264 IST [Coverity Connect Scan] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 19:20:11.2312 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 19:20:11.4896 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 19:20:11.7489 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 19:20:12.0191 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 19:20:12.2686 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 19:20:12.5115 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 19:20:12.5298 IST [Coverity Connect Scan] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 19:20:12.5298 IST [Coverity Connect Scan] INFO:           and it will not be updated.
2025-11-13 19:20:12.5404 IST [Coverity Connect Scan] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 19:20:12.5463 IST [Coverity Connect Scan] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 19:20:12.5512 IST [Coverity Connect Scan] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/capture-file-list-4177294829 --record-with-source
2025-11-13 19:20:12.5769 IST [Coverity Connect Scan] INFO: Buildless capture started.
2025-11-13 19:20:12.5898 IST [Coverity Connect Scan] INFO: Emitting 84 Files.
2025-11-13 19:20:13.0998 IST [Coverity Connect Scan] INFO: Buildless capture completed.
2025-11-13 19:20:13.1017 IST [Coverity Connect Scan] INFO: Executing action No unwanted TUs to delete
2025-11-13 19:20:13.1017 IST [Coverity Connect Scan] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 19:20:13.1018 IST [Coverity Connect Scan] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir
2025-11-13 19:20:13.1020 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:20:13.1206 IST [Coverity Connect Scan] INFO: Executing action Invalidate capture results
2025-11-13 19:20:13.1248 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 19:20:13.1412 IST [Coverity Connect Scan] INFO: Capture summary:
2025-11-13 19:20:13.1412 IST [Coverity Connect Scan] INFO:     SUCCEEDED: 84
2025-11-13 19:20:13.1412 IST [Coverity Connect Scan] INFO:     INCOMPLETE: 0
2025-11-13 19:20:13.1412 IST [Coverity Connect Scan] INFO:     FAILED: 0
2025-11-13 19:20:13.1412 IST [Coverity Connect Scan] INFO:     IGNORED: 6
2025-11-13 19:20:13.1413 IST [Coverity Connect Scan] INFO:     FILES CAPTURED: 84
2025-11-13 19:20:13.1413 IST [Coverity Connect Scan] INFO:     LINES OF CODE: 32728
2025-11-13 19:20:13.1422 IST [Coverity Connect Scan] INFO: Capture phase took 4.047s.
2025-11-13 19:20:13.1423 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml'
2025-11-13 19:20:13.1455 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/hub_Coverity_Buildless_Scan_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml'
2025-11-13 19:20:13.1466 IST [Coverity Connect Scan] INFO: Analyzing project in the cloud using Coverity Analysis version 2025.9.0
2025-11-13 19:20:13.4538 IST [Coverity Connect Scan] INFO: Creating archive containing data to be analyzed...
2025-11-13 19:20:13.5089 IST [Coverity Connect Scan] INFO: Properties archive created.
2025-11-13 19:20:13.5090 IST [Coverity Connect Scan] INFO: Uploading data for analysis...
2025-11-13 19:20:14.2157 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 19:20:20.1103 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 19:20:20.1106 IST [Coverity Connect Scan] INFO: Scan created.
2025-11-13 19:20:20.1106 IST [Coverity Connect Scan] INFO: The scan ID is 'f959af93-1508-494d-bc3f-cc828512b6e0'
2025-11-13 19:20:20.1141 IST [Coverity Connect Scan] INFO: Waiting for scan to complete...
2025-11-13 19:20:20.1141 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 19:22:05.5521 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 19:22:06.2550 IST [Coverity Connect Scan] INFO: Analysis summary after merging defects:
2025-11-13 19:22:06.2552 IST [Coverity Connect Scan] INFO:     HIGH SEVERITY:    2 issue(s)
2025-11-13 19:22:06.2552 IST [Coverity Connect Scan] INFO:     MEDIUM SEVERITY: 12 issue(s)
2025-11-13 19:22:06.2552 IST [Coverity Connect Scan] INFO:     LOW SEVERITY:    25 issue(s)
2025-11-13 19:22:06.2553 IST [Coverity Connect Scan] INFO:     AUDIT SEVERITY:   0 issue(s)
2025-11-13 19:22:06.2553 IST [Coverity Connect Scan] INFO: Results are available at https://integrations-qa.dev.cnc.duckutil.net:443/query/defects.htm?stream=buildless-scan-main&outstanding=true
2025-11-13 19:22:06.2572 IST [Coverity Connect Scan] INFO: Analyze phase took 1m53.11s.
2025-11-13 19:22:06.2630 IST [Coverity Connect Scan] INFO: Scan complete.
2025-11-13 19:22:06.2738 IST [Coverity Connect Scan] INFO: Coverity Capture completed successfully
2025-11-13 19:22:06.2803 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.completed'
2025-11-13 19:22:06.2805 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 19:22:06.2811 IST [Coverity Connect Scan] INFO: Adapter finished
2025-11-13 19:22:06.3277 IST [SCM Checker] INFO: Adapter finished
2025-11-13 19:22:07.8960 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.resultURL'
2025-11-13 19:22:07.8962 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.policy.issueCount'
2025-11-13 19:22:07.8966 IST [Coverity Connect Post Scan] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 39
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
Configuration: [githubOrg:coverity-cnc-jenkins-samples, repoName:buildless-scan, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Coverity_Buildless_Scan/main
[Pipeline] echo
Build Number: 2
[Pipeline] echo
GitHub Organization: coverity-cnc-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: buildless-scan
[Pipeline] echo
Target repository: coverity-cnc-jenkins-samples/buildless-scan
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*