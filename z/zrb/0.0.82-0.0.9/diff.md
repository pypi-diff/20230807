# Comparing `tmp/zrb-0.0.82.tar.gz` & `tmp/zrb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrb-0.0.82.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "zrb-0.0.9.tar", last modified: Fri Feb  3 02:37:15 2023, max compression
```

## Comparing `zrb-0.0.82.tar` & `zrb-0.0.9.tar`

### file list

```diff
@@ -1,1179 +1,64 @@
--rw-r--r--   0        0        0       94 2023-08-04 06:22:49.215485 zrb-0.0.82/.gitignore
--rw-r--r--   0        0        0      728 2023-08-07 02:54:52.915842 zrb-0.0.82/LICENSE
--rw-r--r--   0        0        0     7455 2023-08-07 02:54:52.915842 zrb-0.0.82/README.md
--rw-r--r--   0        0        0       50 2023-08-04 06:22:49.215485 zrb-0.0.82/docker-template/.dockerignore
--rw-r--r--   0        0        0     2164 2023-08-04 06:22:49.215485 zrb-0.0.82/docker-template/Dockerfile
--rw-r--r--   0        0        0      299 2023-08-04 06:22:49.215485 zrb-0.0.82/docker-template/docker-compose.yml
--rw-r--r--   0        0        0      311 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/README.md
--rw-r--r--   0        0        0      144 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/README.md
--rw-r--r--   0        0        0    13969 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/tasks/README.md
--rw-r--r--   0        0        0     1729 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/tasks/checkers.md
--rw-r--r--   0        0        0     3646 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/tasks/cmd-task.md
--rw-r--r--   0        0        0     4003 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/tasks/docker-compose-task.md
--rw-r--r--   0        0        0     1400 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/tasks/flow-task.md
--rw-r--r--   0        0        0     4132 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/tasks/python-task.md
--rw-r--r--   0        0        0     2732 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/tasks/resource-maker.md
--rw-r--r--   0        0        0     3267 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/concepts/template.md
--rw-r--r--   0        0        0     2106 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/configurations.md
--rw-r--r--   0        0        0      268 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/faq.md
--rw-r--r--   0        0        0      600 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/for-contributors.md
--rw-r--r--   0        0        0      852 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/for-maintainers.md
--rw-r--r--   0        0        0    19584 2023-08-07 02:54:52.915842 zrb-0.0.82/docs/getting-started.md
--rw-r--r--   0        0        0     1084 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/quirks.md
--rw-r--r--   0        0        0      154 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/troubleshooting/README.md
--rw-r--r--   0        0        0      587 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/troubleshooting/enable-shell-completion.md
--rw-r--r--   0        0        0      370 2023-08-07 02:54:52.915842 zrb-0.0.82/docs/tutorials/README.md
--rw-r--r--   0        0        0     1135 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/tutorials/define-task-dynamically.md
--rw-r--r--   0        0        0     8144 2023-08-07 02:54:52.915842 zrb-0.0.82/docs/tutorials/development-to-deployment-low-code.md
--rw-r--r--   0        0        0    85450 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/tutorials/images/enable-kubernetes-on-docker-desktop.png
--rw-r--r--   0        0        0    67958 2023-08-07 02:54:52.915842 zrb-0.0.82/docs/tutorials/images/enable-wsl-integration.png
--rw-r--r--   0        0        0    55320 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/tutorials/images/my-app-list-of-book.png
--rw-r--r--   0        0        0     3521 2023-08-07 02:54:52.915842 zrb-0.0.82/docs/tutorials/preparing-your-machine-for-development.md
--rw-r--r--   0        0        0      599 2023-08-04 06:22:49.215485 zrb-0.0.82/docs/tutorials/run-task-programmatically.md
--rwxr-xr-x   0        0        0   207747 2023-08-04 06:22:49.215485 zrb-0.0.82/images/donator.png
--rw-r--r--   0        0        0      350 2023-08-04 06:22:49.215485 zrb-0.0.82/images/fastapp/about.txt
--rw-r--r--   0        0        0    12221 2023-08-04 06:22:49.215485 zrb-0.0.82/images/fastapp/android-chrome-192x192.png
--rw-r--r--   0        0        0    32285 2023-08-04 06:22:49.215485 zrb-0.0.82/images/fastapp/android-chrome-512x512.png
--rw-r--r--   0        0        0    10805 2023-08-04 06:22:49.215485 zrb-0.0.82/images/fastapp/apple-touch-icon.png
--rw-r--r--   0        0        0      632 2023-08-04 06:22:49.215485 zrb-0.0.82/images/fastapp/favicon-16x16.png
--rw-r--r--   0        0        0     1321 2023-08-04 06:22:49.215485 zrb-0.0.82/images/fastapp/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-08-04 06:22:49.215485 zrb-0.0.82/images/fastapp/favicon.ico
--rw-r--r--   0        0        0      263 2023-08-04 06:22:49.215485 zrb-0.0.82/images/fastapp/site.webmanifest
--rwxr-xr-x   0        0        0    45125 2023-08-04 06:22:49.215485 zrb-0.0.82/images/madou-ring-zaruba.jpg
--rw-r--r--   0        0        0      350 2023-08-04 06:22:49.215485 zrb-0.0.82/images/zrb/about.txt
--rw-r--r--   0        0        0    12488 2023-08-04 06:22:49.215485 zrb-0.0.82/images/zrb/android-chrome-192x192.png
--rw-r--r--   0        0        0    32712 2023-08-04 06:22:49.215485 zrb-0.0.82/images/zrb/android-chrome-512x512.png
--rw-r--r--   0        0        0    11303 2023-08-04 06:22:49.215485 zrb-0.0.82/images/zrb/apple-touch-icon.png
--rw-r--r--   0        0        0      704 2023-08-04 06:22:49.215485 zrb-0.0.82/images/zrb/favicon-16x16.png
--rw-r--r--   0        0        0     1456 2023-08-04 06:22:49.215485 zrb-0.0.82/images/zrb/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-08-04 06:22:49.225486 zrb-0.0.82/images/zrb/favicon.ico
--rw-r--r--   0        0        0      263 2023-08-04 06:22:49.225486 zrb-0.0.82/images/zrb/site.webmanifest
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/playground-template/__init__.py
--rwxr-xr-x   0        0        0     1441 2023-08-04 06:22:49.225486 zrb-0.0.82/playground-template/generate-project.sh
--rw-r--r--   0        0        0      415 2023-08-04 06:22:49.225486 zrb-0.0.82/playground-template/programmatic.py
--rw-r--r--   0        0        0     3745 2023-08-04 06:22:49.225486 zrb-0.0.82/playground-template/zrb_init.py
--rwxr-xr-x   0        0        0     1606 2023-08-07 02:54:52.915842 zrb-0.0.82/project.sh
--rw-r--r--   0        0        0     1102 2023-08-07 02:54:52.915842 zrb-0.0.82/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-08-04 06:22:49.225486 zrb-0.0.82/requirements.txt
--rw-r--r--   0        0        0     1509 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/__init__.py
--rw-r--r--   0        0        0      302 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/__main__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/action/__init__.py
--rw-r--r--   0        0        0     3943 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/action/runner.py
--rw-r--r--   0        0        0      501 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/advertisement.py
--rw-r--r--   0        0        0     1248 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/__init__.py
--rw-r--r--   0        0        0     1113 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/_group.py
--rw-r--r--   0        0        0     1291 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/base64.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/__init__.py
--rw-r--r--   0        0        0      329 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/aws/install.sh
--rw-r--r--   0        0        0    11504 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/devtool/devtool_install.py
--rw-r--r--   0        0        0      295 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/docker/install.sh
--rw-r--r--   0        0        0      432 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/gcloud/install.sh
--rw-r--r--   0        0        0      198 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/gvm/download.sh
--rw-r--r--   0        0        0      518 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/devtool/gvm/finalize.sh
--rw-r--r--   0        0        0      110 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/gvm/resource/config.sh
--rw-r--r--   0        0        0      224 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/devtool/helm/install.sh
--rw-r--r--   0        0        0      264 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/kubectl/install.sh
--rw-r--r--   0        0        0      184 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/nvm/download.sh
--rw-r--r--   0        0        0      555 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/devtool/nvm/finalize.sh
--rw-r--r--   0        0        0      180 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/nvm/resource/config.sh
--rw-r--r--   0        0        0      154 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/pulumi/install.sh
--rw-r--r--   0        0        0       79 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/pulumi/resource/config.sh
--rw-r--r--   0        0        0      140 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/pyenv/download.sh
--rw-r--r--   0        0        0      587 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/devtool/pyenv/finalize.sh
--rw-r--r--   0        0        0      145 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/pyenv/resource/config.sh
--rw-r--r--   0        0        0      152 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/sdkman/download.sh
--rw-r--r--   0        0        0      343 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/devtool/sdkman/finalize.sh
--rw-r--r--   0        0        0      173 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/sdkman/resource/config.sh
--rw-r--r--   0        0        0      295 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/terraform/install.sh
--rw-r--r--   0        0        0       84 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/terraform/resource/config.sh
--rw-r--r--   0        0        0      246 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/tmux/install.sh
--rw-r--r--   0        0        0      416 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/tmux/resource/config.sh
--rw-r--r--   0        0        0      438 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/devtool/zsh/install.sh
--rw-r--r--   0        0        0     4736 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/devtool/zsh/resource/config.sh
--rw-r--r--   0        0        0      990 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/env.py
--rw-r--r--   0        0        0      728 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/eval.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/_common/__init__.py
--rw-r--r--   0        0        0     2753 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/_common/helper.py
--rw-r--r--   0        0        0     2479 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/_common/input.py
--rw-r--r--   0        0        0      309 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/_common/lock.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/cmd_task/__init__.py
--rw-r--r--   0        0        0     1904 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/cmd_task/add.py
--rw-r--r--   0        0        0      473 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/cmd_task/template/_automate/snake_task_name.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/__init__.py
--rw-r--r--   0        0        0     2683 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/add.py
--rw-r--r--   0        0        0     1342 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/template/_automate/snake_task_name.py
--rw-r--r--   0        0        0       12 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-task-name/.dockerignore
--rw-r--r--   0        0        0       30 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-task-name/.gitignore
--rw-r--r--   0        0        0       72 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-task-name/docker-compose.env
--rw-r--r--   0        0        0      585 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-task-name/docker-compose.yml
--rw-r--r--   0        0        0      188 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-task-name/image/Dockerfile
--rw-r--r--   0        0        0      447 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-task-name/image/main.py
--rw-r--r--   0        0        0       15 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/docker_compose_task/template/src/kebab-task-name/image/requirements.txt
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/__init__.py
--rw-r--r--   0        0        0     6826 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/add.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/__init__.py
--rw-r--r--   0        0        0     5517 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/_common.py
--rw-r--r--   0        0        0      155 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/cmd/build-frontend.sh
--rw-r--r--   0        0        0      413 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/cmd/load-test.sh
--rw-r--r--   0        0        0      223 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/cmd/prepare-backend.sh
--rw-r--r--   0        0        0      223 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/cmd/prepare-load-test.sh
--rw-r--r--   0        0        0      148 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/cmd/pulumi-destroy.sh
--rw-r--r--   0        0        0      143 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/cmd/pulumi-up.sh
--rw-r--r--   0        0        0      113 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/cmd/start.sh
--rw-r--r--   0        0        0      237 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/cmd/test.sh
--rw-r--r--   0        0        0       15 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/config/modules.json
--rw-r--r--   0        0        0     5732 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/container.py
--rw-r--r--   0        0        0     3988 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/deployment.py
--rw-r--r--   0        0        0     1759 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/frontend.py
--rw-r--r--   0        0        0     2022 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/image.py
--rw-r--r--   0        0        0     2916 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/load_test.py
--rw-r--r--   0        0        0     6526 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/local.py
--rw-r--r--   0        0        0     3590 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/local_microservices.py
--rw-r--r--   0        0        0     2276 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/_automate/snake_app_name/test.py
--rw-r--r--   0        0        0       53 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/.gitignore
--rw-r--r--   0        0        0     9930 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/README.md
--rw-r--r--   0        0        0       56 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/all-module-disabled.env
--rw-r--r--   0        0        0       54 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/all-module-enabled.env
--rw-r--r--   0        0        0       12 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/.gitignore
--rw-r--r--   0        0        0      133 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/Pulumi.yaml
--rw-r--r--   0        0        0      999 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/README.md
--rw-r--r--   0        0        0     1498 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/__main__.py
--rw-r--r--   0        0        0     4935 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/_common.py
--rw-r--r--   0        0        0     6182 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/app_helper.py
--rw-r--r--   0        0        0      333 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/.helmignore
--rw-r--r--   0        0        0      219 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/Chart.lock
--rw-r--r--   0        0        0      866 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/Chart.yaml
--rw-r--r--   0        0        0   102970 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/README.md
--rw-r--r--   0        0        0      342 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/.helmignore
--rw-r--r--   0        0        0      590 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/Chart.yaml
--rw-r--r--   0        0        0     6939 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/README.md
--rw-r--r--   0        0        0     3723 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     4780 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1633 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     2573 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2361 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0      586 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2427 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     7323 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      628 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0      391 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2064 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      580 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2574 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     3989 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4379 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     3933 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5021 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3264 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2456 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      118 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/charts/common/values.yaml
--rw-r--r--   0        0        0     5816 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/NOTES.txt
--rw-r--r--   0        0        0    13878 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/_helpers.tpl
--rw-r--r--   0        0        0      117 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/extra-list.yaml
--rw-r--r--   0        0        0     1341 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/networkpolicy-egress.yaml
--rw-r--r--   0        0        0     1072 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/configmap.yaml
--rw-r--r--   0        0        0      842 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/extended-configmap.yaml
--rw-r--r--   0        0        0      782 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/initialization-configmap.yaml
--rw-r--r--   0        0        0      717 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-configmap.yaml
--rw-r--r--   0        0        0     1359 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/metrics-svc.yaml
--rw-r--r--   0        0        0     3347 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/networkpolicy.yaml
--rw-r--r--   0        0        0     2390 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/servicemonitor.yaml
--rw-r--r--   0        0        0    34938 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/statefulset.yaml
--rw-r--r--   0        0        0     1764 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/svc-headless.yaml
--rw-r--r--   0        0        0     2811 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/primary/svc.yaml
--rw-r--r--   0        0        0     1126 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1162 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/psp.yaml
--rw-r--r--   0        0        0      853 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/read/extended-configmap.yaml
--rw-r--r--   0        0        0      761 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/read/metrics-configmap.yaml
--rw-r--r--   0        0        0     1409 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/read/metrics-svc.yaml
--rw-r--r--   0        0        0     2225 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/read/networkpolicy.yaml
--rw-r--r--   0        0        0     2444 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/read/servicemonitor.yaml
--rw-r--r--   0        0        0    30413 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/read/statefulset.yaml
--rw-r--r--   0        0        0     1847 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/read/svc-headless.yaml
--rw-r--r--   0        0        0     3014 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/read/svc.yaml
--rw-r--r--   0        0        0     1172 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/role.yaml
--rw-r--r--   0        0        0      873 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/rolebinding.yaml
--rw-r--r--   0        0        0     4993 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/secrets.yaml
--rw-r--r--   0        0        0      875 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1984 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/templates/tls-secrets.yaml
--rw-r--r--   0        0        0     4571 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/values.schema.json
--rw-r--r--   0        0        0    63783 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/postgresql/values.yaml
--rw-r--r--   0        0        0      333 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/.helmignore
--rw-r--r--   0        0        0      219 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/Chart.lock
--rw-r--r--   0        0        0      796 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/Chart.yaml
--rw-r--r--   0        0        0    84509 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/README.md
--rw-r--r--   0        0        0      342 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/.helmignore
--rw-r--r--   0        0        0      590 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/Chart.yaml
--rw-r--r--   0        0        0     6939 2023-08-04 06:22:49.225486 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/README.md
--rw-r--r--   0        0        0     3723 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     4780 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1633 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     2573 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2361 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0      586 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2427 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     7323 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      628 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0      391 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2064 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      580 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2574 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     3989 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4379 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     3933 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5021 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3264 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2456 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      118 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/charts/common/values.yaml
--rw-r--r--   0        0        0     7239 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/NOTES.txt
--rw-r--r--   0        0        0     9924 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/_helpers.tpl
--rw-r--r--   0        0        0     1084 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/config-secret.yaml
--rw-r--r--   0        0        0      117 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/extra-list.yaml
--rw-r--r--   0        0        0     3242 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/ingress.yaml
--rw-r--r--   0        0        0      723 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/init-configmap.yaml
--rw-r--r--   0        0        0     1704 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/networkpolicy.yaml
--rw-r--r--   0        0        0      940 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/pdb.yaml
--rw-r--r--   0        0        0     1144 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/prometheusrule.yaml
--rw-r--r--   0        0        0      806 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/role.yaml
--rw-r--r--   0        0        0      900 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/rolebinding.yaml
--rw-r--r--   0        0        0     3239 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/secrets.yaml
--rw-r--r--   0        0        0     1036 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     3033 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/servicemonitor.yaml
--rw-r--r--   0        0        0    22865 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/statefulset.yaml
--rw-r--r--   0        0        0     2067 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/svc-headless.yaml
--rw-r--r--   0        0        0     5247 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/svc.yaml
--rw-r--r--   0        0        0     4058 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/tls-secrets.yaml
--rw-r--r--   0        0        0       44 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/templates/validation.yaml
--rw-r--r--   0        0        0     2815 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/values.schema.json
--rw-r--r--   0        0        0    58803 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/rabbitmq/values.yaml
--rw-r--r--   0        0        0      366 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/.helmignore
--rw-r--r--   0        0        0      218 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/Chart.lock
--rw-r--r--   0        0        0      916 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/Chart.yaml
--rw-r--r--   0        0        0    11357 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/LICENSE
--rw-r--r--   0        0        0     3330 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/README.md
--rw-r--r--   0        0        0      349 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/.helmignore
--rw-r--r--   0        0        0      725 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/Chart.yaml
--rw-r--r--   0        0        0      478 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/README.md
--rw-r--r--   0        0        0     2331 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/examples/console-enterprise.yaml
--rw-r--r--   0        0        0     1747 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/NOTES.txt
--rw-r--r--   0        0        0     3139 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/_helpers.tpl
--rw-r--r--   0        0        0      615 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/configmap.yaml
--rw-r--r--   0        0        0    10535 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/deployment.yaml
--rw-r--r--   0        0        0      916 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/hpa.yaml
--rw-r--r--   0        0        0     2079 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/ingress.yaml
--rw-r--r--   0        0        0     2808 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/secret.yaml
--rw-r--r--   0        0        0      490 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/service.yaml
--rw-r--r--   0        0        0      320 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      379 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0     8040 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/values.schema.json
--rw-r--r--   0        0        0     5180 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/charts/console/values.yaml
--rw-r--r--   0        0        0      832 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/01-default-values.yaml
--rw-r--r--   0        0        0      970 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/02-one-node-cluster-no-tls-no-sasl-values.yaml
--rw-r--r--   0        0        0      908 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/03-one-node-cluster-tls-no-sasl-values.yaml
--rw-r--r--   0        0        0      994 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/04-one-node-cluster-no-tls-sasl-values.yaml
--rw-r--r--   0        0        0      936 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/05-one-node-cluster-tls-sasl-values.yaml
--rw-r--r--   0        0        0      868 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/06-rack-awareness-values.yaml
--rw-r--r--   0        0        0     1850 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/07-multiple-listeners-values.yaml
--rw-r--r--   0        0        0     1099 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/08-custom-podantiaffinity-values.yaml
--rw-r--r--   0        0        0      978 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/ci/09-initcontainers-resources-values.yaml
--rw-r--r--   0        0        0      147 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/cr.yaml
--rw-r--r--   0        0        0     2758 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/NOTES.txt
--rw-r--r--   0        0        0     3235 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/_example-commands.tpl
--rw-r--r--   0        0        0    23263 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/_helpers.tpl
--rw-r--r--   0        0        0     2543 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/_statefulset.tpl
--rw-r--r--   0        0        0      353 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2595 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/cert-issuers.yaml
--rw-r--r--   0        0        0     2927 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/certs.yaml
--rw-r--r--   0        0        0    14325 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/configmap.yaml
--rw-r--r--   0        0        0     2790 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/console/configmap.yaml
--rw-r--r--   0        0        0     5405 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/console/deployment.yaml
--rw-r--r--   0        0        0     1643 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/poddisruptionbudget.yaml
--rw-r--r--   0        0        0     6672 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/post-install-upgrade-job.yaml
--rw-r--r--   0        0        0     5041 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/post-upgrade.yaml
--rw-r--r--   0        0        0     2983 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/rbac.yaml
--rw-r--r--   0        0        0     5137 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/secrets.yaml
--rw-r--r--   0        0        0     1336 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/service.internal.yaml
--rw-r--r--   0        0        0     3442 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/service.loadbalancer.yaml
--rw-r--r--   0        0        0     1151 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     3038 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/services.nodeport.yaml
--rw-r--r--   0        0        0    24004 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/statefulset.yaml
--rw-r--r--   0        0        0     1998 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-api-status.yaml
--rw-r--r--   0        0        0     2937 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-internal-tls-status.yaml
--rw-r--r--   0        0        0     3504 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-produce-consume.yaml
--rw-r--r--   0        0        0     3525 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-kafka-sasl-status.yaml
--rw-r--r--   0        0        0     2739 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-internal-tls-status.yaml
--rw-r--r--   0        0        0     1701 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-pandaproxy-status.yaml
--rw-r--r--   0        0        0     1910 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-rack-awareness.yaml
--rw-r--r--   0        0        0     3889 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-rpk-debug-bundle.yaml
--rw-r--r--   0        0        0     2701 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-internal-tls-status.yaml
--rw-r--r--   0        0        0     1715 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/templates/tests/test-schemaregistry-status.yaml
--rw-r--r--   0        0        0    26989 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/values.schema.json
--rw-r--r--   0        0        0    46235 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/redpanda/values.yaml
--rw-r--r--   0        0        0      632 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/Chart.lock
--rw-r--r--   0        0        0     1334 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/Chart.yaml
--rw-r--r--   0        0        0    29736 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/README.md
--rw-r--r--   0        0        0      816 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/Chart.yaml
--rw-r--r--   0        0        0    17134 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/README.md
--rw-r--r--   0        0        0      593 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/NOTES.txt
--rw-r--r--   0        0        0     5361 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/_helpers.tpl
--rw-r--r--   0        0        0     3837 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-deployment.yaml
--rw-r--r--   0        0        0      634 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrole.yaml
--rw-r--r--   0        0        0      760 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp-clusterrolebinding.yaml
--rw-r--r--   0        0        0     1440 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-psp.yaml
--rw-r--r--   0        0        0     3748 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-rbac.yaml
--rw-r--r--   0        0        0      949 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/cainjector-serviceaccount.yaml
--rw-r--r--   0        0        0   374997 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/crds.yaml
--rw-r--r--   0        0        0     5687 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/deployment.yaml
--rw-r--r--   0        0        0      594 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrole.yaml
--rw-r--r--   0        0        0      722 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp-clusterrolebinding.yaml
--rw-r--r--   0        0        0     1398 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/psp.yaml
--rw-r--r--   0        0        0    19514 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/rbac.yaml
--rw-r--r--   0        0        0      972 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/service.yaml
--rw-r--r--   0        0        0      863 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1591 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/servicemonitor.yaml
--rw-r--r--   0        0        0     2845 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-job.yaml
--rw-r--r--   0        0        0      779 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrole.yaml
--rw-r--r--   0        0        0      910 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp-clusterrolebinding.yaml
--rw-r--r--   0        0        0     1520 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-psp.yaml
--rw-r--r--   0        0        0     1642 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-rbac.yaml
--rw-r--r--   0        0        0      994 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/startupapicheck-serviceaccount.yaml
--rw-r--r--   0        0        0      746 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-config.yaml
--rw-r--r--   0        0        0     6309 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-deployment.yaml
--rw-r--r--   0        0        0     1657 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-mutating-webhook.yaml
--rw-r--r--   0        0        0      572 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrole.yaml
--rw-r--r--   0        0        0      694 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp-clusterrolebinding.yaml
--rw-r--r--   0        0        0     1558 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-psp.yaml
--rw-r--r--   0        0        0     2641 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-rbac.yaml
--rw-r--r--   0        0        0      954 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-service.yaml
--rw-r--r--   0        0        0      877 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-serviceaccount.yaml
--rw-r--r--   0        0        0     1874 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/templates/webhook-validating-webhook.yaml
--rw-r--r--   0        0        0    17877 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/cert-manager/values.yaml
--rw-r--r--   0        0        0      349 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/.helmignore
--rw-r--r--   0        0        0      234 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/Chart.lock
--rw-r--r--   0        0        0      614 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/Chart.yaml
--rw-r--r--   0        0        0      333 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/.helmignore
--rw-r--r--   0        0        0      225 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/Chart.lock
--rw-r--r--   0        0        0      673 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/Chart.yaml
--rw-r--r--   0        0        0    60071 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/README.md
--rw-r--r--   0        0        0      342 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/.helmignore
--rw-r--r--   0        0        0      529 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/Chart.yaml
--rw-r--r--   0        0        0     7114 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/README.md
--rw-r--r--   0        0        0     3723 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     5472 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1633 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     2587 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2361 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0      586 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2427 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     7323 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      628 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0      391 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2064 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      580 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2574 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     3989 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4379 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     3933 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5021 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3264 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2456 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      118 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/charts/common/values.yaml
--rw-r--r--   0        0        0     3774 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/NOTES.txt
--rw-r--r--   0        0        0    12157 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/_helpers.tpl
--rw-r--r--   0        0        0      726 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/configmap.yaml
--rw-r--r--   0        0        0      117 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/extra-list.yaml
--rw-r--r--   0        0        0     1180 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/metrics-svc.yaml
--rw-r--r--   0        0        0     1606 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/networkpolicy.yaml
--rw-r--r--   0        0        0     1096 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/pdb.yaml
--rw-r--r--   0        0        0     1211 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     5313 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/scripts-configmap.yaml
--rw-r--r--   0        0        0     4077 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/secrets.yaml
--rw-r--r--   0        0        0      944 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     2516 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/servicemonitor.yaml
--rw-r--r--   0        0        0    28701 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/statefulset.yaml
--rw-r--r--   0        0        0     1747 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc-headless.yaml
--rw-r--r--   0        0        0     3297 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/svc.yaml
--rw-r--r--   0        0        0     3656 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/templates/tls-secrets.yaml
--rw-r--r--   0        0        0    36148 2023-08-04 06:22:49.235488 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/charts/zookeeper/values.yaml
--rw-r--r--   0        0        0    77365 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallations.clickhouse.altinity.com.yaml
--rw-r--r--   0        0        0    77423 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseinstallationtemplates.clickhouse.altinity.com.yaml
--rw-r--r--   0        0        0    20500 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/crds/clickhouseoperatorconfigurations.clickhouse.altinity.com.yaml
--rw-r--r--   0        0        0    10595 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/_helper.tpl
--rw-r--r--   0        0        0    10738 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/clickhouse-instance.yaml
--rw-r--r--   0        0        0      924 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/configmap.yaml
--rw-r--r--   0        0        0      421 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/serviceaccount.yaml
--rw-r--r--   0        0        0      664 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-instance/storage-class.yaml
--rw-r--r--   0        0        0      333 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-confd-files.yaml
--rw-r--r--   0        0        0     2761 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-configd-files.yaml
--rw-r--r--   0        0        0    11736 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-files.yaml
--rw-r--r--   0        0        0     2694 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-templatesd-files.yaml
--rw-r--r--   0        0        0     1681 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/configmaps/etc-usersd-files.yaml
--rw-r--r--   0        0        0     5371 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/deployment.yaml
--rw-r--r--   0        0        0      173 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/namespace.yaml
--rw-r--r--   0        0        0     2638 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/role.yaml
--rw-r--r--   0        0        0      701 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/rolebinding.yaml
--rw-r--r--   0        0        0      419 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/secret.yaml
--rw-r--r--   0        0        0      600 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/service.yaml
--rw-r--r--   0        0        0      482 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/templates/clickhouse-operator/serviceaccount.yaml
--rw-r--r--   0        0        0    17891 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/clickhouse/values.yaml
--rw-r--r--   0        0        0      342 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/.helmignore
--rw-r--r--   0        0        0    24586 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/CHANGELOG.md
--rw-r--r--   0        0        0     1007 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/Chart.yaml
--rw-r--r--   0        0        0      213 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/OWNERS
--rw-r--r--   0        0        0    36385 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md
--rw-r--r--   0        0        0    10571 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/README.md.gotmpl
--rw-r--r--   0        0        0      171 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/controller-custom-ingressclass-flags.yaml
--rw-r--r--   0        0        0      267 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-customconfig-values.yaml
--rw-r--r--   0        0        0      337 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-customnodeport-values.yaml
--rw-r--r--   0        0        0      198 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-extra-modules.yaml
--rw-r--r--   0        0        0      280 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-headers-values.yaml
--rw-r--r--   0        0        0      315 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-internal-lb-values.yaml
--rw-r--r--   0        0        0      191 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-nodeport-values.yaml
--rw-r--r--   0        0        0      368 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-podannotations-values.yaml
--rw-r--r--   0        0        0      338 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-configMapNamespace-values.yaml
--rw-r--r--   0        0        0      284 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-portNamePrefix-values.yaml
--rw-r--r--   0        0        0      260 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-udp-values.yaml
--rw-r--r--   0        0        0      254 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/daemonset-tcp-values.yaml
--rw-r--r--   0        0        0      192 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-default-values.yaml
--rw-r--r--   0        0        0      221 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-metrics-values.yaml
--rw-r--r--   0        0        0      228 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-psp-values.yaml
--rw-r--r--   0        0        0      227 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-webhook-and-psp-values.yaml
--rw-r--r--   0        0        0      191 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deamonset-webhook-values.yaml
--rw-r--r--   0        0        0      274 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-autoscaling-behavior-values.yaml
--rw-r--r--   0        0        0      207 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-autoscaling-values.yaml
--rw-r--r--   0        0        0      248 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-customconfig-values.yaml
--rw-r--r--   0        0        0      318 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-customnodeport-values.yaml
--rw-r--r--   0        0        0      170 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-default-values.yaml
--rw-r--r--   0        0        0      197 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-extra-modules.yaml
--rw-r--r--   0        0        0      262 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-headers-values.yaml
--rw-r--r--   0        0        0      297 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-internal-lb-values.yaml
--rw-r--r--   0        0        0      203 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-metrics-values.yaml
--rw-r--r--   0        0        0      173 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-nodeport-values.yaml
--rw-r--r--   0        0        0      350 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-podannotations-values.yaml
--rw-r--r--   0        0        0      170 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-psp-values.yaml
--rw-r--r--   0        0        0      320 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-configMapNamespace-values.yaml
--rw-r--r--   0        0        0      266 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-portNamePrefix-values.yaml
--rw-r--r--   0        0        0      242 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-udp-values.yaml
--rw-r--r--   0        0        0      196 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-tcp-values.yaml
--rw-r--r--   0        0        0      209 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-and-psp-values.yaml
--rw-r--r--   0        0        0      204 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-extraEnvs-values.yaml
--rw-r--r--   0        0        0      425 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-resources-values.yaml
--rw-r--r--   0        0        0      173 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/ci/deployment-webhook-values.yaml
--rw-r--r--   0        0        0     3498 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/NOTES.txt
--rw-r--r--   0        0        0     5570 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_helpers.tpl
--rw-r--r--   0        0        0     2996 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/_params.tpl
--rw-r--r--   0        0        0     1120 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrole.yaml
--rw-r--r--   0        0        0      913 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/clusterrolebinding.yaml
--rw-r--r--   0        0        0     3740 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-createSecret.yaml
--rw-r--r--   0        0        0     3783 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/job-patchWebhook.yaml
--rw-r--r--   0        0        0     1183 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/psp.yaml
--rw-r--r--   0        0        0      769 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/role.yaml
--rw-r--r--   0        0        0      936 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/rolebinding.yaml
--rw-r--r--   0        0        0      650 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/job-patch/serviceaccount.yaml
--rw-r--r--   0        0        0     1937 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/admission-webhooks/validating-webhook.yaml
--rw-r--r--   0        0        0     1949 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrole.yaml
--rw-r--r--   0        0        0      612 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0      459 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-addheaders.yaml
--rw-r--r--   0        0        0      693 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-proxyheaders.yaml
--rw-r--r--   0        0        0      547 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-tcp.yaml
--rw-r--r--   0        0        0      547 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap-udp.yaml
--rw-r--r--   0        0        0     1162 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-configmap.yaml
--rw-r--r--   0        0        0     9624 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-daemonset.yaml
--rw-r--r--   0        0        0     9990 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-deployment.yaml
--rw-r--r--   0        0        0     1620 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-hpa.yaml
--rw-r--r--   0        0        0      760 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-ingressclass.yaml
--rw-r--r--   0        0        0     1619 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-keda.yaml
--rw-r--r--   0        0        0      877 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-poddisruptionbudget.yaml
--rw-r--r--   0        0        0      961 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-prometheusrules.yaml
--rw-r--r--   0        0        0     2572 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-psp.yaml
--rw-r--r--   0        0        0     2463 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-role.yaml
--rw-r--r--   0        0        0      651 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-rolebinding.yaml
--rw-r--r--   0        0        0     3570 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-internal.yaml
--rw-r--r--   0        0        0     2106 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-metrics.yaml
--rw-r--r--   0        0        0     1670 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service-webhook.yaml
--rw-r--r--   0        0        0     4504 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-service.yaml
--rw-r--r--   0        0        0      623 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-serviceaccount.yaml
--rw-r--r--   0        0        0     2061 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-servicemonitor.yaml
--rw-r--r--   0        0        0      464 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/controller-wehbooks-networkpolicy.yaml
--rw-r--r--   0        0        0     5476 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-deployment.yaml
--rw-r--r--   0        0        0     1143 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-hpa.yaml
--rw-r--r--   0        0        0      864 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-poddisruptionbudget.yaml
--rw-r--r--   0        0        0      925 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-psp.yaml
--rw-r--r--   0        0        0      806 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-role.yaml
--rw-r--r--   0        0        0      760 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-rolebinding.yaml
--rw-r--r--   0        0        0     1562 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-service.yaml
--rw-r--r--   0        0        0      573 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/default-backend-serviceaccount.yaml
--rw-r--r--   0        0        0      233 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/templates/dh-param-secret.yaml
--rw-r--r--   0        0        0    31188 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/ingress-nginx/values.yaml
--rw-r--r--   0        0        0      349 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/.helmignore
--rw-r--r--   0        0        0      555 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/Chart.yaml
--rw-r--r--   0        0        0      276 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/NOTES.txt
--rw-r--r--   0        0        0    14838 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_config.tpl
--rw-r--r--   0        0        0    12133 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/_helpers.tpl
--rw-r--r--   0        0        0      172 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/namespace.yaml
--rw-r--r--   0        0        0      418 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/clusterrole.yaml
--rw-r--r--   0        0        0      509 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/clusterrolebinding.yaml
--rw-r--r--   0        0        0      286 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/configmap.yaml
--rw-r--r--   0        0        0     5976 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/daemonset.yaml
--rw-r--r--   0        0        0      517 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/service.yaml
--rw-r--r--   0        0        0      441 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/serviceaccount.yaml
--rw-r--r--   0        0        0      526 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-agent/tests/test-connection.yaml
--rw-r--r--   0        0        0      438 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/clusterrole.yaml
--rw-r--r--   0        0        0      529 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/clusterrolebinding.yaml
--rw-r--r--   0        0        0      306 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/configmap.yaml
--rw-r--r--   0        0        0     5799 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/deployment.yaml
--rw-r--r--   0        0        0     1778 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/ingress.yaml
--rw-r--r--   0        0        0      539 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/service.yaml
--rw-r--r--   0        0        0      466 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/serviceaccount.yaml
--rw-r--r--   0        0        0      546 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/otel-deployment/tests/test-connection.yaml
--rw-r--r--   0        0        0      573 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/templates/secret.yaml
--rw-r--r--   0        0        0    27461 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/k8s-infra/values.yaml
--rw-r--r--   0        0        0      305 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/Chart.lock
--rw-r--r--   0        0        0      872 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/Chart.yaml
--rw-r--r--   0        0        0    51454 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/README.md
--rw-r--r--   0        0        0      342 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/.helmignore
--rw-r--r--   0        0        0      569 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/Chart.yaml
--rw-r--r--   0        0        0    25039 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/README.md
--rw-r--r--   0        0        0     3502 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     4780 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1633 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     2437 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2314 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0      586 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2461 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     6183 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      628 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0      391 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2049 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      580 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2574 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     3989 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4379 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     3933 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5021 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3264 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2456 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      118 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/common/values.yaml
--rw-r--r--   0        0        0      333 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/.helmignore
--rw-r--r--   0        0        0      219 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/Chart.lock
--rw-r--r--   0        0        0      845 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/Chart.yaml
--rw-r--r--   0        0        0   101381 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/README.md
--rw-r--r--   0        0        0      342 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/.helmignore
--rw-r--r--   0        0        0      569 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/Chart.yaml
--rw-r--r--   0        0        0    25039 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/README.md
--rw-r--r--   0        0        0     3502 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_affinities.tpl
--rw-r--r--   0        0        0     4780 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_capabilities.tpl
--rw-r--r--   0        0        0     1633 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_errors.tpl
--rw-r--r--   0        0        0     2437 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_images.tpl
--rw-r--r--   0        0        0     2314 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_ingress.tpl
--rw-r--r--   0        0        0      586 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_labels.tpl
--rw-r--r--   0        0        0     2461 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_names.tpl
--rw-r--r--   0        0        0     6183 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_secrets.tpl
--rw-r--r--   0        0        0      628 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_storage.tpl
--rw-r--r--   0        0        0      391 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_tplvalues.tpl
--rw-r--r--   0        0        0     2049 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_utils.tpl
--rw-r--r--   0        0        0      580 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/_warnings.tpl
--rw-r--r--   0        0        0     2574 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_cassandra.tpl
--rw-r--r--   0        0        0     3989 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mariadb.tpl
--rw-r--r--   0        0        0     4379 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mongodb.tpl
--rw-r--r--   0        0        0     3933 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_mysql.tpl
--rw-r--r--   0        0        0     5021 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_postgresql.tpl
--rw-r--r--   0        0        0     3264 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_redis.tpl
--rw-r--r--   0        0        0     2456 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/templates/validations/_validations.tpl
--rw-r--r--   0        0        0      118 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/charts/common/values.yaml
--rw-r--r--   0        0        0     5433 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/NOTES.txt
--rw-r--r--   0        0        0    13838 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/_helpers.tpl
--rw-r--r--   0        0        0      117 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/extra-list.yaml
--rw-r--r--   0        0        0     1341 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/networkpolicy-egress.yaml
--rw-r--r--   0        0        0     1072 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/configmap.yaml
--rw-r--r--   0        0        0      842 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/extended-configmap.yaml
--rw-r--r--   0        0        0      782 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/initialization-configmap.yaml
--rw-r--r--   0        0        0      717 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-configmap.yaml
--rw-r--r--   0        0        0     1269 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/metrics-svc.yaml
--rw-r--r--   0        0        0     3347 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/networkpolicy.yaml
--rw-r--r--   0        0        0     2390 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/servicemonitor.yaml
--rw-r--r--   0        0        0    34437 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/statefulset.yaml
--rw-r--r--   0        0        0     1452 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc-headless.yaml
--rw-r--r--   0        0        0     2721 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/primary/svc.yaml
--rw-r--r--   0        0        0     1126 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1162 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/psp.yaml
--rw-r--r--   0        0        0      853 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/extended-configmap.yaml
--rw-r--r--   0        0        0      761 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-configmap.yaml
--rw-r--r--   0        0        0     1319 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/metrics-svc.yaml
--rw-r--r--   0        0        0     2225 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/networkpolicy.yaml
--rw-r--r--   0        0        0     2444 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/servicemonitor.yaml
--rw-r--r--   0        0        0    29932 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/statefulset.yaml
--rw-r--r--   0        0        0     1520 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc-headless.yaml
--rw-r--r--   0        0        0     2919 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/read/svc.yaml
--rw-r--r--   0        0        0     1172 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/role.yaml
--rw-r--r--   0        0        0      873 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/rolebinding.yaml
--rw-r--r--   0        0        0     1769 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/secrets.yaml
--rw-r--r--   0        0        0      875 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     1690 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/templates/tls-secrets.yaml
--rw-r--r--   0        0        0     4571 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.schema.json
--rw-r--r--   0        0        0    63223 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/charts/postgresql/values.yaml
--rw-r--r--   0        0        0     5526 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/NOTES.txt
--rw-r--r--   0        0        0     9090 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/_helpers.tpl
--rw-r--r--   0        0        0     1947 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap-env-vars.yaml
--rw-r--r--   0        0        0      743 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/configmap.yaml
--rw-r--r--   0        0        0      117 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/extra-list.yaml
--rw-r--r--   0        0        0     1160 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/headless-service.yaml
--rw-r--r--   0        0        0     1858 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/hpa.yaml
--rw-r--r--   0        0        0     3152 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/ingress.yaml
--rw-r--r--   0        0        0      802 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/init-scripts-configmap.yaml
--rw-r--r--   0        0        0      850 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-configmap.yaml
--rw-r--r--   0        0        0     7172 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/keycloak-config-cli-job.yaml
--rw-r--r--   0        0        0     1228 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/metrics-service.yaml
--rw-r--r--   0        0        0     1498 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/networkpolicy.yaml
--rw-r--r--   0        0        0     1023 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/pdb.yaml
--rw-r--r--   0        0        0     1129 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/prometheusrule.yaml
--rw-r--r--   0        0        0      950 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/role.yaml
--rw-r--r--   0        0        0      974 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/rolebinding.yaml
--rw-r--r--   0        0        0     1982 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/secrets.yaml
--rw-r--r--   0        0        0     3171 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/service.yaml
--rw-r--r--   0        0        0     1019 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     2655 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/servicemonitor.yaml
--rw-r--r--   0        0        0    20259 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/statefulset.yaml
--rw-r--r--   0        0        0     3273 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/templates/tls-secret.yaml
--rw-r--r--   0        0        0    40146 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/keycloak/values.yaml
--rw-r--r--   0        0        0      368 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/.helmignore
--rw-r--r--   0        0        0      359 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/Chart.yaml
--rw-r--r--   0        0        0     9349 2023-08-04 06:22:49.245489 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/README.md
--rw-r--r--   0        0        0     2668 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/NOTES.txt
--rw-r--r--   0        0        0     3022 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_bucket.txt
--rw-r--r--   0        0        0     2010 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_policy.txt
--rw-r--r--   0        0        0     3087 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_create_user.txt
--rw-r--r--   0        0        0     1473 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_custom_command.txt
--rw-r--r--   0        0        0      469 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helper_policy.tpl
--rw-r--r--   0        0        0     6479 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/_helpers.tpl
--rw-r--r--   0        0        0      887 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/configmap.yaml
--rw-r--r--   0        0        0     1693 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-ingress.yaml
--rw-r--r--   0        0        0     1558 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/console-service.yaml
--rw-r--r--   0        0        0     6682 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/deployment.yaml
--rw-r--r--   0        0        0     6449 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/gateway-deployment.yaml
--rw-r--r--   0        0        0     1594 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/ingress.yaml
--rw-r--r--   0        0        0      812 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/networkpolicy.yaml
--rw-r--r--   0        0        0      371 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/poddisruptionbudget.yaml
--rw-r--r--   0        0        0     3130 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-bucket-job.yaml
--rw-r--r--   0        0        0     3135 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-policy-job.yaml
--rw-r--r--   0        0        0     3460 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-create-user-job.yaml
--rw-r--r--   0        0        0     3190 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/post-install-custom-command.yaml
--rw-r--r--   0        0        0     1059 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/pvc.yaml
--rw-r--r--   0        0        0      752 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/secrets.yaml
--rw-r--r--   0        0        0     1117 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/securitycontextconstraints.yaml
--rw-r--r--   0        0        0     1457 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/service.yaml
--rw-r--r--   0        0        0      195 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/serviceaccount.yaml
--rw-r--r--   0        0        0     2036 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/servicemonitor.yaml
--rw-r--r--   0        0        0     8507 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/templates/statefulset.yaml
--rw-r--r--   0        0        0    13974 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/charts/minio/values.yaml
--rw-r--r--   0        0        0     2317 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/NOTES.txt
--rw-r--r--   0        0        0     7117 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/_clickhouse.tpl
--rw-r--r--   0        0        0    19612 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/_helpers.tpl
--rw-r--r--   0        0        0      426 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/alertmanager/configmap.yaml
--rw-r--r--   0        0        0     1683 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/alertmanager/ingress.yaml
--rw-r--r--   0        0        0      401 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/alertmanager/pdb.yaml
--rw-r--r--   0        0        0      399 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/alertmanager/serviceaccount.yaml
--rw-r--r--   0        0        0     1404 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/alertmanager/services.yaml
--rw-r--r--   0        0        0     8073 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/alertmanager/statefulset.yaml
--rw-r--r--   0        0        0      974 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/cert-issuer.yaml
--rw-r--r--   0        0        0     1533 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/frontend/configmap.yaml
--rw-r--r--   0        0        0     3461 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/frontend/deployment.yaml
--rw-r--r--   0        0        0     1311 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/frontend/hpa.yaml
--rw-r--r--   0        0        0     1647 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/frontend/ingress.yaml
--rw-r--r--   0        0        0     1016 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/frontend/keda-autoscaler.yaml
--rw-r--r--   0        0        0      542 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/frontend/service.yaml
--rw-r--r--   0        0        0      384 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/frontend/serviceaccount.yaml
--rw-r--r--   0        0        0      459 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/frontend/tests/test-connection.yaml
--rw-r--r--   0        0        0      482 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrole.yaml
--rw-r--r--   0        0        0      718 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/clusterrolebinding.yaml
--rw-r--r--   0        0        0      283 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/configmap.yaml
--rw-r--r--   0        0        0     7577 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/deployment.yaml
--rw-r--r--   0        0        0     1755 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/ingress.yaml
--rw-r--r--   0        0        0      519 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/service.yaml
--rw-r--r--   0        0        0      432 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector-metrics/serviceaccount.yaml
--rw-r--r--   0        0        0      429 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/clusterrole.yaml
--rw-r--r--   0        0        0      519 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/clusterrolebinding.yaml
--rw-r--r--   0        0        0      254 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/configmap.yaml
--rw-r--r--   0        0        0     7299 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/deployment.yaml
--rw-r--r--   0        0        0     1361 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/hpa.yaml
--rw-r--r--   0        0        0     1692 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/ingress.yaml
--rw-r--r--   0        0        0     1061 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/keda-autoscaler.yaml
--rw-r--r--   0        0        0      487 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/service.yaml
--rw-r--r--   0        0        0      404 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/otel-collector/serviceaccount.yaml
--rw-r--r--   0        0        0      972 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/query-service/configmap.yaml
--rw-r--r--   0        0        0     1683 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/query-service/ingress.yaml
--rw-r--r--   0        0        0      956 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/query-service/service.yaml
--rw-r--r--   0        0        0      400 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/query-service/serviceaccount.yaml
--rw-r--r--   0        0        0     7195 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/query-service/statefulset.yaml
--rw-r--r--   0        0        0      540 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/query-service/tests/test-connection.yaml
--rw-r--r--   0        0        0      273 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/templates/secrets-clickhouse-external.yaml
--rw-r--r--   0        0        0    84917 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm-charts/signoz/values.yaml
--rw-r--r--   0        0        0     1097 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm_postgresql_helper.py
--rw-r--r--   0        0        0      900 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm_rabbitmq_helper.py
--rw-r--r--   0        0        0     1036 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm_redpanda_helper.py
--rw-r--r--   0        0        0     1033 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/helm_signoz_helper.py
--rw-r--r--   0        0        0       87 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/requirements.txt
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/state/.gitkeep
--rw-r--r--   0        0        0      552 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/deployment/template.env
--rw-r--r--   0        0        0     1132 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/docker-compose.env
--rw-r--r--   0        0        0    14926 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/docker-compose.yml
--rw-r--r--   0        0        0       68 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/docs/README.md
--rw-r--r--   0        0        0     6256 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/docs/modular-monolith/README.md
--rw-r--r--   0        0        0    81204 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/docs/modular-monolith/images/fastapp-microservices.png
--rw-r--r--   0        0        0    41834 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/docs/modular-monolith/images/fastapp-monolith.png
--rw-r--r--   0        0        0    40600 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/docs/modular-monolith/images/fastapp.png
--rw-r--r--   0        0        0       17 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/loadtest/.gitignore
--rw-r--r--   0        0        0      914 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/loadtest/locustfile.py
--rw-r--r--   0        0        0       15 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/loadtest/requirements.txt
--rw-r--r--   0        0        0      107 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/loadtest/template.env
--rw-r--r--   0        0        0     2870 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/clickhouse/clickhouse-cluster.xml
--rw-r--r--   0        0        0    55854 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/clickhouse/clickhouse-config.xml
--rw-r--r--   0        0        0     1754 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/clickhouse/clickhouse-storage.xml
--rw-r--r--   0        0        0     6258 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/clickhouse/clickhouse-users.xml
--rw-r--r--   0        0        0      575 2023-08-04 06:22:49.255491 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/clickhouse/custom-function.xml
--rwxr-xr-x   0        0        0  1849156 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/clickhouse/user_scripts/histogramQuantile
--rw-r--r--   0        0        0     6986 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/clickhouse/user_scripts/histogramQuantile.go
--rw-r--r--   0        0        0     1184 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/frontend/nginx-config.conf
--rw-r--r--   0        0        0     1548 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/otel-collector-metrics/otel-collector-metrics-config.yaml
--rw-r--r--   0        0        0     5856 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/otel-collector/otel-collector-config.yaml
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/query-service/dashboards/.gitkeep
--rw-r--r--   0        0        0        9 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/query-service/data/.gitignore
--rw-r--r--   0        0        0      757 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/monitoring/query-service/prometheus.yml
--rw-r--r--   0        0        0      135 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/.dockerignore
--rw-r--r--   0        0        0       53 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/.gitignore
--rw-r--r--   0        0        0      435 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/Dockerfile
--rwxr-xr-x   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/__init__.py
--rwxr-xr-x   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/__init__.py
--rwxr-xr-x   0        0        0     3182 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/app.py
--rw-r--r--   0        0        0     1364 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/app_lifespan.py
--rw-r--r--   0        0        0      869 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/app_state.py
--rw-r--r--   0        0        0     1039 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/db_connection.py
--rw-r--r--   0        0        0      327 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/frontend_index.py
--rw-r--r--   0        0        0     1874 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/log.py
--rw-r--r--   0        0        0     3436 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/messagebus.py
--rw-r--r--   0        0        0     1380 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/component/rpc.py
--rwxr-xr-x   0        0        0     4477 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/config.py
--rwxr-xr-x   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/__init__.py
--rw-r--r--   0        0        0     1944 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/error.py
--rwxr-xr-x   0        0        0      748 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/kafka/__init__.py
--rw-r--r--   0        0        0     5926 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/kafka/admin.py
--rwxr-xr-x   0        0        0    10924 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/kafka/consumer.py
--rwxr-xr-x   0        0        0     7129 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/kafka/publisher.py
--rwxr-xr-x   0        0        0     1784 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/messagebus.py
--rw-r--r--   0        0        0     1980 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/mock.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/rabbitmq/__init__.py
--rw-r--r--   0        0        0     5149 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/rabbitmq/admin.py
--rwxr-xr-x   0        0        0     7188 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/rabbitmq/consumer.py
--rwxr-xr-x   0        0        0     4919 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/messagebus/rabbitmq/publisher.py
--rw-r--r--   0        0        0       62 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/model/__init__.py
--rw-r--r--   0        0        0     1746 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/model/repo_model.py
--rw-r--r--   0        0        0      238 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/repo/__init__.py
--rw-r--r--   0        0        0      555 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/repo/db_entity_mixin.py
--rw-r--r--   0        0        0     9584 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/repo/db_repo.py
--rw-r--r--   0        0        0      927 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/repo/repo.py
--rw-r--r--   0        0        0      146 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/repo/search_filter.py
--rw-r--r--   0        0        0      229 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/rpc/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/rpc/messagebus/__init__.py
--rw-r--r--   0        0        0     3720 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/rpc/messagebus/caller.py
--rw-r--r--   0        0        0     2218 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/rpc/messagebus/server.py
--rw-r--r--   0        0        0     1741 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/rpc/rpc.py
--rw-r--r--   0        0        0      122 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/schema/__init__.py
--rw-r--r--   0        0        0      313 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/schema/base_schema.py
--rw-r--r--   0        0        0      157 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/serializer/__init__.py
--rw-r--r--   0        0        0      867 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/core/serializer/serializer.py
--rw-r--r--   0        0        0      160 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/.eslintignore
--rw-r--r--   0        0        0      494 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      132 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/.gitignore
--rw-r--r--   0        0        0       19 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/.npmrc
--rw-r--r--   0        0        0      160 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/.prettierignore
--rw-r--r--   0        0        0      233 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/.prettierrc
--rwxr-xr-x   0        0        0      944 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/README.md
--rw-r--r--   0        0        0   125175 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/package-lock.json
--rwxr-xr-x   0        0        0     1362 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/package.json
--rwxr-xr-x   0        0        0      225 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/playwright.config.ts
--rwxr-xr-x   0        0        0       80 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/postcss.config.js
--rwxr-xr-x   0        0        0       58 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/app.css
--rwxr-xr-x   0        0        0      241 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/app.d.ts
--rwxr-xr-x   0        0        0      350 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/app.html
--rwxr-xr-x   0        0        0      148 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/index.test.ts
--rwxr-xr-x   0        0        0   130279 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/assets/logo.png
--rwxr-xr-x   0        0        0     5281 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/auth/helper.ts
--rwxr-xr-x   0        0        0      125 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/auth/store.ts
--rwxr-xr-x   0        0        0      197 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/auth/type.ts
--rw-r--r--   0        0        0      608 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/components/arrayOfObject/arrayOfObjectDiv.svelte
--rw-r--r--   0        0        0      361 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/components/arrayOfObject/arrayOfObjectUl.svelte
--rw-r--r--   0        0        0     1906 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/components/arrayOfObject/input/arrayOfObjectCheckboxes.svelte
--rw-r--r--   0        0        0      281 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/components/json/jsonView.svelte
--rwxr-xr-x   0        0        0     1675 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/components/navigation/Menu.svelte
--rwxr-xr-x   0        0        0     4085 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/components/navigation/Navigation.svelte
--rwxr-xr-x   0        0        0      727 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/components/navigation/helper.ts
--rwxr-xr-x   0        0        0      127 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/components/navigation/type.ts
--rwxr-xr-x   0        0        0     1609 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/config/app.ts
--rwxr-xr-x   0        0        0      648 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/config/navData.ts
--rwxr-xr-x   0        0        0      350 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/lib/error/helper.ts
--rwxr-xr-x   0        0        0      291 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/+error.svelte
--rwxr-xr-x   0        0        0       65 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/+layout.js
--rwxr-xr-x   0        0        0      584 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/+layout.svelte
--rwxr-xr-x   0        0        0      478 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/+page.svelte
--rwxr-xr-x   0        0        0     6285 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/group/+page.svelte
--rwxr-xr-x   0        0        0     3763 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/group/delete/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/group/delete/[id]/+page.ts
--rwxr-xr-x   0        0        0     2968 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/group/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/group/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     4306 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/group/new/+page.svelte
--rw-r--r--   0        0        0     5028 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/group/update/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/group/update/[id]/+page.ts
--rwxr-xr-x   0        0        0     6051 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/permission/+page.svelte
--rwxr-xr-x   0        0        0     3462 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/permission/delete/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/permission/delete/[id]/+page.ts
--rwxr-xr-x   0        0        0     2662 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/permission/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/permission/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     2905 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/permission/new/+page.svelte
--rw-r--r--   0        0        0     3659 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/permission/update/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/permission/update/[id]/+page.ts
--rwxr-xr-x   0        0        0     6622 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/user/+page.svelte
--rwxr-xr-x   0        0        0     4323 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/user/delete/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/user/delete/[id]/+page.ts
--rwxr-xr-x   0        0        0     3529 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/user/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/user/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     6049 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/user/new/+page.svelte
--rw-r--r--   0        0        0     6952 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/user/update/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/auth/user/update/[id]/+page.ts
--rwxr-xr-x   0        0        0     5409 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/log/activity/+page.svelte
--rwxr-xr-x   0        0        0     2941 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/log/activity/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/src/routes/log/activity/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     1321 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/static/favicon.png
--rwxr-xr-x   0        0        0    12221 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/static/logo.png
--rwxr-xr-x   0        0        0      317 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/svelte.config.js
--rwxr-xr-x   0        0        0      203 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/tailwind.config.js
--rwxr-xr-x   0        0        0      224 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/tests/test.ts
--rwxr-xr-x   0        0        0      532 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/tsconfig.json
--rwxr-xr-x   0        0        0      210 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/frontend/vite.config.ts
--rwxr-xr-x   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/helper/__init__.py
--rw-r--r--   0        0        0      499 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/helper/async_task.py
--rwxr-xr-x   0        0        0      763 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/helper/conversion.py
--rw-r--r--   0        0        0     1902 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/helper/migration.py
--rw-r--r--   0        0        0      103 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/helper/value.py
--rwxr-xr-x   0        0        0      278 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/main.py
--rw-r--r--   0        0        0      231 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/migrate.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/__init__.py
--rw-r--r--   0        0        0      950 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/api.py
--rw-r--r--   0        0        0      769 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/__init__.py
--rw-r--r--   0        0        0      527 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/access_token_scheme.py
--rw-r--r--   0        0        0      549 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/access_token_util.py
--rw-r--r--   0        0        0      308 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/authorizer.py
--rw-r--r--   0        0        0       83 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/base.py
--rw-r--r--   0        0        0      155 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/bearer_token_scheme.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/model/__init__.py
--rw-r--r--   0        0        0      219 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/model/group_model.py
--rw-r--r--   0        0        0      259 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/model/permission_model.py
--rw-r--r--   0        0        0     1003 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/model/user_model.py
--rw-r--r--   0        0        0      124 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/password_hasher.py
--rw-r--r--   0        0        0      557 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/refresh_token_util.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/repo/__init__.py
--rw-r--r--   0        0        0      223 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/repo/group_repo.py
--rw-r--r--   0        0        0      252 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/repo/permission_repo.py
--rw-r--r--   0        0        0      315 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/repo/user_repo.py
--rw-r--r--   0        0        0      782 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/component/user.py
--rw-r--r--   0        0        0      869 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/access_token/_init_.py
--rw-r--r--   0        0        0     1252 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/access_token/scheme.py
--rw-r--r--   0        0        0     2183 2023-08-04 06:22:49.265492 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/access_token/util.py
--rw-r--r--   0        0        0      368 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/authorizer/authorizer.py
--rw-r--r--   0        0        0     1226 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/authorizer/rpc_authorizer.py
--rw-r--r--   0        0        0      486 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/password_hasher/bcrypt_password_hasher.py
--rw-r--r--   0        0        0      259 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/password_hasher/password_hasher.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/refresh_token/_init_.py
--rw-r--r--   0        0        0     1706 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/core/refresh_token/util.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/group/__init__.py
--rw-r--r--   0        0        0     4154 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/group/api.py
--rw-r--r--   0        0        0      289 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/group/model.py
--rw-r--r--   0        0        0     1225 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/group/repo.py
--rw-r--r--   0        0        0     2421 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/group/rpc.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/permission/__init__.py
--rw-r--r--   0        0        0     4341 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/permission/api.py
--rw-r--r--   0        0        0      903 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/permission/model.py
--rw-r--r--   0        0        0     1082 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/permission/repo.py
--rw-r--r--   0        0        0     2666 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/permission/rpc.py
--rw-r--r--   0        0        0      659 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/table.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/user/__init__.py
--rw-r--r--   0        0        0     6533 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/user/api.py
--rw-r--r--   0        0        0     6924 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/user/model.py
--rw-r--r--   0        0        0     3155 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/user/repo.py
--rw-r--r--   0        0        0     3726 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/entity/user/rpc.py
--rw-r--r--   0        0        0      280 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/event.py
--rw-r--r--   0        0        0      578 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/migrate.py
--rw-r--r--   0        0        0     1169 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/register_module.py
--rw-r--r--   0        0        0     1350 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/register_permission.py
--rw-r--r--   0        0        0      736 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/rpc.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/schema/__init__.py
--rw-r--r--   0        0        0      448 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/schema/group.py
--rw-r--r--   0        0        0      324 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/schema/permission.py
--rw-r--r--   0        0        0      189 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/schema/request.py
--rw-r--r--   0        0        0      303 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/schema/token.py
--rw-r--r--   0        0        0      684 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/auth/schema/user.py
--rw-r--r--   0        0        0      509 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/api.py
--rw-r--r--   0        0        0       56 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/component/__init__.py
--rw-r--r--   0        0        0       83 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/component/base.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/component/model/__init__.py
--rw-r--r--   0        0        0      209 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/component/model/activity_model.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/component/repo/__init__.py
--rw-r--r--   0        0        0      239 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/component/repo/activity_repo.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/core/__init__.py
--rw-r--r--   0        0        0     1584 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/core/historical_repo_model.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/entity/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/entity/activity/__init__.py
--rw-r--r--   0        0        0     2116 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/entity/activity/api.py
--rw-r--r--   0        0        0      610 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/entity/activity/event.py
--rw-r--r--   0        0        0      238 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/entity/activity/model.py
--rw-r--r--   0        0        0      578 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/entity/activity/repo.py
--rw-r--r--   0        0        0     2438 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/entity/activity/rpc.py
--rw-r--r--   0        0        0      550 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/entity/table.py
--rw-r--r--   0        0        0      443 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/event.py
--rw-r--r--   0        0        0      431 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/migrate.py
--rw-r--r--   0        0        0     1162 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/register_module.py
--rw-r--r--   0        0        0      446 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/rpc.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/schema/__init__.py
--rw-r--r--   0        0        0      325 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/module/log/schema/activity.py
--rw-r--r--   0        0        0      462 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/requirements.txt
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/schema/__init__.py
--rw-r--r--   0        0        0      163 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/schema/frontend_config.py
--rwxr-xr-x   0        0        0     1691 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/start.sh
--rw-r--r--   0        0        0     1591 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/src/template.env
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/auth/__init__.py
--rw-r--r--   0        0        0     8136 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/auth/test_group_crud.py
--rw-r--r--   0        0        0     8194 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/auth/test_permission_crud.py
--rw-r--r--   0        0        0     8417 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/auth/test_user_crud.py
--rw-r--r--   0        0        0     8936 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/auth/test_user_login.py
--rw-r--r--   0        0        0      314 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/conftest.py
--rw-r--r--   0        0        0      278 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/helper.py
--rw-r--r--   0        0        0     1243 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp/template/src/kebab-app-name/test/test_liveness_and_readiness.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/__init__.py
--rw-r--r--   0        0        0     8704 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/add.py
--rw-r--r--   0        0        0     1212 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/add_navigation.py
--rw-r--r--   0        0        0       13 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/.gitignore
--rw-r--r--   0        0        0    11261 2023-08-04 06:57:19.085172 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/package-lock.json
--rw-r--r--   0        0        0      369 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/package.json
--rw-r--r--   0        0        0     1460 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/src/addNav.ts
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/src/fastapp/src/frontend/src/lib/config/navData.ts
--rw-r--r--   0        0        0    12289 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/nodejs/codemod/tsconfig.json
--rwxr-xr-x   0        0        0     6244 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/frontend/src/routes/kebab-module-name/kebab-entity-name/+page.svelte
--rwxr-xr-x   0        0        0     3461 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/frontend/src/routes/kebab-module-name/kebab-entity-name/delete/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/frontend/src/routes/kebab-module-name/kebab-entity-name/delete/[id]/+page.ts
--rwxr-xr-x   0        0        0     2635 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/frontend/src/routes/kebab-module-name/kebab-entity-name/detail/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/frontend/src/routes/kebab-module-name/kebab-entity-name/detail/[id]/+page.ts
--rwxr-xr-x   0        0        0     2855 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/frontend/src/routes/kebab-module-name/kebab-entity-name/new/+page.svelte
--rw-r--r--   0        0        0     3613 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/frontend/src/routes/kebab-module-name/kebab-entity-name/update/[id]/+page.svelte
--rw-r--r--   0        0        0       85 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/frontend/src/routes/kebab-module-name/kebab-entity-name/update/[id]/+page.ts
--rw-r--r--   0        0        0      360 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/module/snake_module_name/component/model/snake_entity_name_model.py
--rw-r--r--   0        0        0      303 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/module/snake_module_name/component/repo/snake_entity_name_repo.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/module/snake_module_name/entity/snake_entity_name/__init__.py
--rw-r--r--   0        0        0     4836 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/module/snake_module_name/entity/snake_entity_name/api.py
--rw-r--r--   0        0        0      414 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/module/snake_module_name/entity/snake_entity_name/model.py
--rw-r--r--   0        0        0      662 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/module/snake_module_name/entity/snake_entity_name/repo.py
--rw-r--r--   0        0        0     2700 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/module/snake_module_name/entity/snake_entity_name/rpc.py
--rw-r--r--   0        0        0      346 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/src/module/snake_module_name/schema/snake_entity_name.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/test/snake_module_name/__init__.py
--rw-r--r--   0        0        0     8470 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_crud/template/src/kebab-app-name/test/snake_module_name/test_snake_entity_name.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_field/__init__.py
--rw-r--r--   0        0        0    15514 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_field/add.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/__init__.py
--rw-r--r--   0        0        0    15128 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/add.py
--rw-r--r--   0        0        0      360 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/api.py
--rw-r--r--   0        0        0       70 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/component/__init__.py
--rw-r--r--   0        0        0       83 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/component/base.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/component/model/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/component/repo/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/core/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/entity/__init__.py
--rw-r--r--   0        0        0      564 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/entity/table.py
--rw-r--r--   0        0        0      293 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/event.py
--rw-r--r--   0        0        0      515 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/migrate.py
--rw-r--r--   0        0        0     1260 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/register_module.py
--rw-r--r--   0        0        0      310 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/rpc.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/src/module/snake_module_name/schema/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/fastapp_module/template/src/kebab-app-name/test/snake_module_name/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/__init__.py
--rw-r--r--   0        0        0     2206 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/create.py
--rw-r--r--   0        0        0       27 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/template/.gitignore
--rw-r--r--   0        0        0     2000 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/builtin/generator/project/template/README.md
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/template/_automate/__init__.py
--rwxr-xr-x   0        0        0     1507 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/template/project.sh
--rw-r--r--   0        0        0       16 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/template/requirements.txt
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/template/src/.gitkeep
--rw-r--r--   0        0        0      100 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/template/template.env
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project/template/zrb_init.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/__init__.py
--rw-r--r--   0        0        0     4089 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/task_factory.py
--rw-r--r--   0        0        0      644 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/__init__.py
--rw-r--r--   0        0        0      322 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/build_project_images.py
--rw-r--r--   0        0        0      298 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/deploy_project.py
--rw-r--r--   0        0        0      312 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/destroy_project.py
--rw-r--r--   0        0        0      319 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/push_project_images.py
--rw-r--r--   0        0        0      342 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/remove_project_containers.py
--rw-r--r--   0        0        0      294 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/start_project.py
--rw-r--r--   0        0        0      333 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/start_project_containers.py
--rw-r--r--   0        0        0      334 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/project_task/template/_automate/_project/stop_project_containers.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/python_task/__init__.py
--rw-r--r--   0        0        0     1916 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/python_task/add.py
--rw-r--r--   0        0        0      742 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/python_task/template/_automate/snake_task_name.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/__init__.py
--rw-r--r--   0        0        0     6180 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/add.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/__init__.py
--rw-r--r--   0        0        0     1286 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/_common.py
--rw-r--r--   0        0        0      148 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/cmd/pulumi-destroy.sh
--rw-r--r--   0        0        0      143 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/cmd/pulumi-up.sh
--rw-r--r--   0        0        0      338 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/cmd/start.sh
--rw-r--r--   0        0        0     4197 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/container.py
--rw-r--r--   0        0        0     3088 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/deployment.py
--rw-r--r--   0        0        0     1976 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/image.py
--rw-r--r--   0        0        0     1494 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/_automate/snake_app_name/local.py
--rw-r--r--   0        0        0       31 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/.gitignore
--rw-r--r--   0        0        0       12 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/deployment/.gitignore
--rw-r--r--   0        0        0      133 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/deployment/Pulumi.yaml
--rw-r--r--   0        0        0     2876 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/deployment/__main__.py
--rw-r--r--   0        0        0       75 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/deployment/requirements.txt
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/deployment/state/.gitkeep
--rw-r--r--   0        0        0       62 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/docker-compose.env
--rw-r--r--   0        0        0      479 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/docker-compose.yml
--rw-r--r--   0        0        0       22 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/src/.dockerignore
--rw-r--r--   0        0        0       23 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/src/.gitignore
--rw-r--r--   0        0        0      187 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/src/Dockerfile
--rw-r--r--   0        0        0      447 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/src/main.py
--rw-r--r--   0        0        0       15 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/src/requirements.txt
--rw-r--r--   0        0        0       84 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/generator/simple_python_app/template/src/kebab-app-name/src/template.env
--rw-r--r--   0        0        0     1643 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/git.py
--rw-r--r--   0        0        0     1349 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/md5.py
--rw-r--r--   0        0        0     1869 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/principle.py
--rw-r--r--   0        0        0     1178 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/project.py
--rw-r--r--   0        0        0     1590 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/ubuntu.py
--rw-r--r--   0        0        0      409 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/update.py
--rw-r--r--   0        0        0      475 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/builtin/version.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/config.toml
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/config/__init__.py
--rw-r--r--   0        0        0     1057 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/config/config.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/accessories/__init__.py
--rw-r--r--   0        0        0      607 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/accessories/color.py
--rw-r--r--   0        0        0      289 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/accessories/icon.py
--rw-r--r--   0        0        0     1213 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/accessories/name.py
--rw-r--r--   0        0        0      773 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/advertisement.py
--rw-r--r--   0        0        0     1734 2023-08-07 02:54:52.915842 zrb-0.0.82/src/zrb/helper/cli.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/__init__.py
--rw-r--r--   0        0        0     1194 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/add_argument_to_function.py
--rw-r--r--   0        0        0      970 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/add_argument_to_function_call.py
--rw-r--r--   0        0        0      778 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/add_assert_resource.py
--rw-r--r--   0        0        0     1022 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/add_function_call.py
--rw-r--r--   0        0        0     3277 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/add_import_module.py
--rw-r--r--   0        0        0     1581 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/add_key_value_to_dict.py
--rw-r--r--   0        0        0     2716 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/add_property_to_class.py
--rw-r--r--   0        0        0     3212 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/add_upstream_to_task.py
--rw-r--r--   0        0        0      941 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/append_code_to_function.py
--rw-r--r--   0        0        0       88 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/codemod/format_code.py
--rw-r--r--   0        0        0     1623 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/default_env.py
--rw-r--r--   0        0        0     1960 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/docker_compose/fetch_external_env.py
--rw-r--r--   0        0        0      590 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/docker_compose/file.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/env_map/__init__.py
--rw-r--r--   0        0        0     2014 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/env_map/fetch.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.275493 zrb-0.0.82/src/zrb/helper/file/__init__.py
--rw-r--r--   0        0        0     1441 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/file/copy_tree.py
--rw-r--r--   0        0        0      654 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/file/text.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/git/__init__.py
--rw-r--r--   0        0        0     1092 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/git/detect_changes.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/loader/__init__.py
--rw-r--r--   0        0        0      682 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/loader/load_module.py
--rw-r--r--   0        0        0      504 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/log.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/map/__init__.py
--rw-r--r--   0        0        0      382 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/map/conversion.py
--rw-r--r--   0        0        0      642 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/render_data.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/string/__init__.py
--rw-r--r--   0        0        0     1325 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/string/conversion.py
--rw-r--r--   0        0        0       66 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/string/double_quote.py
--rw-r--r--   0        0        0      261 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/string/jinja.py
--rw-r--r--   0        0        0      222 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/string/parse_replacement.py
--rw-r--r--   0        0        0     3247 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/helper/util.py
--rw-r--r--   0        0        0      112 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/runner.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/__init__.py
--rw-r--r--   0        0        0     3418 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/any_task.py
--rw-r--r--   0        0        0    17466 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/base_task.py
--rw-r--r--   0        0        0    13909 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/base_task_composite.py
--rw-r--r--   0        0        0     8856 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/cmd_task.py
--rw-r--r--   0        0        0     1594 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/decorator.py
--rw-r--r--   0        0        0    10965 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/docker_compose_task.py
--rw-r--r--   0        0        0     5242 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/flow_task.py
--rw-r--r--   0        0        0     4646 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/http_checker.py
--rw-r--r--   0        0        0     3006 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/path_checker.py
--rw-r--r--   0        0        0     3525 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/port_checker.py
--rw-r--r--   0        0        0     5542 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/resource_maker.py
--rw-r--r--   0        0        0      217 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task/task.py
--rw-r--r--   0        0        0     1778 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_env/env.py
--rw-r--r--   0        0        0     1325 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_env/env_file.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_group/__init__.py
--rw-r--r--   0        0        0     1394 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_group/group.py
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/__init__.py
--rw-r--r--   0        0        0       42 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/_constant.py
--rw-r--r--   0        0        0     2946 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/base_input.py
--rw-r--r--   0        0        0     1570 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/bool_input.py
--rw-r--r--   0        0        0     1636 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/choice_input.py
--rw-r--r--   0        0        0     1560 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/float_input.py
--rw-r--r--   0        0        0       69 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/input.py
--rw-r--r--   0        0        0     1568 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/int_input.py
--rw-r--r--   0        0        0     1521 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/password_input.py
--rw-r--r--   0        0        0     1568 2023-08-04 06:22:49.285495 zrb-0.0.82/src/zrb/task_input/str_input.py
--rw-r--r--   0        0        0       33 2023-08-04 06:22:49.285495 zrb-0.0.82/template.env
--rw-r--r--   0        0        0        0 2023-08-04 06:22:49.285495 zrb-0.0.82/test/.gitignore
--rw-r--r--   0        0        0        3 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/cmd_task/.gitignore
--rw-r--r--   0        0        0     1394 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/cmd_task/test_add_cmd_task.py
--rw-r--r--   0        0        0        3 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/docker_compose_task/.gitignore
--rw-r--r--   0        0        0     1640 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/docker_compose_task/test_add_docker_compose_task.py
--rw-r--r--   0        0        0        3 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/project/.gitignore
--rw-r--r--   0        0        0     1537 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/project/test_create_project.py
--rw-r--r--   0        0        0        3 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/python_task/.gitignore
--rw-r--r--   0        0        0     1427 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/python_task/test_add_python_task.py
--rw-r--r--   0        0        0        3 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/simple-python-app/.gitignore
--rw-r--r--   0        0        0     2323 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/generator/simple-python-app/test_add_simple_python_app.py
--rw-r--r--   0        0        0       17 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/md5_test_sum.txt
--rw-r--r--   0        0        0      352 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/test_base64.py
--rw-r--r--   0        0        0      141 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/test_env.py
--rw-r--r--   0        0        0      158 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/test_eval.py
--rw-r--r--   0        0        0      484 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/test_md5.py
--rw-r--r--   0        0        0      664 2023-08-04 06:22:49.285495 zrb-0.0.82/test/builtin/test_principle.py
--rw-r--r--   0        0        0      630 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/codemod/test_add_argument_to_function call.py
--rw-r--r--   0        0        0      536 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/codemod/test_add_argument_to_function.py
--rw-r--r--   0        0        0      260 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/codemod/test_add_assert_resource.py
--rw-r--r--   0        0        0      400 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/codemod/test_add_function_call.py
--rw-r--r--   0        0        0     1815 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/codemod/test_add_import_module.py
--rw-r--r--   0        0        0      540 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/codemod/test_add_key_value_to_dict.py
--rw-r--r--   0        0        0      643 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/codemod/test_add_property_to_class.py
--rw-r--r--   0        0        0     1068 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/codemod/test_add_upstream_to_task.py
--rw-r--r--   0        0        0     1468 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/test_fetch_external_env.py
--rw-r--r--   0        0        0     3022 2023-08-04 06:22:49.285495 zrb-0.0.82/test/helper/test_util.py
--rw-r--r--   0        0        0       72 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/cmd_task/templates/hello.sh
--rw-r--r--   0        0        0       62 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/cmd_task/templates/macros.jinja
--rw-r--r--   0        0        0     4547 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/cmd_task/test_cmd_task.py
--rw-r--r--   0        0        0       31 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/.gitignore
--rw-r--r--   0        0        0      154 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/docker-compose-simple-list-env.yml
--rw-r--r--   0        0        0      153 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/docker-compose-simple-map-env.yml
--rw-r--r--   0        0        0      153 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/docker-compose-simple-no-default-env.yml
--rw-r--r--   0        0        0      108 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/docker-compose-simple.yml
--rw-r--r--   0        0        0      101 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/docker-compose.yml
--rw-r--r--   0        0        0      130 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/image/Dockerfile
--rw-r--r--   0        0        0      278 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/image/my_program.py
--rw-r--r--   0        0        0       32 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/resource/runtime.env
--rw-r--r--   0        0        0     6867 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/docker_compose_task/test_docker_compose_task.py
--rw-r--r--   0        0        0        3 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/resource_maker/.gitignore
--rw-r--r--   0        0        0       21 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/resource_maker/template/excluded
--rw-r--r--   0        0        0      111 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/resource_maker/template/src/app_name.py
--rw-r--r--   0        0        0       12 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/resource_maker/template/src/config_app_name.py
--rw-r--r--   0        0        0     1896 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/resource_maker/test_resource_maker.py
--rw-r--r--   0        0        0      286 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/test_decorator.py
--rw-r--r--   0        0        0     1990 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/test_flow_task.py
--rw-r--r--   0        0        0       10 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/test_task.env
--rw-r--r--   0        0        0     8886 2023-08-04 06:22:49.285495 zrb-0.0.82/test/task/test_task.py
--rw-r--r--   0        0        0     7488 2023-08-04 06:22:49.285495 zrb-0.0.82/zrb_init.py
--rw-r--r--   0        0        0     8595 1970-01-01 00:00:00.000000 zrb-0.0.82/PKG-INFO
+-rw-r--r--   0        0        0       91 2023-02-03 00:50:39.432627 zrb-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2023-01-25 23:16:29.196224 zrb-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6721 2023-02-03 02:33:59.127475 zrb-0.0.9/README.md
+-rw-r--r--   0        0        0       23 2023-01-26 00:56:17.990155 zrb-0.0.9/playground-template/requirements.txt
+-rw-r--r--   0        0        0     2361 2023-02-03 02:08:04.414417 zrb-0.0.9/playground-template/zrb_init.py
+-rw-r--r--   0        0        0      885 2023-02-03 02:36:44.190380 zrb-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      456 2023-02-01 14:06:02.425736 zrb-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      361 2023-02-02 00:15:49.253344 zrb-0.0.9/src/zrb/__init__.py
+-rw-r--r--   0        0        0      308 2023-01-29 07:05:35.143713 zrb-0.0.9/src/zrb/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-26 13:13:07.014863 zrb-0.0.9/src/zrb/action/__init__.py
+-rw-r--r--   0        0        0      271 2023-01-31 22:50:45.065675 zrb-0.0.9/src/zrb/action/base_action.py
+-rw-r--r--   0        0        0     3188 2023-02-03 01:52:09.242861 zrb-0.0.9/src/zrb/action/runner.py
+-rw-r--r--   0        0        0        0 2023-01-25 23:08:05.399961 zrb-0.0.9/src/zrb/config.toml
+-rw-r--r--   0        0        0        0 2023-01-28 15:51:34.079390 zrb-0.0.9/src/zrb/config/__init__.py
+-rw-r--r--   0        0        0      723 2023-02-01 01:07:49.107707 zrb-0.0.9/src/zrb/config/config.py
+-rw-r--r--   0        0        0        0 2023-02-01 00:57:08.130185 zrb-0.0.9/src/zrb/default/__init__.py
+-rw-r--r--   0        0        0      143 2023-02-01 12:27:30.727064 zrb-0.0.9/src/zrb/default/_register.py
+-rw-r--r--   0        0        0        0 2023-02-01 12:23:14.002683 zrb-0.0.9/src/zrb/default/show/__init__.py
+-rw-r--r--   0        0        0       71 2023-02-01 12:23:07.211120 zrb-0.0.9/src/zrb/default/show/_group.py
+-rw-r--r--   0        0        0      165 2023-02-01 12:25:08.076005 zrb-0.0.9/src/zrb/default/show/_register.py
+-rw-r--r--   0        0        0      419 2023-02-01 12:22:39.670923 zrb-0.0.9/src/zrb/default/show/solid_principle.py
+-rw-r--r--   0        0        0        0 2023-01-26 17:05:38.257459 zrb-0.0.9/src/zrb/helper/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-29 07:18:18.811612 zrb-0.0.9/src/zrb/helper/accessories/__init__.py
+-rw-r--r--   0        0        0      605 2023-02-01 13:09:57.333054 zrb-0.0.9/src/zrb/helper/accessories/color.py
+-rw-r--r--   0        0        0      289 2023-01-29 07:22:31.556891 zrb-0.0.9/src/zrb/helper/accessories/icon.py
+-rw-r--r--   0        0        0      734 2023-01-29 07:23:03.100524 zrb-0.0.9/src/zrb/helper/accessories/name.py
+-rw-r--r--   0        0        0        0 2023-01-29 07:04:25.375901 zrb-0.0.9/src/zrb/helper/cli/__init__.py
+-rw-r--r--   0        0        0      854 2023-02-02 13:26:09.841649 zrb-0.0.9/src/zrb/helper/cli/create_cli.py
+-rw-r--r--   0        0        0        0 2023-02-02 00:07:34.128110 zrb-0.0.9/src/zrb/helper/file/__init__.py
+-rw-r--r--   0        0        0     1072 2023-02-02 00:14:53.350008 zrb-0.0.9/src/zrb/helper/file/copy_tree.py
+-rw-r--r--   0        0        0        0 2023-01-29 09:51:03.021386 zrb-0.0.9/src/zrb/helper/keyval/__init__.py
+-rw-r--r--   0        0        0      292 2023-01-29 12:03:56.752556 zrb-0.0.9/src/zrb/helper/keyval/get_object_from_keyval.py
+-rw-r--r--   0        0        0        0 2023-01-30 00:00:14.499191 zrb-0.0.9/src/zrb/helper/list/__init__.py
+-rw-r--r--   0        0        0      225 2023-01-30 00:34:10.735498 zrb-0.0.9/src/zrb/helper/list/append_unique.py
+-rw-r--r--   0        0        0        0 2023-01-29 07:10:48.042678 zrb-0.0.9/src/zrb/helper/loader/__init__.py
+-rw-r--r--   0        0        0      515 2023-01-28 09:35:10.871488 zrb-0.0.9/src/zrb/helper/loader/load_module.py
+-rw-r--r--   0        0        0        0 2023-01-30 11:33:05.031065 zrb-0.0.9/src/zrb/helper/string/__init__.py
+-rw-r--r--   0        0        0      106 2023-02-02 00:14:42.379983 zrb-0.0.9/src/zrb/helper/string/get_cmd_name.py
+-rw-r--r--   0        0        0      222 2023-02-02 00:14:36.549973 zrb-0.0.9/src/zrb/helper/string/parse_replacement.py
+-rw-r--r--   0        0        0      112 2023-01-30 12:25:25.659518 zrb-0.0.9/src/zrb/runner.py
+-rw-r--r--   0        0        0        0 2023-01-28 08:13:04.531303 zrb-0.0.9/src/zrb/task/__init__.py
+-rw-r--r--   0        0        0     9311 2023-02-03 00:58:03.044328 zrb-0.0.9/src/zrb/task/base_model.py
+-rw-r--r--   0        0        0     8044 2023-02-03 02:31:11.013437 zrb-0.0.9/src/zrb/task/base_task.py
+-rw-r--r--   0        0        0     5817 2023-02-03 01:55:32.572250 zrb-0.0.9/src/zrb/task/cmd_task.py
+-rw-r--r--   0        0        0     1889 2023-02-03 01:55:32.572250 zrb-0.0.9/src/zrb/task/code_maker.py
+-rw-r--r--   0        0        0     3204 2023-02-03 02:31:27.533455 zrb-0.0.9/src/zrb/task/http_checker.py
+-rw-r--r--   0        0        0     2293 2023-02-03 01:55:32.572250 zrb-0.0.9/src/zrb/task/port_checker.py
+-rw-r--r--   0        0        0      178 2023-02-03 01:29:30.760810 zrb-0.0.9/src/zrb/task/task.py
+-rw-r--r--   0        0        0     1256 2023-02-02 13:25:22.958598 zrb-0.0.9/src/zrb/task_env/env.py
+-rw-r--r--   0        0        0        0 2023-01-30 12:22:20.499082 zrb-0.0.9/src/zrb/task_group/__init__.py
+-rw-r--r--   0        0        0      976 2023-02-02 00:14:02.737901 zrb-0.0.9/src/zrb/task_group/group.py
+-rw-r--r--   0        0        0        0 2023-01-26 13:46:53.388645 zrb-0.0.9/src/zrb/task_input/__init__.py
+-rw-r--r--   0        0        0     2635 2023-02-01 00:50:56.349866 zrb-0.0.9/src/zrb/task_input/base_input.py
+-rw-r--r--   0        0        0     1593 2023-02-01 00:45:48.330541 zrb-0.0.9/src/zrb/task_input/str_input.py
+-rw-r--r--   0        0        0        0 2023-01-26 00:53:09.508720 zrb-0.0.9/tests/.gitignore
+-rw-r--r--   0        0        0       72 2023-02-03 00:06:05.061598 zrb-0.0.9/tests/task/cmd_task/templates/hello.sh
+-rw-r--r--   0        0        0       62 2023-02-03 00:05:58.761569 zrb-0.0.9/tests/task/cmd_task/templates/macros.jinja
+-rw-r--r--   0        0        0     3704 2023-02-03 00:41:42.217733 zrb-0.0.9/tests/task/cmd_task/test_cmd_task.py
+-rw-r--r--   0        0        0       21 2023-02-03 00:51:35.527191 zrb-0.0.9/tests/task/code_maker/template/excluded
+-rw-r--r--   0        0        0      111 2023-02-03 00:53:04.081119 zrb-0.0.9/tests/task/code_maker/template/src/app_name.py
+-rw-r--r--   0        0        0       12 2023-02-03 00:53:09.531127 zrb-0.0.9/tests/task/code_maker/template/src/config_app_name.py
+-rw-r--r--   0        0        0     1568 2023-02-03 01:10:58.177183 zrb-0.0.9/tests/task/code_maker/test_code_maker.py
+-rwxr-xr-x   0        0        0     2729 2023-02-02 00:23:14.924872 zrb-0.0.9/toolkit.sh
+-rw-r--r--   0        0        0     7335 1970-01-01 00:00:00.000000 zrb-0.0.9/PKG-INFO
```

### Comparing `zrb-0.0.82/pyproject.toml` & `zrb-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,41 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "zrb"
-version = "0.0.82"
+version = "0.0.9"
 authors = [
   { name="Go Frendi Gunawan", email="gofrendiasgard@gmail.com" },
 ]
-description = "Super framework for your super app"
+description = "Your faithful companion"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
 ]
 dependencies = [
-  "click==8.1.4",
-  "aiofiles==23.1.0",
-  "typeguard==2.13.3",
-  "termcolor==2.3.0",
-  "Jinja2==3.1.2",
-  "libcst==0.4.9",
-  "python-dotenv==1.0.0",
-  "jsons==1.6.3",
-  "ruamel.yaml==0.17.32",
-  "setuptools==68.0.0",
-  "autopep8==2.0.2",
+    "click==8.1.3",
+    "typeguard==2.13.3",
+    "termcolor==2.2.0",
+    "Jinja2==3.1.2"
 ]
-
-[project.optional-dependencies]
-dev = [
-  "flake8==6.0.0",
-]
-test = [
-  "pytest==7.4.0",
-  "pytest-cov==4.1.0",
-  "pytest-xdist==3.3.1",
-  "pytest-asyncio==0.21.0",
+dev-dependencies = [
+  "autopep8=2.0.1",
+  "flake8=6.0.0",
+  "pytest=7.2.1",
+  "pytest-cov=4.0.0"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/state-alchemists/zrb"
-"Bug Tracker" = "https://github.com/state-alchemists/zrb/issues"
+"Homepage" = "https://github.com/state-alchemists/zaruba"
+"Bug Tracker" = "https://github.com/state-alchemists/zaruba/issues"
 
 [project.scripts]
 zrb = "zrb.__main__:cli"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
```

### Comparing `zrb-0.0.82/src/zrb/action/runner.py` & `zrb-0.0.9/src/zrb/action/runner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,46 @@
-from typing import Any, Callable, Iterable, List, Mapping, Union
+from typing import List, Mapping, Union
+from ..action.base_action import BaseAction
+from ..task.base_task import BaseTask
 from ..task_group.group import Group as TaskGroup
-from ..task.any_task import AnyTask
 import click
-import sys
 
 CliSubcommand = Union[click.Group, click.Command]
 
 
-class Runner():
+class Runner(BaseAction):
     '''
     Runner class.
     Any tasks registered to the runner will be accessible from the terminal
     '''
 
     def __init__(self, env_prefix: str = ''):
-        self._env_prefix = env_prefix
-        self._tasks: Iterable[AnyTask] = []
+        BaseAction.__init__(self)
+        self.env_prefix = env_prefix
         self._registered_groups: Mapping[str, click.Group] = {}
         self._top_levels: List[CliSubcommand] = []
         self._subcommands: Mapping[str, List[click.Group]] = {}
 
-    def register(self, task: AnyTask):
-        self._tasks.append(task)
-        task.set_has_cli_interface()
-
     def serve(self, cli: click.Group) -> click.Group:
         for task in self._tasks:
             subcommand = self._create_cli_subcommand(task)
             if subcommand not in self._top_levels:
                 self._top_levels.append(subcommand)
                 cli.add_command(subcommand)
         return cli
 
-    def _create_cli_subcommand(self, task: AnyTask) -> click.Group:
+    def _create_cli_subcommand(self, task: BaseTask) -> click.Group:
         subcommand: CliSubcommand = self._create_cli_command(task)
-        task_group = task._group
+        task_group = task.group
         while task_group is not None:
             group = self._register_sub_command(task_group, subcommand)
-            if task_group._parent is None:
+            if task_group.parent is None:
                 return group
             subcommand = group
-            task_group = task_group._parent
+            task_group = task_group.parent
         return subcommand
 
     def _register_sub_command(
         self, task_group: TaskGroup, subcommand: CliSubcommand
     ) -> click.Group:
         task_group_id = task_group.get_id()
         group = self._get_cli_group(task_group)
@@ -56,46 +52,28 @@
         return group
 
     def _get_cli_group(self, task_group: TaskGroup) -> click.Group:
         task_group_id = task_group.get_id()
         if task_group_id in self._registered_groups:
             return self._registered_groups[task_group_id]
         group_cmd_name = task_group.get_cmd_name()
-        group_description = task_group._description
+        group_description = task_group.description
         group = click.Group(name=group_cmd_name, help=group_description)
         self._registered_groups[task_group_id] = group
         return group
 
-    def _create_cli_command(self, task: AnyTask) -> click.Command:
+    def _create_cli_command(self, task: BaseTask) -> click.Command:
         task_inputs = task.get_all_inputs()
         task_cmd_name = task.get_cmd_name()
         task_description = task.get_description()
-        task_function = task.to_function(
-            env_prefix=self._env_prefix, raise_error=True
-        )
-        callback = self._wrap_task_function(task_function)
+        task_main_loop = task.create_main_loop(env_prefix=self.env_prefix)
         command = click.Command(
-            callback=callback, name=task_cmd_name, help=task_description
+            callback=task_main_loop, name=task_cmd_name, help=task_description
         )
         # by default, add an argument named _args
         command.params.append(click.Argument(['_args'], nargs=-1))
-        # add task inputs,
-        # if there are inputs with the same name, choose the first.
-        registered_input: Mapping[str, bool] = {}
+        # add task inputs
         for task_input in task_inputs:
-            if task_input.name in registered_input:
-                continue
-            registered_input[task_input.name] = True
             param_decl = task_input.get_param_decl()
             options = task_input.get_options()
             command.params.append(click.Option(param_decl, **options))
         return command
-
-    def _wrap_task_function(
-        self, function: Callable[..., Any]
-    ) -> Callable[..., Any]:
-        def wrapped_function(*args: Any, **kwargs: Any) -> Any:
-            try:
-                function(*args, **kwargs)
-            except Exception:
-                sys.exit(1)
-        return wrapped_function
```

### Comparing `zrb-0.0.82/src/zrb/helper/accessories/color.py` & `zrb-0.0.9/src/zrb/helper/accessories/color.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Iterable, Optional
 from termcolor import colored as term_colored, COLORS
 import random
 
 
 def get_random_color():
     colors = [
-        'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'light_green',
-        'light_yellow', 'light_blue', 'light_magenta', 'light_cyan',
+        'green', 'yellow', 'blue', 'magenta', 'cyan',
+        'light_green', 'light_yellow', 'light_blue',
+        'light_magenta', 'light_cyan'
     ]
     return random.choice(colors)
 
 
 def is_valid_color(color: str) -> bool:
     return color in COLORS
```

### Comparing `zrb-0.0.82/src/zrb/task/cmd_task.py` & `zrb-0.0.9/src/zrb/task/base_task.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,267 +1,232 @@
-from typing import Any, Callable, Iterable, Mapping, Optional, Union
+from typing import Any, Callable, List, Mapping, Optional, TypeVar
 from typeguard import typechecked
-from .any_task import AnyTask
-from .base_task import BaseTask
+from .base_model import TaskModel
+from ..task_input.base_input import BaseInput
 from ..task_env.env import Env
-from ..task_env.env_file import EnvFile
 from ..task_group.group import Group
-from ..task_input.base_input import BaseInput
-from ..config.config import default_shell
+from ..helper.list.append_unique import append_unique
 
 import asyncio
-import atexit
-import os
-import pathlib
-import signal
+import copy
+import inspect
 
-
-class CmdResult():
-    def __init__(self, output: str, error: str):
-        self.output = output
-        self.error = error
+TTask = TypeVar('TTask', bound='BaseTask')
 
 
 @typechecked
-class CmdTask(BaseTask):
+class BaseTask(TaskModel):
     '''
-    Command Task.
-    You can use this task to run shell command.
-
-    For example:
-    ```python
-    # run a simple task
-    hello = CmdTask(
-        name='hello',
-        inputs=[StrInput(name='name', default='World')],
-        envs=[Env(name='HOME_DIR', os_name='HOME')],
-        cmd=[
-            'echo Hello {{ input.name }}',
-            'echo Home directory is: $HOME_DIR',
-        ]
-    )
-    runner.register(hello)
-
-    # run a long running process
-    run_server = CmdTask(
-        name='run',
-        inputs=[StrInput(name='dir', default='.')],
-        envs=[Env(name='PORT', os_name='WEB_PORT', default='3000')],
-        cmd='python -m http.server $PORT --directory {{input.dir}}',
-        checkers=[HTTPChecker(port='{{env.PORT}}')]
-    )
-    runner.register(run_server)
-    ```
+    Base class for all tasks.
+    Every task definition should be extended from this class.
     '''
 
     def __init__(
         self,
         name: str,
         group: Optional[Group] = None,
-        inputs: Iterable[BaseInput] = [],
-        envs: Iterable[Env] = [],
-        env_files: Iterable[EnvFile] = [],
+        inputs: List[BaseInput] = [],
+        envs: List[Env] = [],
         icon: Optional[str] = None,
         color: Optional[str] = None,
         description: str = '',
-        executable: Optional[str] = None,
-        cmd: Union[str, Iterable[str], Callable[..., str]] = '',
-        cmd_path: str = '',
-        cwd: Optional[Union[str, pathlib.Path]] = None,
-        upstreams: Iterable[AnyTask] = [],
-        checkers: Iterable[AnyTask] = [],
-        checking_interval: float = 0,
+        upstreams: List[TTask] = [],
+        checkers: List[TTask] = [],
+        checking_interval: float = 0.1,
         retry: int = 2,
         retry_interval: float = 1,
-        max_output_line: int = 1000,
-        max_error_line: int = 1000,
-        preexec_fn: Optional[Callable[[], Any]] = os.setsid,
-        skip_execution: Union[bool, str, Callable[..., bool]] = False
     ):
-        BaseTask.__init__(
+        TaskModel.__init__(
             self,
             name=name,
             group=group,
-            inputs=inputs,
             envs=envs,
-            env_files=env_files,
             icon=icon,
             color=color,
-            description=description,
-            upstreams=upstreams,
-            checkers=checkers,
-            checking_interval=checking_interval,
-            retry=retry,
-            retry_interval=retry_interval,
-            skip_execution=skip_execution
+            retry=retry
         )
-        max_output_line = max_output_line if max_output_line > 0 else 1
-        max_error_line = max_error_line if max_error_line > 0 else 1
-        self._cmd = cmd
-        self._cmd_path = cmd_path
-        self._set_cwd(cwd)
-        self._max_output_size = max_output_line
-        self._max_error_size = max_error_line
-        self._output_buffer: Iterable[str] = []
-        self._error_buffer: Iterable[str] = []
-        if executable is None and default_shell != '':
-            executable = default_shell
-        self._executable = executable
-        self._process: Optional[asyncio.subprocess.Process]
-        self._preexec_fn = preexec_fn
-
-    def _set_cwd(
-        self, cwd: Optional[Union[str, pathlib.Path]]
-    ):
-        if cwd is None:
-            self.cwd: Union[str, pathlib.Path] = os.getcwd()
-            return
-        self.cwd: Union[str, pathlib.Path] = cwd
-
-    def to_function(
-        self, env_prefix: str = '', raise_error: bool = True
-    ) -> Callable[..., CmdResult]:
-        return super().to_function(env_prefix, raise_error)
-
-    def _print_result(self, result: CmdResult):
-        if result.output == '':
-            return
-        print(result.output)
-
-    def _get_run_env_map(self) -> Mapping[str, Any]:
-        env_map = self.get_env_map()
-        input_map = self.get_input_map()
-        for input_name, input_value in input_map.items():
-            upper_input_name = '_INPUT_' + input_name.upper()
-            if upper_input_name not in env_map:
-                env_map[upper_input_name] = f'{input_value}'
-        return env_map
-
-    async def run(self, *args: Any, **kwargs: Any) -> CmdResult:
-        cmd = self._get_cmd_str(*args, **kwargs)
-        env_map = self._get_run_env_map()
-        self.print_out_dark('Run script: ' + self._get_multiline_repr(cmd))
-        self.print_out_dark('Current working directory: ' + self.cwd)
-        self._output_buffer = []
-        self._error_buffer = []
-        process = await asyncio.create_subprocess_shell(
-            cmd,
-            cwd=self.cwd,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-            env=env_map,
-            shell=True,
-            executable=self._executable,
-            close_fds=True,
-            preexec_fn=self._preexec_fn,
-            bufsize=0
+        self.inputs = inputs
+        self.description = description
+        self.retry_interval = self.sanitize_interval(
+            retry_interval, 'retry'
+        )
+        self.upstreams = upstreams
+        self.checkers = checkers
+        self.checking_interval = self.sanitize_interval(
+            checking_interval, 'checking'
         )
-        self._set_task_pid(process.pid)
-        self._process = process
-        atexit.register(self._at_exit)
-        await self._wait_process(process)
-        atexit.unregister(self._at_exit)
-        # get output and error
-        output = '\n'.join(self._output_buffer)
-        error = '\n'.join(self._error_buffer)
-        # get return code
-        return_code = process.returncode
-        if return_code != 0:
-            self.log_info(f'Exit status: {return_code}')
-            raise Exception(
-                f'Process {self._name} exited ({return_code}): {error}'
+        self._is_checked: bool = False
+        self._is_executed: bool = False
+        self._runner: Optional[Callable[..., Any]] = None
+
+    def runner(self, runner: Callable[..., Any]):
+        self._runner = runner
+
+    async def run(self, *args: Any, **kwargs: Any) -> Any:
+        '''
+        Do task execution
+        Please override this method.
+        '''
+        self.log_debug(
+            f'Run with args: {args} and kwargs: {kwargs}'
+        )
+        if self._runner is not None:
+            result = self._runner(*args, **kwargs)
+            if inspect.isawaitable(result):
+                sync_result = await result
+                self.print_out(sync_result)
+                return sync_result
+            self.print_out(result)
+            return result
+        return True
+
+    async def check(self) -> bool:
+        '''
+        Return true when task is considered completed.
+        By default, this will wait the task execution to be completed.
+        You can override this method.
+        '''
+        return self.is_done()
+
+    def get_all_inputs(self) -> List[BaseInput]:
+        ''''
+        Getting all inputs of this task and all its upstream, non-duplicated.
+        '''
+        inputs: List[BaseInput] = []
+        for upstream in self.upstreams:
+            upstream_inputs = upstream.get_all_inputs()
+            append_unique(inputs, *upstream_inputs)
+        append_unique(inputs, *self.inputs)
+        return inputs
+
+    def get_description(self) -> str:
+        if self.description != '':
+            return self.description
+        return self.name
+
+    def sanitize_interval(self, interval: float, label: str) -> float:
+        if interval < 0:
+            name = self._get_complete_name()
+            self.log_warn(
+                f'Find negative {label} interval for {name}: {interval}'
             )
-        return CmdResult(output, error)
+            return 0
+        return interval
+
+    def create_main_loop(self, env_prefix: str = '') -> Callable[..., Any]:
+        self_cp = copy.deepcopy(self)
 
-    def _at_exit(self):
-        self.retry = 0
-        if self._process.returncode is None:
+        def main_loop(**kwargs: Any) -> Any:
+            '''
+            Task main loop.
+            '''
+            async def run_and_check_all_async() -> Any:
+                self_cp._set_keyval(input_map=kwargs, env_prefix=env_prefix)
+                processes = [
+                    asyncio.create_task(self_cp._loop_check(celebrate=True)),
+                    asyncio.create_task(self_cp._run_all(**kwargs))
+                ]
+                results = await asyncio.gather(*processes)
+                return results[-1]
             try:
-                self.log_info(f'Send SIGTERM to process {self._process.pid}')
-                os.killpg(os.getpgid(self._process.pid), signal.SIGTERM)
+                return asyncio.run(run_and_check_all_async())
             except Exception:
-                self.log_error(
-                    f'Cannot send SIGTERM to process {self._process.pid}'
-                )
-
-    async def _wait_process(self, process: asyncio.subprocess.Process):
-        # Create queue
-        stdout_queue = asyncio.Queue()
-        stderr_queue = asyncio.Queue()
-        # Read from streams and put into queue
-        stdout_process = asyncio.create_task(self._queue_stream(
-            process.stdout, stdout_queue
-        ))
-        stderr_process = asyncio.create_task(self._queue_stream(
-            process.stderr, stderr_queue
-        ))
-        # Handle messages in queue
-        stdout_log_process = asyncio.create_task(self._log_from_queue(
-            stdout_queue, self.print_out,
-            self._output_buffer, self._max_output_size
-        ))
-        stderr_log_process = asyncio.create_task(self._log_from_queue(
-            stderr_queue, self.print_err,
-            self._error_buffer, self._max_error_size
-        ))
-        # wait process
-        await process.wait()
-        # wait reader and logger
-        await stdout_process
-        await stderr_process
-        await stdout_queue.put(None)
-        await stderr_queue.put(None)
-        await stdout_log_process
-        await stderr_log_process
-
-    def _get_cmd_str(self, *args: Any, **kwargs: Any) -> str:
-        return self._create_cmd_str(self._cmd_path, self._cmd, *args, **kwargs)
-
-    def _create_cmd_str(
-        self,
-        cmd_path: str,
-        cmd: Union[str, Iterable[str], Callable[..., str]],
-        *args: Any,
-        **kwargs: Any
-    ) -> str:
-        if cmd_path != '':
-            return self.render_file(cmd_path)
-        if callable(cmd):
-            return cmd(*args, **kwargs)
-        if isinstance(cmd, str):
-            return self.render_str(cmd)
-        return self.render_str('\n'.join(list(cmd)))
-
-    async def _queue_stream(self, stream, queue: asyncio.Queue):
-        while True:
+                self_cp.log_error('Failed')
+                raise
+            finally:
+                self_cp.play_bell()
+        return main_loop
+
+    async def _loop_check(self, celebrate: bool = False) -> bool:
+        while not await self._cached_check():
+            self.log_debug('Task is not ready')
+            await asyncio.sleep(self.checking_interval)
+        self.end_timer()
+        self.log_info('Task is ready')
+        if celebrate:
+            self.show_celebration()
+        return True
+
+    async def _cached_check(self) -> bool:
+        if self._is_checked:
+            self.log_debug('Skip checking, because checking flag has been set')
+            return True
+        check_result = await self._check()
+        if check_result:
+            self._is_checked = True
+            self.log_debug('Set checking flag')
+        return check_result
+
+    async def _check(self) -> bool:
+        '''
+        Check current task readiness.
+        - If self.checkers is defined,
+          this will return True once every self.checkers is completed
+        - Otherwise, this will return check method's return value.
+        '''
+        if len(self.checkers) == 0:
+            return await self.check()
+        check_processes: List[asyncio.Task] = []
+        for checker_task in self.checkers:
+            check_processes.append(asyncio.create_task(checker_task.run()))
+        await asyncio.gather(*check_processes)
+        return True
+
+    async def _run_all(self, **kwargs: Any) -> Any:
+        processes: List[asyncio.Task] = []
+        # Add upstream tasks to processes
+        for upstream_task in self.upstreams:
+            processes.append(asyncio.create_task(
+                upstream_task._run_all(**kwargs)
+            ))
+        # Add current task to processes
+        processes.append(self._cached_run(**kwargs))
+        # Wait everything to complete
+        results = await asyncio.gather(*processes)
+        return results[-1]
+
+    async def _cached_run(self, **kwargs: Any) -> Any:
+        if self._is_executed:
+            self.log_debug('Skip running, because execution flag has been set')
+            return
+        self._is_executed = True
+        self.log_debug('Set execution flag and running')
+        self.start_timer()
+        # get upstream checker
+        upstream_check_processes: List[asyncio.Task] = []
+        for upstream_task in self.upstreams:
+            upstream_check_processes.append(asyncio.create_task(
+                upstream_task._loop_check()
+            ))
+        # wait all upstream checkers to complete
+        await asyncio.gather(*upstream_check_processes)
+        # initiate args
+        args: List[Any] = [] if '_args' not in kwargs else kwargs['_args']
+        # start running task
+        result: Any
+        while self.should_attempt():
             try:
-                line = await stream.readline()
-            except Exception as e:
-                line = str(e)
-            if not line:
-                break
-            await queue.put(line)
-
-    async def _log_from_queue(
-        self,
-        queue: asyncio.Queue,
-        print_log: Callable[[str], None],
-        buffer: Iterable[str],
-        max_size: int
-    ):
-        while True:
-            line = await queue.get()
-            if not line:
+                result = await self.run(*args, **kwargs)
                 break
-            line_str = line.decode().rstrip()
-            self._add_to_buffer(buffer, max_size, line_str)
-            print_log(line_str)
-
-    def _add_to_buffer(
-        self, buffer: Iterable[str], max_size: int, new_line: str
-    ):
-        if len(buffer) >= max_size:
-            buffer.pop(0)
-        buffer.append(new_line)
-
-    def __repr__(self) -> str:
-        return f'<CmdTask name={self._name}>'
+            except Exception:
+                if self.is_last_attempt():
+                    raise
+                attempt = self.get_attempt()
+                self.log_error(f'Encounter error on attempt {attempt}')
+                self.increase_attempt()
+                await asyncio.sleep(self.retry_interval)
+        self.mark_as_done()
+        return result
+
+    def _set_keyval(self, input_map: Mapping[str, Any], env_prefix: str):
+        self.set_local_keyval(input_map=input_map, env_prefix=env_prefix)
+        for upstream_task in self.upstreams:
+            upstream_task._set_keyval(
+                input_map=input_map, env_prefix=env_prefix
+            )
+        local_env_map = self.get_env_map()
+        for checker_task in self.checkers:
+            checker_task._set_keyval(
+                input_map=input_map, env_prefix=env_prefix
+            )
+            # Checker task should be able to read local env
+            checker_task.inject_env_map(local_env_map)
```

### Comparing `zrb-0.0.82/src/zrb/task/port_checker.py` & `zrb-0.0.9/src/zrb/task/http_checker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,98 @@
-from typing import Any, Callable, Iterable, Optional, Union
+from typing import Any, Callable, List, Optional, Union
 from typeguard import typechecked
+from http.client import HTTPConnection, HTTPSConnection
 from .base_task import BaseTask
-from .any_task import AnyTask
 from ..task_env.env import Env
-from ..task_env.env_file import EnvFile
 from ..task_group.group import Group
 from ..task_input.base_input import BaseInput
 
-import socket
 import asyncio
 
 
 @typechecked
-class PortChecker(BaseTask):
+class HTTPChecker(BaseTask):
 
     def __init__(
         self,
-        name: str = 'port-check',
+        name: str = 'http_check',
         group: Optional[Group] = None,
-        inputs: Iterable[BaseInput] = [],
-        envs: Iterable[Env] = [],
-        env_files: Iterable[EnvFile] = [],
+        inputs: List[BaseInput] = [],
+        envs: List[Env] = [],
         icon: Optional[str] = None,
         color: Optional[str] = None,
         description: str = '',
         host: str = 'localhost',
         port: Union[int, str] = 80,
         timeout: Union[int, str] = 5,
-        upstreams: Iterable[AnyTask] = [],
+        method: str = 'HEAD',
+        url: str = '/',
+        is_https: bool = False,
+        upstreams: List[BaseTask] = [],
         checking_interval: float = 0.1,
-        show_error_interval: float = 5,
-        skip_execution: Union[bool, str, Callable[..., bool]] = False
     ):
         BaseTask.__init__(
             self,
             name=name,
             group=group,
             inputs=inputs,
             envs=envs,
-            env_files=env_files,
             icon=icon,
             color=color,
             description=description,
             upstreams=upstreams,
             checkers=[],
             checking_interval=checking_interval,
             retry=0,
-            retry_interval=0,
-            skip_execution=skip_execution,
+            retry_interval=0
         )
-        self._host = host
-        self._port = port
-        self._timeout = timeout
-        self._show_error_interval = show_error_interval
+        self.host = host
+        self.port = port
+        self.timeout = timeout
+        self.method = method
+        self.url = url
+        self.is_https = is_https
 
-    def to_function(
-        self, env_prefix: str = '', raise_error: bool = True
+    def create_main_loop(
+        self, env_prefix: str = ''
     ) -> Callable[..., bool]:
-        return super().to_function(env_prefix, raise_error)
+        return super().create_main_loop(env_prefix)
 
     async def run(self, *args: Any, **kwargs: Any) -> bool:
-        host = self.render_str(self._host)
-        port = self.render_int(self._port)
-        timeout = self.render_int(self._timeout)
-        wait_time = 0
-        while not self._check_port(
-            host=host,
-            port=port,
-            timeout=timeout,
-            should_print_error=wait_time >= self._show_error_interval
-        ):
-            if wait_time >= self._show_error_interval:
-                wait_time = 0
-            await asyncio.sleep(self._checking_interval)
-            wait_time += self._checking_interval
+        method = self.render_str(self.method)
+        host = self.render_str(self.host)
+        port = self.get_int(self.port)
+        url = self.render_str(self.url)
+        timeout = self.get_int(self.timeout)
+        while not self._check_connection(method, host, port, url, timeout):
+            await asyncio.sleep(self.checking_interval)
         return True
 
-    def _check_port(
-        self, host: str, port: int, timeout: int, should_print_error: bool
+    def _check_connection(
+        self, method: str, host: str, port: int, url: str, timeout: int
     ) -> bool:
-        label = self._get_label(host, port)
+        label = self._get_label(method, host, port, url)
+        conn = self._get_connection(host, port, timeout)
         try:
-            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
-                sock.settimeout(timeout)
-                result = sock.connect_ex((host, port))
-                if result == 0:
-                    self.print_out(f'{label} (OK)')
-                    return True
-                self._debug_and_print_error(
-                    f'{label} (Not OK)', should_print_error
-                )
+            conn.request(method, url)
+            res = conn.getresponse()
+            if res.status < 300:
+                self.log_info('Connection success')
+                self.print_out(f'{label} {res.status} (OK)')
+                return True
+            self.log_debug(f'{label} {res.status} (Not OK)')
         except Exception:
-            self._debug_and_print_error(
-                f'{label} Socket error', should_print_error
-            )
+            self.log_debug(f'{label} Connection error')
+        finally:
+            conn.close()
         return False
 
-    def _debug_and_print_error(self, message: str, should_print_error: bool):
-        if should_print_error:
-            self.print_err(message)
-        self.log_debug(message)
-
-    def _get_label(self, host: str, port: int) -> str:
-        return f'Checking {host}:{port}'
-
-    def __repr__(self) -> str:
-        return f'<PortChecker name={self._name}>'
+    def _get_label(self, method: str, host: str, port: int, url: str) -> str:
+        protocol = 'https' if self.is_https else 'http'
+        return f'{method} {protocol}://{host}:{port}{url}'
+
+    def _get_connection(
+        self, host: str, port: int, timeout: int
+    ) -> Union[HTTPConnection, HTTPSConnection]:
+        if self.is_https:
+            return HTTPSConnection(host, port, timeout=timeout)
+        return HTTPConnection(host, port, timeout=timeout)
```

### Comparing `zrb-0.0.82/src/zrb/task_input/base_input.py` & `zrb-0.0.9/src/zrb/task_input/base_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-from typing import Any, List, Mapping, Optional, Union
+from typing import Any, Callable, List, Mapping, Optional, Type, Union
 from typeguard import typechecked
-from ._constant import RESERVED_INPUT_NAMES
-from ..config.config import show_prompt
-from ..helper.string.jinja import is_probably_jinja
 
 
 @typechecked
 class BaseInput():
 
     def __init__(
         self,
         name: str,
         shortcut: Optional[str] = None,
-        default: Optional[Any] = None,
+        default: Any = None,
         description: Optional[str] = None,
         show_default: Union[bool, str, None] = None,
         prompt: Union[bool, str] = True,
         confirmation_prompt: Union[bool, str] = False,
         prompt_required: bool = True,
         hide_input: bool = False,
         is_flag: Optional[bool] = None,
@@ -26,16 +23,14 @@
         allow_from_autoenv: bool = True,
         type: Optional[Any] = None,
         hidden: bool = False,
         show_choices: bool = True,
         show_envvar: bool = False,
         nargs: int = 1,
     ):
-        if name in RESERVED_INPUT_NAMES:
-            raise ValueError(f'Forbidden input name: {name}')
         self.name = name
         self.shortcut = shortcut
         self.prompt = prompt
         self.default = default
         self.help = description if description is not None else name
         self.type = type
         self.show_default = show_default
@@ -58,15 +53,16 @@
     def get_param_decl(self) -> List[str]:
         param_decl: List[str] = [f'--{self.name}']
         if self.shortcut is not None:
             param_decl.append(f'-{self.shortcut}')
         return param_decl
 
     def get_options(self) -> Mapping[str, Any]:
-        options: Mapping[str, Any] = {
+        return {
+            'prompt': self.prompt,
             'default': self.default,
             'help': self.help,
             'type': self.type,
             'show_default': self.show_default,
             'confirmation_prompt': self.confirmation_prompt,
             'prompt_required': self.prompt_required,
             'hide_input': self.hide_input,
@@ -76,10 +72,7 @@
             'count': self.count,
             'allow_from_autoenv': self.allow_from_autoenv,
             'hidden': self.hidden,
             'show_choices': self.show_choices,
             'show_envvar': self.show_envvar,
             'nargs': self.nargs
         }
-        if show_prompt:
-            options['prompt'] = self.prompt
-        return options
```

### Comparing `zrb-0.0.82/src/zrb/task_input/bool_input.py` & `zrb-0.0.9/src/zrb/task_input/str_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from typing import Any, Optional, Union
 from typeguard import typechecked
 
 from ..task_input.base_input import BaseInput
 
 
 @typechecked
-class BoolInput(BaseInput):
+class StrInput(BaseInput):
 
     def __init__(
         self,
         name: str,
         shortcut: Optional[str] = None,
-        default: Optional[Any] = None,
+        default: str = '',
         description: Optional[str] = None,
         show_default: Union[bool, str, None] = None,
         prompt: Union[bool, str] = True,
         confirmation_prompt: Union[bool, str] = False,
         prompt_required: bool = True,
         hide_input: bool = False,
         is_flag: Optional[bool] = None,
         flag_value: Optional[Any] = None,
         multiple: bool = False,
         count: bool = False,
         allow_from_autoenv: bool = True,
+        type: Optional[Any] = str,
         hidden: bool = False,
         show_choices: bool = True,
         show_envvar: bool = False,
-        nargs: int = 1
+        nargs: int = 1,
     ):
         BaseInput.__init__(
             self,
             name=name,
             shortcut=shortcut,
             default=default,
             description=description,
@@ -40,13 +41,13 @@
             prompt_required=prompt_required,
             hide_input=hide_input,
             is_flag=is_flag,
             flag_value=flag_value,
             multiple=multiple,
             count=count,
             allow_from_autoenv=allow_from_autoenv,
-            type=bool,
+            type=type,
             hidden=hidden,
             show_choices=show_choices,
             show_envvar=show_envvar,
             nargs=nargs,
         )
```

### Comparing `zrb-0.0.82/test/builtin/generator/project/test_create_project.py` & `zrb-0.0.9/tests/task/code_maker/test_code_maker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,56 @@
-from zrb.builtin.generator.project.create import create_project
-from zrb.config.config import version
+from zrb.task.code_maker import CodeMaker
 import os
 import pathlib
 import shutil
 
 
-def test_create_project():
+def test_code_maker():
     # prepare path
     dir_path = pathlib.Path(__file__).parent.absolute()
+    template_path = os.path.join(dir_path, 'template')
     destination_path = os.path.join(dir_path, 'app')
     # remove destination if exists
     if os.path.exists(destination_path):
         shutil.rmtree(destination_path)
-
-    # first attempt should success
-    first_attempt_loop = create_project.to_function()
-    result = first_attempt_loop(project_dir=destination_path)
+    # initiate code_maker
+    code_maker = CodeMaker(
+        name='create-app',
+        template_path=template_path,
+        destination_path=destination_path,
+        excludes=['*/excluded'],
+        replacements={
+            'app_name': 'my_app',
+            '3000': '8080'
+        }
+    )
+    main_loop = code_maker.create_main_loop()
+    result = main_loop()
     assert result
-
-    # .git directory should exists
-    assert os.path.isdir(os.path.join(destination_path, '.git'))
-    # .gitignore file should exists
-    assert os.path.isfile(os.path.join(destination_path, '.gitignore'))
-    # zrb_init.py should exists
-    assert os.path.isfile(os.path.join(destination_path, 'zrb_init.py'))
-
-    with open(os.path.join(destination_path, 'README.md')) as readme_file:
-        readme_lines = readme_file.readlines()
-    assert readme_lines[0] == '# App\n'
-
-    with open(
-        os.path.join(destination_path, 'requirements.txt')
-    ) as requirements_file:
-        requirements_lines = requirements_file.readlines()
-    assert requirements_lines[0] == f'zrb=={version}\n'
-
-    # second attempt should failed
-    is_error = False
-    try:
-        second_attempt_loop = create_project.to_function()
-        result = second_attempt_loop(project_dir=destination_path)
-    except Exception:
-        is_error = True
-    assert is_error
+    # excluded should not exists
+    assert not os.path.exists(os.path.join(
+        destination_path, 'excluded'
+    ))
+    # config_my_app.py should exists and contain the right data
+    assert read_file(
+        os.path.join(destination_path, 'src', 'config_my_app.py')
+    ) == '\n'.join([
+        'port = 8080',
+        ''
+    ])
+    # my_app.py should exists and contain the right data
+    assert read_file(
+        os.path.join(destination_path, 'src', 'my_app.py')
+    ) == '\n'.join([
+        'from config_my_app import port',
+        '',
+        '',
+        'def start():',
+        "    print(f'starting my_app on port {port}')",
+        '    return True',
+        ''
+    ])
+
+
+def read_file(file_name: str) -> str:
+    with open(file_name) as f:
+        return f.read()
```

### Comparing `zrb-0.0.82/test/task/cmd_task/test_cmd_task.py` & `zrb-0.0.9/tests/task/cmd_task/test_cmd_task.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,125 +1,95 @@
 from zrb.task.cmd_task import CmdTask
-from zrb.task_input.str_input import StrInput
 import pathlib
 import os
 
 
-def test_cmd_task():
+def test_simple_with_no_error():
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello'
     )
-    function = cmd_task.to_function()
-    result = function()
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
     assert result.output == 'hello'
 
 
-def test_cmd_task_with_error():
+def test_simple_with_error():
     cmd_task = CmdTask(
         name='simple-error',
         cmd='forbidden command'
     )
-    function = cmd_task.to_function()
+    main_loop = cmd_task.create_main_loop()
     is_error: bool = False
     try:
-        function()
+        main_loop()
     except Exception:
         is_error = True
     assert is_error
 
 
-def test_cmd_task_with_multiline_command():
+def test_multiline_cmd():
     cmd_task = CmdTask(
-        name='multiline-no-error',
+        name='simple-no-error',
         cmd=[
             'echo hello',
             'echo hello again',
         ]
     )
-    function = cmd_task.to_function()
-    result = function()
-    assert result.output == '\n'.join(['hello', 'hello again'])
-
-
-def test_cmd_task_with_function_command():
-    cmd_task = CmdTask(
-        name='simple-no-error',
-        cmd=lambda *args, **kwargs: '\n'.join([
-            'echo hello', 'echo hello again'
-        ])
-    )
-    function = cmd_task.to_function()
-    result = function()
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
     assert result.output == '\n'.join(['hello', 'hello again'])
 
 
-def test_cmd_task_with_cmd_path():
+def test_cmd_path():
     dir_path = pathlib.Path(__file__).parent.absolute()
     cmd_task = CmdTask(
-        name='cmd-path-no-error',
+        name='simple-no-error',
         cmd_path=os.path.join(dir_path, 'templates', 'hello.sh')
     )
-    function = cmd_task.to_function()
-    result = function()
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
     assert result.output == 'Hello, World!'
 
 
-def test_cmd_task_with_upstream_with_no_error():
+def test_upstream_with_no_error():
     upstream_task = CmdTask(
         name='upstream-no-error',
         cmd='echo upstream'
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         upstreams=[upstream_task]
     )
-    function = cmd_task.to_function()
-    result = function()
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
     assert result.output == 'hello'
 
 
-def test_cmd_task_with_upstream_with_error():
+def test_upstream_with_error():
     upstream_task = CmdTask(
         name='upstream-error',
         cmd='forbidden command'
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         upstreams=[upstream_task]
     )
-    function = cmd_task.to_function()
+    main_loop = cmd_task.create_main_loop()
     is_error: bool = False
     try:
-        function()
+        main_loop()
     except Exception:
         is_error = True
     assert is_error
 
 
-def test_cmd_task_with_upstream_containing_inputs():
-    upstream = CmdTask(
-        name='ask-name',
-        inputs=[
-            StrInput(name='name')
-        ]
-    )
-    cmd_task = CmdTask(
-        name='hello',
-        cmd='echo hello {{input.name}}',
-        upstreams=[upstream]
-    )
-    function = cmd_task.to_function()
-    result = function(name='Dumbledore')
-    assert result.output == 'hello Dumbledore'
-
-
-def test_cmd_task_with_diamond_upstream():
+def test_diamond_upstream():
     upstream_0 = CmdTask(
         name='upstream-no-error',
         cmd='echo upstream 0'
     )
     upstream_1 = CmdTask(
         name='upstream-no-error',
         cmd='echo upstream 1',
@@ -131,61 +101,61 @@
         upstreams=[upstream_0]
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         upstreams=[upstream_1, upstream_2]
     )
-    function = cmd_task.to_function()
-    result = function()
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
     assert result.output == 'hello'
 
 
-def test_cmd_task_with_checker_with_no_error():
+def test_checker_with_no_error():
     checker = CmdTask(
         name='check',
         cmd='echo checked'
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         checkers=[checker]
     )
-    function = cmd_task.to_function()
-    result = function()
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
     assert result.output == 'hello'
 
 
-def test_cmd_task_with_checker_with_error():
+def test_checker_with_error():
     checker = CmdTask(
         name='check',
         cmd='forbidden command'
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         checkers=[checker]
     )
-    function = cmd_task.to_function()
+    main_loop = cmd_task.create_main_loop()
     is_error: bool = False
     try:
-        function()
+        main_loop()
     except Exception:
         is_error = True
     assert is_error
 
 
-def test_cmd_task_with_long_output():
+def test_long_output():
     cmd_task = CmdTask(
         name='long-output',
         cmd=[
             'echo 1',
             'echo 2',
             'echo 3',
             'echo 4',
             'echo 5',
         ],
         max_output_line=3,
     )
-    function = cmd_task.to_function()
-    result = function()
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
     assert result.output == '\n'.join(['3', '4', '5'])
```

