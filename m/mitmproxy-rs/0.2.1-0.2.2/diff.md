# Comparing `tmp/mitmproxy_rs-0.2.1.tar.gz` & `tmp/mitmproxy_rs-0.2.2.tar.gz`

## Comparing `mitmproxy_rs-0.2.1.tar` & `mitmproxy_rs-0.2.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/Cargo.toml
--rw-r--r--   0     1001      123       84 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.cargo/config.toml
--rw-r--r--   0     1001      123       28 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/FUNDING.yml
--rw-r--r--   0     1001      123      511 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/dependabot.yml
--rw-r--r--   0     1001      123        5 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/python-version.txt
--rwxr-xr-x   0     1001      123     2437 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/scripts/build-macos-redirector.sh
--rw-r--r--   0     1001      123     1158 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/autofix.yml
--rw-r--r--   0     1001      123     5072 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/ci.yml
--rw-r--r--   0     1001      123     1869 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/docs.yml
--rw-r--r--   0     1001      123       71 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.gitignore
--rw-r--r--   0     1001      123     4472 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/CHANGELOG.md
--rwxr-xr-x   0     1001      123     2085 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1080 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/LICENSE
--rw-r--r--   0     1001      123     3271 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/README.md
--rw-r--r--   0     1001      123   243520 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/architecture.png
--rw-r--r--   0     1001      123       22 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/.gitignore
--rw-r--r--   0     1001      123      220 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/local.conf
--rw-r--r--   0     1001      123      214 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/nonlocal.conf
--rw-r--r--   0     1001      123    67352 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/openvpnserv.exe
--rw-r--r--   0     1001      123    10121 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/plot.py
--rwxr-xr-x   0     1001      123     1730 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/process.rs
--rw-r--r--   0     1001      123     2375 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/py_echo_client.py
--rw-r--r--   0     1001      123     1246 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/py_echo_server.py
--rw-r--r--   0     1001      123     2346 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/wg_echo_client.py
--rw-r--r--   0     1001      123     2036 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/wg_echo_server.py
--rw-r--r--   0     1001      123      306 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/build.rs
--rwxr-xr-x   0     1001      123      264 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/coverage.sh
--rw-r--r--   0     1001      123      431 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/Info.plist
--rw-r--r--   0     1001      123      690 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/MitmproxyAppleExtension.entitlements
--rw-r--r--   0     1001      123     5141 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/PacketTunnelProvider.swift
--rw-r--r--   0     1001      123     5628 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/ipc.pb.swift
--rw-r--r--   0     1001      123   345532 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/1024.png
--rw-r--r--   0     1001      123    13181 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/128.png
--rw-r--r--   0     1001      123      902 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/16.png
--rw-r--r--   0     1001      123    36415 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/256.png
--rw-r--r--   0     1001      123     2205 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/32.png
--rw-r--r--   0     1001      123   116514 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/512.png
--rw-r--r--   0     1001      123     5379 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/64.png
--rw-r--r--   0     1001      123     1358 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0     1001      123       63 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/Contents.json
--rw-r--r--   0     1001      123      171 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Constants.swift
--rw-r--r--   0     1001      123     1509 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Controller/AppDelegate.swift
--rw-r--r--   0     1001      123      218 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Controller/ViewController.swift
--rw-r--r--   0     1001      123      690 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/MitmproxyAppleTunnel.entitlements
--rw-r--r--   0     1001      123     6048 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Model/Proxy.swift
--rw-r--r--   0     1001      123    60507 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/View/Base.lproj/Main.storyboard
--rw-r--r--   0     1001      123    26319 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.pbxproj
--rw-r--r--   0     1001      123      135 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/contents.xcworkspacedata
--rw-r--r--   0     1001      123      238 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0     1001      123      181 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/WorkspaceSettings.xcsettings
--rw-r--r--   0     1001      123      311 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
--rw-r--r--   0     1001      123      182 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcuserdata/emanuelemicheletti.xcuserdatad/IDEFindNavigatorScopes.plist
--rw-r--r--   0     1001      123      453 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcuserdata/emanuelemicheletti.xcuserdatad/WorkspaceSettings.xcsettings
--rw-r--r--   0     1001      123     3869 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleExtension.xcscheme
--rw-r--r--   0     1001      123     4638 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleTunnel.xcscheme
--rw-r--r--   0     1001      123      872 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcdebugger/Breakpoints_v2.xcbkptlist
--rw-r--r--   0     1001      123      719 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcschemes/xcschememanagement.plist
--rwxr-xr-x   0     1001      123     4410 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/intercept_conf.rs
--rwxr-xr-x   0     1001      123      202 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/lib.rs
--rwxr-xr-x   0     1001      123     3863 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/messages.rs
--rwxr-xr-x   0     1001      123      126 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/mod.rs
--rwxr-xr-x   0     1001      123    26233 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/task.rs
--rwxr-xr-x   0     1001      123    26991 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/tests.rs
--rwxr-xr-x   0     1001      123     2705 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/virtual_device.rs
--rw-r--r--   0     1001      123      322 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/ipc.proto
--rwxr-xr-x   0     1001      123      740 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/mod.rs
--rwxr-xr-x   0     1001      123     7965 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/windows.rs
--rwxr-xr-x   0     1001      123    13781 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs
--rw-r--r--   0     1001      123      243 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/processes.rs
--rwxr-xr-x   0     1001      123     3721 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/shutdown.rs
--rwxr-xr-x   0     1001      123        1 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/util.rs
--rw-r--r--   0     1001      123     5276 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/icons.rs
--rw-r--r--   0     1001      123       51 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/mod.rs
--rw-r--r--   0     1001      123     6828 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/network.rs
--rw-r--r--   0     1001      123    10928 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/processes.rs
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123       97 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/.gitignore
--rw-r--r--   0     1001      123     2850 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/README.md
--rwxr-xr-x   0     1001      123     1919 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/build.rs
--rw-r--r--   0     1001      123      132 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/__init__.py
--rw-r--r--   0     1001      123     2296 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/__init__.pyi
--rw-r--r--   0     1001      123      121 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/_pyinstaller/__init__.py
--rw-r--r--   0     1001      123       99 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
--rw-r--r--   0     1001      123        0 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/py.typed
--rw-r--r--   0     1001      123      745 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/pyproject.toml
--rwxr-xr-x   0     1001      123     3575 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/datagram_transport.rs
--rwxr-xr-x   0     1001      123     1737 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123     2054 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/process_info.rs
--rwxr-xr-x   0     1001      123    10121 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/server.rs
--rwxr-xr-x   0     1001      123     7234 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/task.rs
--rwxr-xr-x   0     1001      123     5452 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/tcp_stream.rs
--rwxr-xr-x   0     1001      123     2048 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/util.rs
--rwxr-xr-x   0     1001      123       70 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/stubtest-allowlist.txt
--rw-r--r--   0     1001      123      125 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/test.py
--rw-r--r--   0     1001      123    70506 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/Cargo.toml
+-rw-r--r--   0     1001      123       84 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.cargo/config.toml
+-rw-r--r--   0     1001      123       28 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/FUNDING.yml
+-rw-r--r--   0     1001      123      511 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/dependabot.yml
+-rw-r--r--   0     1001      123        5 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/python-version.txt
+-rwxr-xr-x   0     1001      123     2437 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/scripts/build-macos-redirector.sh
+-rw-r--r--   0     1001      123     1158 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/workflows/autofix.yml
+-rw-r--r--   0     1001      123     5072 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     1869 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/workflows/docs.yml
+-rw-r--r--   0     1001      123       71 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.gitignore
+-rw-r--r--   0     1001      123     4472 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/CHANGELOG.md
+-rwxr-xr-x   0     1001      123     2085 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1080 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/LICENSE
+-rw-r--r--   0     1001      123     3271 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/README.md
+-rw-r--r--   0     1001      123   243520 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/architecture.png
+-rw-r--r--   0     1001      123       22 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/.gitignore
+-rw-r--r--   0     1001      123      220 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/local.conf
+-rw-r--r--   0     1001      123      214 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/nonlocal.conf
+-rw-r--r--   0     1001      123    67352 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/openvpnserv.exe
+-rw-r--r--   0     1001      123    10121 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/plot.py
+-rwxr-xr-x   0     1001      123     1730 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/process.rs
+-rw-r--r--   0     1001      123     2375 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/py_echo_client.py
+-rw-r--r--   0     1001      123     1246 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/py_echo_server.py
+-rw-r--r--   0     1001      123     2346 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/wg_echo_client.py
+-rw-r--r--   0     1001      123     2036 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/wg_echo_server.py
+-rw-r--r--   0     1001      123      303 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/build.rs
+-rwxr-xr-x   0     1001      123      264 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/coverage.sh
+-rw-r--r--   0     1001      123      431 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/Info.plist
+-rw-r--r--   0     1001      123      690 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/MitmproxyAppleExtension.entitlements
+-rw-r--r--   0     1001      123     5141 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/PacketTunnelProvider.swift
+-rw-r--r--   0     1001      123     5628 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/ipc.pb.swift
+-rw-r--r--   0     1001      123   345532 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/1024.png
+-rw-r--r--   0     1001      123    13181 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/128.png
+-rw-r--r--   0     1001      123      902 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/16.png
+-rw-r--r--   0     1001      123    36415 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/256.png
+-rw-r--r--   0     1001      123     2205 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/32.png
+-rw-r--r--   0     1001      123   116514 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/512.png
+-rw-r--r--   0     1001      123     5379 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/64.png
+-rw-r--r--   0     1001      123     1358 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0     1001      123       63 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/Contents.json
+-rw-r--r--   0     1001      123      171 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Constants.swift
+-rw-r--r--   0     1001      123     1509 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Controller/AppDelegate.swift
+-rw-r--r--   0     1001      123      218 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Controller/ViewController.swift
+-rw-r--r--   0     1001      123      690 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/MitmproxyAppleTunnel.entitlements
+-rw-r--r--   0     1001      123     6048 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Model/Proxy.swift
+-rw-r--r--   0     1001      123    60507 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/View/Base.lproj/Main.storyboard
+-rw-r--r--   0     1001      123    26319 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.pbxproj
+-rw-r--r--   0     1001      123      135 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+-rw-r--r--   0     1001      123      238 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0     1001      123      181 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/WorkspaceSettings.xcsettings
+-rw-r--r--   0     1001      123      311 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
+-rw-r--r--   0     1001      123      182 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcuserdata/emanuelemicheletti.xcuserdatad/IDEFindNavigatorScopes.plist
+-rw-r--r--   0     1001      123      453 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcuserdata/emanuelemicheletti.xcuserdatad/WorkspaceSettings.xcsettings
+-rw-r--r--   0     1001      123     3869 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleExtension.xcscheme
+-rw-r--r--   0     1001      123     4638 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleTunnel.xcscheme
+-rw-r--r--   0     1001      123      872 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcdebugger/Breakpoints_v2.xcbkptlist
+-rw-r--r--   0     1001      123      719 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcschemes/xcschememanagement.plist
+-rwxr-xr-x   0     1001      123     4410 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/intercept_conf.rs
+-rwxr-xr-x   0     1001      123      202 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/lib.rs
+-rwxr-xr-x   0     1001      123     3863 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/messages.rs
+-rwxr-xr-x   0     1001      123      126 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/network/mod.rs
+-rwxr-xr-x   0     1001      123    26233 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/network/task.rs
+-rwxr-xr-x   0     1001      123    26991 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/network/tests.rs
+-rwxr-xr-x   0     1001      123     2705 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/network/virtual_device.rs
+-rw-r--r--   0     1001      123      322 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/packet_sources/ipc.proto
+-rwxr-xr-x   0     1001      123      740 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/packet_sources/mod.rs
+-rwxr-xr-x   0     1001      123     7965 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/packet_sources/windows.rs
+-rwxr-xr-x   0     1001      123    13781 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs
+-rw-r--r--   0     1001      123      243 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/processes.rs
+-rwxr-xr-x   0     1001      123     3721 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/shutdown.rs
+-rwxr-xr-x   0     1001      123        1 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/util.rs
+-rw-r--r--   0     1001      123     5276 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/windows/icons.rs
+-rw-r--r--   0     1001      123       51 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/windows/mod.rs
+-rw-r--r--   0     1001      123     6828 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/windows/network.rs
+-rw-r--r--   0     1001      123    10928 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/windows/processes.rs
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123       97 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/.gitignore
+-rw-r--r--   0     1001      123     2850 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/README.md
+-rwxr-xr-x   0     1001      123     1919 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/build.rs
+-rw-r--r--   0     1001      123      132 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/mitmproxy_rs/__init__.py
+-rw-r--r--   0     1001      123     2296 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/mitmproxy_rs/__init__.pyi
+-rw-r--r--   0     1001      123      121 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/mitmproxy_rs/_pyinstaller/__init__.py
+-rw-r--r--   0     1001      123       99 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
+-rw-r--r--   0     1001      123        0 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/mitmproxy_rs/py.typed
+-rw-r--r--   0     1001      123      745 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/pyproject.toml
+-rwxr-xr-x   0     1001      123     3575 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/src/datagram_transport.rs
+-rwxr-xr-x   0     1001      123     1737 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123     2054 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/src/process_info.rs
+-rwxr-xr-x   0     1001      123    10121 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/src/server.rs
+-rwxr-xr-x   0     1001      123     7234 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/src/task.rs
+-rwxr-xr-x   0     1001      123     5452 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/src/tcp_stream.rs
+-rwxr-xr-x   0     1001      123     2048 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/src/util.rs
+-rwxr-xr-x   0     1001      123       70 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/stubtest-allowlist.txt
+-rw-r--r--   0     1001      123      125 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/test.py
+-rw-r--r--   0     1001      123    70506 2023-08-07 12:42:35.000000 mitmproxy_rs-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.2/PKG-INFO
```

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/Cargo.toml` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 ]
 
 [workspace.package]
 authors = [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version = "0.2.1"
+version = "0.2.2"
 publish = false
 repository = "https://github.com/mitmproxy/mitmproxy-rs"
 edition = "2021"
 rust-version = "1.65.0"
 
 [package]
 name = "mitmproxy"
 license = "MIT"
 authors= [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version= "0.2.1"
+version= "0.2.2"
 repository= "https://github.com/mitmproxy/mitmproxy-rs"
 edition= "2021"
 rust-version= "1.65.0"
 publish= false
 
 [dependencies]
 anyhow = { version = "1.0.71", features = ["backtrace"] }
```

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/scripts/build-macos-redirector.sh` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/scripts/build-macos-redirector.sh`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/autofix.yml` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/workflows/autofix.yml`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/ci.yml` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/docs.yml` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/CHANGELOG.md` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/CONTRIBUTING.md` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/LICENSE` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/LICENSE`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/README.md` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/architecture.png` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/architecture.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/openvpnserv.exe` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/openvpnserv.exe`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/plot.py` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/plot.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/process.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/process.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/py_echo_client.py` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/py_echo_client.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/py_echo_server.py` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/py_echo_server.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/wg_echo_client.py` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/wg_echo_client.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/wg_echo_server.py` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/benches/wg_echo_server.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/MitmproxyAppleExtension.entitlements` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/MitmproxyAppleExtension.entitlements`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/PacketTunnelProvider.swift` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/PacketTunnelProvider.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/ipc.pb.swift` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/ipc.pb.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/1024.png` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/1024.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/128.png` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/128.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/16.png` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/16.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/256.png` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/256.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/32.png` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/32.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/512.png` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/512.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/64.png` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/64.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/Contents.json` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Controller/AppDelegate.swift` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Controller/AppDelegate.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/MitmproxyAppleTunnel.entitlements` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/MitmproxyAppleTunnel.entitlements`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Model/Proxy.swift` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Model/Proxy.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/View/Base.lproj/Main.storyboard` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/View/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.pbxproj` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleExtension.xcscheme` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleExtension.xcscheme`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleTunnel.xcscheme` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleTunnel.xcscheme`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcdebugger/Breakpoints_v2.xcbkptlist` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcdebugger/Breakpoints_v2.xcbkptlist`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcschemes/xcschememanagement.plist` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcschemes/xcschememanagement.plist`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/intercept_conf.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/intercept_conf.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/messages.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/messages.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/task.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/network/task.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/tests.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/network/tests.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/virtual_device.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/network/virtual_device.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/mod.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/packet_sources/mod.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/windows.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/packet_sources/windows.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/shutdown.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/shutdown.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/icons.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/windows/icons.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/network.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/windows/network.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/processes.rs` & `mitmproxy_rs-0.2.2/local_dependencies/mitmproxy/src/windows/processes.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/Cargo.toml` & `mitmproxy_rs-0.2.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [package]
 name = "mitmproxy_rs"
 license = "MIT"
 authors= [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version= "0.2.1"
+version= "0.2.2"
 repository= "https://github.com/mitmproxy/mitmproxy-rs"
 edition= "2021"
 rust-version= "1.65.0"
 publish= false
 
 [lib]
 name = "mitmproxy_rs"
```

### Comparing `mitmproxy_rs-0.2.1/README.md` & `mitmproxy_rs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/build.rs` & `mitmproxy_rs-0.2.2/build.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/mitmproxy_rs/__init__.pyi` & `mitmproxy_rs-0.2.2/mitmproxy_rs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/pyproject.toml` & `mitmproxy_rs-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/src/datagram_transport.rs` & `mitmproxy_rs-0.2.2/src/datagram_transport.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/src/lib.rs` & `mitmproxy_rs-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/src/process_info.rs` & `mitmproxy_rs-0.2.2/src/process_info.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/src/server.rs` & `mitmproxy_rs-0.2.2/src/server.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/src/task.rs` & `mitmproxy_rs-0.2.2/src/task.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/src/tcp_stream.rs` & `mitmproxy_rs-0.2.2/src/tcp_stream.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/src/util.rs` & `mitmproxy_rs-0.2.2/src/util.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.1/Cargo.lock` & `mitmproxy_rs-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1305,27 +1305,27 @@
  "libc",
  "wasi",
  "windows-sys",
 ]
 
 [[package]]
 name = "mitm-wg-test-client"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "anyhow",
  "boringtun",
  "data-encoding",
  "hex",
  "smoltcp",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "mitmproxy"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "anyhow",
  "async-trait",
  "boringtun",
  "console-subscriber",
  "criterion",
  "env_logger",
@@ -1342,15 +1342,15 @@
  "tokio",
  "windows",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "mitmproxy_rs"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "anyhow",
  "console-subscriber",
  "data-encoding",
  "env_logger",
  "log",
  "mitmproxy",
@@ -2682,15 +2682,15 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-redirector"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "anyhow",
  "env_logger",
  "hex",
  "internet-packet",
  "log",
  "lru_time_cache",
```

### Comparing `mitmproxy_rs-0.2.1/PKG-INFO` & `mitmproxy_rs-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitmproxy_rs
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

