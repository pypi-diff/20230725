# Comparing `tmp/topgrade-12.0.1.tar.gz` & `tmp/topgrade-12.0.2.tar.gz`

## Comparing `topgrade-12.0.1.tar` & `topgrade-12.0.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 topgrade-12.0.1/Cargo.toml
--rw-r--r--   0     1001      123     1503 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      182 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0     1001      123      580 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      512 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0     1001      123     2337 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/check-and-lint.yaml
--rw-r--r--   0     1001      123      758 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/check-semver.yml
--rw-r--r--   0     1001      123     1903 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/code-coverage.yml
--rw-r--r--   0     1001      123      656 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/crates-publish.yml
--rw-r--r--   0     1001      123     2132 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/release-cross.yml
--rw-r--r--   0     1001      123     2297 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/release.yml
--rw-r--r--   0     1001      123      419 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/test-config-creation.yml
--rw-r--r--   0     1001      123      498 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/update_aur.yml
--rw-r--r--   0     1001      123     1083 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/update_homebrew.yml
--rw-r--r--   0     1001      123     2261 2023-07-23 12:09:10.000000 topgrade-12.0.1/.github/workflows/update_pypi.yml
--rw-r--r--   0     1001      123       27 2023-07-23 12:09:10.000000 topgrade-12.0.1/.gitignore
--rw-r--r--   0     1001      123     1040 2023-07-23 12:09:10.000000 topgrade-12.0.1/.vscode/launch.json
--rw-r--r--   0     1001      123      187 2023-07-23 12:09:10.000000 topgrade-12.0.1/.vscode/tasks.json
--rw-r--r--   0     1001      123     1401 2023-07-23 12:09:10.000000 topgrade-12.0.1/.vscode/topgrade.code-snippets
--rw-r--r--   0     1001      123     5226 2023-07-23 12:09:10.000000 topgrade-12.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123     4344 2023-07-23 12:09:10.000000 topgrade-12.0.1/CONTRIBUTING.md
--rw-r--r--   0     1001      123    71180 2023-07-23 12:09:10.000000 topgrade-12.0.1/Cargo.lock
--rw-r--r--   0     1001      123    35149 2023-07-23 12:09:10.000000 topgrade-12.0.1/LICENSE
--rw-r--r--   0     1001      123     4918 2023-07-23 12:09:10.000000 topgrade-12.0.1/README.md
--rw-r--r--   0     1001      123      242 2023-07-23 12:09:10.000000 topgrade-12.0.1/SECURITY.md
--rwxr-xr-x   0     1001      123     2640 2023-07-23 12:09:10.000000 topgrade-12.0.1/build-all.sh
--rw-r--r--   0     1001      123       91 2023-07-23 12:09:10.000000 topgrade-12.0.1/build.rs
--rw-r--r--   0     1001      123      280 2023-07-23 12:09:10.000000 topgrade-12.0.1/clippy.toml
--rw-r--r--   0     1001      123     4635 2023-07-23 12:09:10.000000 topgrade-12.0.1/config.example.toml
--rw-r--r--   0     1001      123       10 2023-07-23 12:09:22.000000 topgrade-12.0.1/dist/topgrade-12.0.1.tar.gz
--rw-r--r--   0     1001      123    16603 2023-07-23 12:09:10.000000 topgrade-12.0.1/doc/topgrade.afdesign
--rw-r--r--   0     1001      123    31029 2023-07-23 12:09:10.000000 topgrade-12.0.1/doc/topgrade.png
--rw-r--r--   0     1001      123    35141 2023-07-23 12:09:10.000000 topgrade-12.0.1/doc/topgrade_transparent.png
--rw-r--r--   0     1001      123      348 2023-07-23 12:09:10.000000 topgrade-12.0.1/pyproject.toml
--rw-r--r--   0     1001      123       16 2023-07-23 12:09:10.000000 topgrade-12.0.1/rustfmt.toml
--rw-r--r--   0     1001      123     9299 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/command.rs
--rw-r--r--   0     1001      123    44755 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/config.rs
--rw-r--r--   0     1001      123      566 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/ctrlc/interrupted.rs
--rw-r--r--   0     1001      123      200 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/ctrlc/mod.rs
--rw-r--r--   0     1001      123      572 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/ctrlc/unix.rs
--rw-r--r--   0     1001      123      578 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/ctrlc/windows.rs
--rw-r--r--   0     1001      123      871 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/error.rs
--rw-r--r--   0     1001      123     1908 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/execution_context.rs
--rw-r--r--   0     1001      123     7171 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/executor.rs
--rw-r--r--   0     1001      123       34 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/lib.rs
--rw-r--r--   0     1001      123    22717 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/main.rs
--rw-r--r--   0     1001      123      993 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/report.rs
--rw-r--r--   0     1001      123     2755 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/runner.rs
--rw-r--r--   0     1001      123     1178 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/self_renamer.rs
--rw-r--r--   0     1001      123     1723 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/self_update.rs
--rw-r--r--   0     1001      123        0 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/bun.rs
--rw-r--r--   0     1001      123     6141 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/containers.rs
--rw-r--r--   0     1001      123      341 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/emacs.el
--rw-r--r--   0     1001      123     2849 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/emacs.rs
--rw-r--r--   0     1001      123    24466 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/generic.rs
--rw-r--r--   0     1001      123     9975 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/git.rs
--rw-r--r--   0     1001      123     1513 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/go.rs
--rw-r--r--   0     1001      123      541 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/kakoune.rs
--rw-r--r--   0     1001      123      288 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/mod.rs
--rw-r--r--   0     1001      123     7868 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/node.rs
--rw-r--r--   0     1001      123     1027 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/android.rs
--rw-r--r--   0     1001      123    10400 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/archlinux.rs
--rw-r--r--   0     1001      123      862 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/dragonfly.rs
--rw-r--r--   0     1001      123     1220 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/freebsd.rs
--rw-r--r--   0     1001      123    31120 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/linux.rs
--rw-r--r--   0     1001      123     2788 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/macos.rs
--rw-r--r--   0     1001      123      473 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/mod.rs
--rw-r--r--   0     1001      123      788 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/openbsd.rs
--rw-r--r--   0     1001      123      211 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/amazon_linux
--rw-r--r--   0     1001      123      258 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/arch
--rw-r--r--   0     1001      123      311 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/arch32
--rw-r--r--   0     1001      123      284 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/artix
--rw-r--r--   0     1001      123      393 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/centos
--rw-r--r--   0     1001      123      307 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/clearlinux
--rw-r--r--   0     1001      123      267 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/debian
--rw-r--r--   0     1001      123      186 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/deepin
--rw-r--r--   0     1001      123      199 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/exherbo
--rw-r--r--   0     1001      123      769 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/fedora
--rwxr-xr-x   0     1001      123      580 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/fedoraremixforwsl
--rw-r--r--   0     1001      123      307 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/garuda
--rw-r--r--   0     1001      123      190 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/gentoo
--rw-r--r--   0     1001      123      209 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/manjaro
--rw-r--r--   0     1001      123      170 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/manjaro-arm
--rw-r--r--   0     1001      123      308 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/mint
--rw-r--r--   0     1001      123      410 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/nixos
--rw-r--r--   0     1001      123      275 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/opensuse
--rw-r--r--   0     1001      123      451 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/oracle
--rw-r--r--   0     1001      123      204 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/pclinuxos
--rwxr-xr-x   0     1001      123      355 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/pengwinonwsl
--rw-r--r--   0     1001      123       85 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/pureos
--rw-r--r--   0     1001      123      501 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/rhel
--rw-r--r--   0     1001      123      306 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/solus
--rw-r--r--   0     1001      123      398 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/ubuntu
--rw-r--r--   0     1001      123      384 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/os_release/vanilla
--rw-r--r--   0     1001      123    16411 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/unix.rs
--rw-r--r--   0     1001      123     5469 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/os/windows.rs
--rw-r--r--   0     1001      123     3712 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/powershell.rs
--rw-r--r--   0     1001      123       32 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/remote/mod.rs
--rw-r--r--   0     1001      123     1981 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/remote/ssh.rs
--rw-r--r--   0     1001      123     6718 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/remote/vagrant.rs
--rw-r--r--   0     1001      123     5892 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/tmux.rs
--rw-r--r--   0     1001      123     1947 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/toolbx.rs
--rw-r--r--   0     1001      123       70 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/upgrade.kak
--rw-r--r--   0     1001      123      954 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/upgrade.vim
--rw-r--r--   0     1001      123     3972 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/vim.rs
--rw-r--r--   0     1001      123     7004 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/steps/zsh.rs
--rw-r--r--   0     1001      123     4068 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/sudo.rs
--rw-r--r--   0     1001      123     9572 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/terminal.rs
--rw-r--r--   0     1001      123     8062 2023-07-23 12:09:10.000000 topgrade-12.0.1/src/utils.rs
--rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 topgrade-12.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 topgrade-12.0.2/Cargo.toml
+-rw-r--r--   0     1001      123     1503 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      182 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0     1001      123      580 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      512 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0     1001      123     2337 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/check-and-lint.yaml
+-rw-r--r--   0     1001      123      758 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/check-semver.yml
+-rw-r--r--   0     1001      123     1903 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/code-coverage.yml
+-rw-r--r--   0     1001      123      656 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/crates-publish.yml
+-rw-r--r--   0     1001      123     2132 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/release-cross.yml
+-rw-r--r--   0     1001      123     2297 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      419 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/test-config-creation.yml
+-rw-r--r--   0     1001      123      498 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/update_aur.yml
+-rw-r--r--   0     1001      123     1083 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/update_homebrew.yml
+-rw-r--r--   0     1001      123     2261 2023-07-25 06:27:08.000000 topgrade-12.0.2/.github/workflows/update_pypi.yml
+-rw-r--r--   0     1001      123       27 2023-07-25 06:27:08.000000 topgrade-12.0.2/.gitignore
+-rw-r--r--   0     1001      123     1040 2023-07-25 06:27:08.000000 topgrade-12.0.2/.vscode/launch.json
+-rw-r--r--   0     1001      123      187 2023-07-25 06:27:08.000000 topgrade-12.0.2/.vscode/tasks.json
+-rw-r--r--   0     1001      123     1401 2023-07-25 06:27:08.000000 topgrade-12.0.2/.vscode/topgrade.code-snippets
+-rw-r--r--   0     1001      123     5226 2023-07-25 06:27:08.000000 topgrade-12.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123     4344 2023-07-25 06:27:08.000000 topgrade-12.0.2/CONTRIBUTING.md
+-rw-r--r--   0     1001      123    72314 2023-07-25 06:27:08.000000 topgrade-12.0.2/Cargo.lock
+-rw-r--r--   0     1001      123    35149 2023-07-25 06:27:08.000000 topgrade-12.0.2/LICENSE
+-rw-r--r--   0     1001      123     4918 2023-07-25 06:27:08.000000 topgrade-12.0.2/README.md
+-rw-r--r--   0     1001      123      242 2023-07-25 06:27:08.000000 topgrade-12.0.2/SECURITY.md
+-rwxr-xr-x   0     1001      123     2640 2023-07-25 06:27:08.000000 topgrade-12.0.2/build-all.sh
+-rw-r--r--   0     1001      123       91 2023-07-25 06:27:08.000000 topgrade-12.0.2/build.rs
+-rw-r--r--   0     1001      123      280 2023-07-25 06:27:08.000000 topgrade-12.0.2/clippy.toml
+-rw-r--r--   0     1001      123     4713 2023-07-25 06:27:08.000000 topgrade-12.0.2/config.example.toml
+-rw-r--r--   0     1001      123       10 2023-07-25 06:27:22.000000 topgrade-12.0.2/dist/topgrade-12.0.2.tar.gz
+-rw-r--r--   0     1001      123    16603 2023-07-25 06:27:08.000000 topgrade-12.0.2/doc/topgrade.afdesign
+-rw-r--r--   0     1001      123    31029 2023-07-25 06:27:08.000000 topgrade-12.0.2/doc/topgrade.png
+-rw-r--r--   0     1001      123    35141 2023-07-25 06:27:08.000000 topgrade-12.0.2/doc/topgrade_transparent.png
+-rw-r--r--   0     1001      123      348 2023-07-25 06:27:08.000000 topgrade-12.0.2/pyproject.toml
+-rw-r--r--   0     1001      123       16 2023-07-25 06:27:08.000000 topgrade-12.0.2/rustfmt.toml
+-rw-r--r--   0     1001      123     9299 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/command.rs
+-rw-r--r--   0     1001      123    45112 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/config.rs
+-rw-r--r--   0     1001      123      566 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/ctrlc/interrupted.rs
+-rw-r--r--   0     1001      123      200 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/ctrlc/mod.rs
+-rw-r--r--   0     1001      123      572 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/ctrlc/unix.rs
+-rw-r--r--   0     1001      123      578 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/ctrlc/windows.rs
+-rw-r--r--   0     1001      123      996 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/error.rs
+-rw-r--r--   0     1001      123     1908 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/execution_context.rs
+-rw-r--r--   0     1001      123     7171 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/executor.rs
+-rw-r--r--   0     1001      123       34 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/lib.rs
+-rw-r--r--   0     1001      123    22717 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/main.rs
+-rw-r--r--   0     1001      123      993 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/report.rs
+-rw-r--r--   0     1001      123     2755 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/runner.rs
+-rw-r--r--   0     1001      123     1178 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/self_renamer.rs
+-rw-r--r--   0     1001      123     1723 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/self_update.rs
+-rw-r--r--   0     1001      123        0 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/bun.rs
+-rw-r--r--   0     1001      123     6141 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/containers.rs
+-rw-r--r--   0     1001      123      341 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/emacs.el
+-rw-r--r--   0     1001      123     2849 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/emacs.rs
+-rw-r--r--   0     1001      123    24466 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/generic.rs
+-rw-r--r--   0     1001      123     9975 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/git.rs
+-rw-r--r--   0     1001      123     1513 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/go.rs
+-rw-r--r--   0     1001      123      541 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/kakoune.rs
+-rw-r--r--   0     1001      123      288 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/mod.rs
+-rw-r--r--   0     1001      123     7868 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/node.rs
+-rw-r--r--   0     1001      123     1027 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/android.rs
+-rw-r--r--   0     1001      123    10400 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/archlinux.rs
+-rw-r--r--   0     1001      123      876 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/dragonfly.rs
+-rw-r--r--   0     1001      123     1220 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/freebsd.rs
+-rw-r--r--   0     1001      123    31112 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/linux.rs
+-rw-r--r--   0     1001      123     2788 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/macos.rs
+-rw-r--r--   0     1001      123      473 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/mod.rs
+-rw-r--r--   0     1001      123      788 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/openbsd.rs
+-rw-r--r--   0     1001      123      211 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/amazon_linux
+-rw-r--r--   0     1001      123      258 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/arch
+-rw-r--r--   0     1001      123      311 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/arch32
+-rw-r--r--   0     1001      123      284 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/artix
+-rw-r--r--   0     1001      123      393 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/centos
+-rw-r--r--   0     1001      123      307 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/clearlinux
+-rw-r--r--   0     1001      123      267 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/debian
+-rw-r--r--   0     1001      123      186 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/deepin
+-rw-r--r--   0     1001      123      199 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/exherbo
+-rw-r--r--   0     1001      123      769 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/fedora
+-rwxr-xr-x   0     1001      123      580 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/fedoraremixforwsl
+-rw-r--r--   0     1001      123      307 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/garuda
+-rw-r--r--   0     1001      123      190 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/gentoo
+-rw-r--r--   0     1001      123      209 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/manjaro
+-rw-r--r--   0     1001      123      170 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/manjaro-arm
+-rw-r--r--   0     1001      123      308 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/mint
+-rw-r--r--   0     1001      123      410 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/nixos
+-rw-r--r--   0     1001      123      275 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/opensuse
+-rw-r--r--   0     1001      123      451 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/oracle
+-rw-r--r--   0     1001      123      204 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/pclinuxos
+-rwxr-xr-x   0     1001      123      355 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/pengwinonwsl
+-rw-r--r--   0     1001      123       85 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/pureos
+-rw-r--r--   0     1001      123      501 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/rhel
+-rw-r--r--   0     1001      123      306 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/solus
+-rw-r--r--   0     1001      123      398 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/ubuntu
+-rw-r--r--   0     1001      123      384 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/os_release/vanilla
+-rw-r--r--   0     1001      123    16542 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/unix.rs
+-rw-r--r--   0     1001      123     6524 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/os/windows.rs
+-rw-r--r--   0     1001      123     3712 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/powershell.rs
+-rw-r--r--   0     1001      123       32 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/remote/mod.rs
+-rw-r--r--   0     1001      123     1981 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/remote/ssh.rs
+-rw-r--r--   0     1001      123     6718 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/remote/vagrant.rs
+-rw-r--r--   0     1001      123     5892 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/tmux.rs
+-rw-r--r--   0     1001      123     1947 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/toolbx.rs
+-rw-r--r--   0     1001      123       70 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/upgrade.kak
+-rw-r--r--   0     1001      123      954 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/upgrade.vim
+-rw-r--r--   0     1001      123     3972 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/vim.rs
+-rw-r--r--   0     1001      123     7004 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/steps/zsh.rs
+-rw-r--r--   0     1001      123     4068 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/sudo.rs
+-rw-r--r--   0     1001      123     9572 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/terminal.rs
+-rw-r--r--   0     1001      123     8062 2023-07-25 06:27:08.000000 topgrade-12.0.2/src/utils.rs
+-rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 topgrade-12.0.2/PKG-INFO
```

### Comparing `topgrade-12.0.1/Cargo.toml` & `topgrade-12.0.2/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [package]
 name = "topgrade"
 description = "Upgrade all the things"
 categories = ["os"]
 keywords = ["upgrade", "update"]
 license = "GPL-3.0"
 repository = "https://github.com/topgrade-rs/topgrade"
-version = "12.0.1"
+version = "12.0.2"
 authors = ["Roey Darwish Dror <roey.ghost@gmail.com>", "Thomas Schönauer <t.schoenauer@hgs-wt.at>"]
 exclude = ["doc/screenshot.gif"]
 edition = "2021"
 
 readme = "README.md"
 
 [[bin]]
@@ -59,15 +59,15 @@
 
 [package.metadata.deb]
 depends = "$auto,git"
 
 [target.'cfg(unix)'.dependencies]
 libc = "~0.2"
 nix = "~0.24"
-rust-ini = "~0.18"
+rust-ini = "~0.19"
 self_update_crate = { version = "~0.30", default-features = false, optional = true, package = "self_update", features = ["archive-tar", "compression-flate2", "rustls"] }
 
 [target.'cfg(windows)'.dependencies]
 self_update_crate = { version = "~0.30", default-features = false, optional = true, package = "self_update", features = ["archive-zip", "compression-zip-deflate", "rustls"] }
 winapi = "~0.3"
 parselnk = "~0.1"
```

### Comparing `topgrade-12.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `topgrade-12.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `topgrade-12.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/PULL_REQUEST_TEMPLATE.md` & `topgrade-12.0.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/workflows/check-and-lint.yaml` & `topgrade-12.0.2/.github/workflows/check-and-lint.yaml`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/workflows/check-semver.yml` & `topgrade-12.0.2/.github/workflows/check-semver.yml`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/workflows/code-coverage.yml` & `topgrade-12.0.2/.github/workflows/code-coverage.yml`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/workflows/crates-publish.yml` & `topgrade-12.0.2/.github/workflows/crates-publish.yml`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/workflows/release-cross.yml` & `topgrade-12.0.2/.github/workflows/release-cross.yml`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/workflows/release.yml` & `topgrade-12.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/workflows/update_homebrew.yml` & `topgrade-12.0.2/.github/workflows/update_homebrew.yml`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.github/workflows/update_pypi.yml` & `topgrade-12.0.2/.github/workflows/update_pypi.yml`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.vscode/launch.json` & `topgrade-12.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/.vscode/topgrade.code-snippets` & `topgrade-12.0.2/.vscode/topgrade.code-snippets`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/CODE_OF_CONDUCT.md` & `topgrade-12.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/CONTRIBUTING.md` & `topgrade-12.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/Cargo.lock` & `topgrade-12.0.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,14 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
-name = "ahash"
-version = "0.7.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
-dependencies = [
- "getrandom",
- "once_cell",
- "version_check",
-]
-
-[[package]]
 name = "aho-corasick"
 version = "0.7.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
@@ -403,14 +392,36 @@
  "lazy_static",
  "libc",
  "unicode-width",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "const-random"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "368a7a772ead6ce7e1de82bfb04c485f3db8ec744f72925af5735e29a22cc18e"
+dependencies = [
+ "const-random-macro",
+ "proc-macro-hack",
+]
+
+[[package]]
+name = "const-random-macro"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d7d6ab3c3a2282db210df5f02c4dab6e0a7057af0fb7ebd4070f30fe05c0ddb"
+dependencies = [
+ "getrandom",
+ "once_cell",
+ "proc-macro-hack",
+ "tiny-keccak",
+]
+
+[[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
@@ -436,14 +447,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
@@ -509,17 +526,20 @@
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
 name = "dlv-list"
-version = "0.3.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0688c2a7f92e427f44895cd63841bff7b29f8d7a1648b9e7e07a4a365b2e1257"
+checksum = "d529fd73d344663edfd598ccb3f344e46034db51ebd103518eae34338248ad73"
+dependencies = [
+ "const-random",
+]
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
@@ -810,17 +830,20 @@
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
-dependencies = [
- "ahash",
-]
+
+[[package]]
+name = "hashbrown"
+version = "0.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -976,15 +999,15 @@
 [[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
- "hashbrown",
+ "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indicatif"
 version = "0.16.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d207dc617c7a380ab07ff572a6e52fa202a2a8f355860ac9c38e23f8196be1b"
@@ -1287,20 +1310,20 @@
 name = "once_cell"
 version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "ordered-multimap"
-version = "0.4.3"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccd746e37177e1711c20dd619a1620f34f5c8b569c53590a72dedd5344d8924a"
+checksum = "4ed8acf08e98e744e5384c8bc63ceb0364e68a6854187221c18df61c4797690e"
 dependencies = [
  "dlv-list",
- "hashbrown",
+ "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "ordered-stream"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aa2b01e1d916879f73a53d01d1d6cee68adbb31d6d9177a8cfce093cced1d50"
@@ -1417,14 +1440,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
+name = "proc-macro-hack"
+version = "0.5.20+deprecated"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
@@ -1608,17 +1637,17 @@
 name = "roff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b833d8d034ea094b1ea68aa6d5c740e0d04bad9d16568d08ba6f76823a114316"
 
 [[package]]
 name = "rust-ini"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6d5f2436026b4f6e79dc829837d467cc7e9a55ee40e750d716713540715a2df"
+checksum = "7e2a3bcec1f113553ef1c88aae6c020a369d03d55b58de9869a0908930385091"
 dependencies = [
  "cfg-if",
  "ordered-multimap",
 ]
 
 [[package]]
 name = "rustc-demangle"
@@ -2039,14 +2068,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
+name = "tiny-keccak"
+version = "2.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
+dependencies = [
+ "crunchy",
+]
+
+[[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
@@ -2122,15 +2160,15 @@
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "topgrade"
-version = "12.0.1"
+version = "12.0.2"
 dependencies = [
  "cfg-if",
  "chrono",
  "clap",
  "clap_complete",
  "clap_mangen",
  "color-eyre",
```

### Comparing `topgrade-12.0.1/LICENSE` & `topgrade-12.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/README.md` & `topgrade-12.0.2/README.md`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/build-all.sh` & `topgrade-12.0.2/build-all.sh`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/config.example.toml` & `topgrade-12.0.2/config.example.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
 # Skip sending a notification at the end of a run
 #skip_notify = true
 
 # Whether to self update (this is ignored if the binary has been built without self update support, available also via setting the environment variable TOPGRADE_NO_SELF_UPGRADE)
 #no_self_update = true
 
+# Extra Home Manager arguments
+#home_manager_arguments = ["--flake", "file"]
+
 # Commands to run before anything
 [pre_commands]
 #"Emacs Snapshot" = "rm -rf ~/.emacs.d/elpa.bak && cp -rl ~/.emacs.d/elpa ~/.emacs.d/elpa.bak"
 
 # Commands to run after anything
 [post_commands]
 #"Emacs Snapshot" = "rm -rf ~/.emacs.d/elpa.bak && cp -rl ~/.emacs.d/elpa ~/.emacs.d/elpa.bak"
```

### Comparing `topgrade-12.0.1/doc/topgrade.afdesign` & `topgrade-12.0.2/doc/topgrade.afdesign`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/doc/topgrade.png` & `topgrade-12.0.2/doc/topgrade.png`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/doc/topgrade_transparent.png` & `topgrade-12.0.2/doc/topgrade_transparent.png`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/command.rs` & `topgrade-12.0.2/src/command.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/config.rs` & `topgrade-12.0.2/src/config.rs`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,17 @@
     rpm_ostree: Option<bool>,
 
     #[merge(strategy = crate::utils::merge_strategies::string_append_opt)]
     emerge_sync_flags: Option<String>,
 
     #[merge(strategy = crate::utils::merge_strategies::string_append_opt)]
     emerge_update_flags: Option<String>,
+
+    #[merge(strategy = crate::utils::merge_strategies::vec_prepend_opt)]
+    home_manager_arguments: Option<Vec<String>>,
 }
 
 #[derive(Deserialize, Default, Debug, Merge)]
 #[serde(deny_unknown_fields)]
 pub struct Composer {
     self_update: Option<bool>,
 }
@@ -1271,14 +1274,22 @@
     pub fn nix_arguments(&self) -> Option<&str> {
         self.config_file
             .linux
             .as_ref()
             .and_then(|linux| linux.nix_arguments.as_deref())
     }
 
+    /// Extra Home Manager arguments
+    pub fn home_manager(&self) -> Option<&Vec<String>> {
+        self.config_file
+            .linux
+            .as_ref()
+            .and_then(|misc| misc.home_manager_arguments.as_ref())
+    }
+
     /// Distrobox use root
     pub fn distrobox_root(&self) -> bool {
         self.config_file
             .distrobox
             .as_ref()
             .and_then(|r| r.use_root)
             .unwrap_or(false)
```

### Comparing `topgrade-12.0.1/src/ctrlc/interrupted.rs` & `topgrade-12.0.2/src/ctrlc/interrupted.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/ctrlc/unix.rs` & `topgrade-12.0.2/src/ctrlc/unix.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/ctrlc/windows.rs` & `topgrade-12.0.2/src/ctrlc/windows.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/error.rs` & `topgrade-12.0.2/src/error.rs`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     #[error("`{0}` failed: {1}")]
     ProcessFailedWithOutput(String, ExitStatus, String),
 
     #[error("Unknown Linux Distribution")]
     #[cfg(target_os = "linux")]
     UnknownLinuxDistribution,
 
+    #[error("File \"/etc/os-release\" does not exist or is empty")]
+    #[cfg(target_os = "linux")]
+    EmptyOSReleaseFile,
+
     #[error("Failed getting the system package manager")]
     #[cfg(target_os = "linux")]
     FailedGettingPackageManager,
 }
 
 #[derive(Error, Debug)]
 #[error("A step failed")]
```

### Comparing `topgrade-12.0.1/src/execution_context.rs` & `topgrade-12.0.2/src/execution_context.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/executor.rs` & `topgrade-12.0.2/src/executor.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/main.rs` & `topgrade-12.0.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/report.rs` & `topgrade-12.0.2/src/report.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/runner.rs` & `topgrade-12.0.2/src/runner.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/self_renamer.rs` & `topgrade-12.0.2/src/self_renamer.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/self_update.rs` & `topgrade-12.0.2/src/self_update.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/containers.rs` & `topgrade-12.0.2/src/steps/containers.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/emacs.rs` & `topgrade-12.0.2/src/steps/emacs.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/generic.rs` & `topgrade-12.0.2/src/steps/generic.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/git.rs` & `topgrade-12.0.2/src/steps/git.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/go.rs` & `topgrade-12.0.2/src/steps/go.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/kakoune.rs` & `topgrade-12.0.2/src/steps/kakoune.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/node.rs` & `topgrade-12.0.2/src/steps/node.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/os/android.rs` & `topgrade-12.0.2/src/steps/os/android.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/os/archlinux.rs` & `topgrade-12.0.2/src/steps/os/archlinux.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/os/dragonfly.rs` & `topgrade-12.0.2/src/steps/os/freebsd.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 use crate::command::CommandExt;
 use crate::execution_context::ExecutionContext;
 use crate::terminal::print_separator;
 use crate::utils::{require_option, REQUIRE_SUDO};
+use crate::Step;
 use color_eyre::eyre::Result;
 use std::process::Command;
 
-pub fn upgrade_packages(ctx: &ExecutionContext) -> Result<()> {
+pub fn upgrade_freebsd(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
-    print_separator("DragonFly BSD Packages");
-    ctx.execute(sudo)
-        .args(["/usr/local/sbin/pkg", "upgrade"])
-        .arg(if ctx.config().yes(Step::System) { "-y" } else { "" })
+    print_separator("FreeBSD Update");
+    ctx.run_type()
+        .execute(sudo)
+        .args(["/usr/sbin/freebsd-update", "fetch", "install"])
         .status_checked()
 }
 
+pub fn upgrade_packages(ctx: &ExecutionContext) -> Result<()> {
+    let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
+    print_separator("FreeBSD Packages");
+
+    let mut command = ctx.run_type().execute(sudo);
+
+    command.args(["/usr/sbin/pkg", "upgrade"]);
+    if ctx.config().yes(Step::System) {
+        command.arg("-y");
+    }
+    command.status_checked()
+}
+
 pub fn audit_packages(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
     println!();
     Command::new(sudo)
-        .args(["/usr/local/sbin/pkg", "audit", "-Fr"])
+        .args(["/usr/sbin/pkg", "audit", "-Fr"])
         .status_checked()?;
     Ok(())
 }
```

### Comparing `topgrade-12.0.1/src/steps/os/freebsd.rs` & `topgrade-12.0.2/src/steps/os/dragonfly.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 use crate::command::CommandExt;
 use crate::execution_context::ExecutionContext;
 use crate::terminal::print_separator;
 use crate::utils::{require_option, REQUIRE_SUDO};
-use crate::Step;
 use color_eyre::eyre::Result;
 use std::process::Command;
 
-pub fn upgrade_freebsd(ctx: &ExecutionContext) -> Result<()> {
-    let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
-    print_separator("FreeBSD Update");
-    ctx.run_type()
-        .execute(sudo)
-        .args(["/usr/sbin/freebsd-update", "fetch", "install"])
-        .status_checked()
-}
-
 pub fn upgrade_packages(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
-    print_separator("FreeBSD Packages");
-
-    let mut command = ctx.run_type().execute(sudo);
-
-    command.args(["/usr/sbin/pkg", "upgrade"]);
+    print_separator("DragonFly BSD Packages");
+    let mut cmd = ctx.execute(sudo);
+    cmd.args(["/usr/local/sbin/pkg", "upgrade"]);
     if ctx.config().yes(Step::System) {
-        command.arg("-y");
+        cmd.arg("-y");
     }
-    command.status_checked()
+    cmd.status_checked()
 }
 
 pub fn audit_packages(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
     println!();
     Command::new(sudo)
-        .args(["/usr/sbin/pkg", "audit", "-Fr"])
+        .args(["/usr/local/sbin/pkg", "audit", "-Fr"])
         .status_checked()?;
     Ok(())
 }
```

### Comparing `topgrade-12.0.1/src/steps/os/linux.rs` & `topgrade-12.0.2/src/steps/os/linux.rs`

 * *Files 6% similar despite different names*

```diff
@@ -110,18 +110,22 @@
         if PathBuf::from("/bedrock").exists() {
             return Ok(Distribution::Bedrock);
         }
 
         if PathBuf::from(OS_RELEASE_PATH).exists() {
             let os_release = Ini::load_from_file(OS_RELEASE_PATH)?;
 
+            if os_release.general_section().is_empty() {
+                return Err(TopgradeError::EmptyOSReleaseFile.into());
+            }
+
             return Self::parse_os_release(&os_release);
         }
 
-        Err(TopgradeError::UnknownLinuxDistribution.into())
+        Err(TopgradeError::EmptyOSReleaseFile.into())
     }
 
     pub fn upgrade(self, ctx: &ExecutionContext) -> Result<()> {
         print_separator("System update");
 
         match self {
             Distribution::Alpine => upgrade_alpine_linux(ctx),
@@ -244,53 +248,57 @@
 fn upgrade_suse(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
     ctx.run_type()
         .execute(sudo)
         .args(["zypper", "refresh"])
         .status_checked()?;
 
-    ctx.run_type()
-        .execute(sudo)
-        .arg("zypper")
-        .arg(if ctx.config().suse_dup() {
-            "dist-upgrade"
-        } else {
-            "update"
-        })
-        .arg(if ctx.config().yes(Step::System) { "-y" } else { "" })
-        .status_checked()?;
+    let mut cmd = ctx.run_type().execute(sudo);
+    cmd.arg("zypper");
+    cmd.arg(if ctx.config().suse_dup() {
+        "dist-upgrade"
+    } else {
+        "update"
+    });
+    if ctx.config().yes(Step::System) {
+        cmd.arg("-y");
+    }
+
+    cmd.status_checked()?;
 
     Ok(())
 }
 
 fn upgrade_opensuse_tumbleweed(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
     ctx.run_type()
         .execute(sudo)
         .args(["zypper", "refresh"])
         .status_checked()?;
 
-    ctx.run_type()
-        .execute(sudo)
-        .arg("zypper")
-        .arg("dist-upgrade")
-        .arg(if ctx.config().yes(Step::System) { "-y" } else { "" })
-        .status_checked()?;
+    let mut cmd = ctx.run_type().execute(sudo);
+    cmd.args(["zypper", "dist-upgrade"]);
+    if ctx.config().yes(Step::System) {
+        cmd.arg("-y");
+    }
+
+    cmd.status_checked()?;
 
     Ok(())
 }
 
 fn upgrade_suse_micro(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
-    ctx.run_type()
-        .execute(sudo)
-        .arg("transactional-update")
-        .arg(if ctx.config().yes(Step::System) { "-n" } else { "" })
-        .arg("dup")
-        .status_checked()?;
+    let mut cmd = ctx.run_type().execute(sudo);
+    cmd.arg("transactional-update");
+    if ctx.config().yes(Step::System) {
+        cmd.arg("-n");
+    }
+
+    cmd.arg("dup").status_checked()?;
 
     Ok(())
 }
 
 fn upgrade_openmandriva(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
     let mut command = ctx.run_type().execute(sudo);
@@ -321,20 +329,21 @@
 
     if ctx.config().yes(Step::System) {
         command_update.arg("-y");
     }
 
     command_update.status_checked()?;
 
-    ctx.run_type()
-        .execute(sudo)
-        .arg(&which("apt-get").unwrap())
-        .arg("dist-upgrade")
-        .arg(if ctx.config().yes(Step::System) { "-y" } else { "" })
-        .status_checked()?;
+    let mut cmd = ctx.run_type().execute(sudo);
+    cmd.arg(&which("apt-get").unwrap());
+    cmd.arg("dist-upgrade");
+    if ctx.config().yes(Step::System) {
+        cmd.arg("-y");
+    }
+    cmd.status_checked()?;
 
     Ok(())
 }
 
 fn upgrade_vanilla(ctx: &ExecutionContext) -> Result<()> {
     let apx = require("apx")?;
 
@@ -498,20 +507,20 @@
     }
 
     Ok(())
 }
 
 fn upgrade_solus(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
-    ctx.run_type()
-        .execute(sudo)
-        .arg("eopkg")
-        .arg(if ctx.config().yes(Step::System) { "-y" } else { "" })
-        .arg("upgrade")
-        .status_checked()?;
+    let mut cmd = ctx.run_type().execute(sudo);
+    cmd.arg("eopkg");
+    if ctx.config().yes(Step::System) {
+        cmd.arg("-y");
+    }
+    cmd.arg("upgrade").status_checked()?;
 
     Ok(())
 }
 
 pub fn run_am(ctx: &ExecutionContext) -> Result<()> {
     let am = require("am")?;
 
@@ -542,39 +551,34 @@
     print_separator("pacdef");
 
     let output = ctx.run_type().execute(&pacdef).arg("version").output_checked()?;
     let string = String::from_utf8(output.stdout)?;
     let new_version = string.contains("version: 1");
 
     if new_version {
-        ctx.run_type()
-            .execute(&pacdef)
-            .args(["package", "sync"])
-            .arg(if ctx.config().yes(Step::System) {
-                "--noconfirm"
-            } else {
-                ""
-            })
-            .status_checked()?;
+        let mut cmd = ctx.run_type().execute(&pacdef);
+        cmd.args(["package", "sync"]);
+        if ctx.config().yes(Step::System) {
+            cmd.arg("--noconfirm");
+        }
+        cmd.status_checked()?;
 
         println!();
         ctx.run_type()
             .execute(&pacdef)
             .args(["package", "review"])
             .status_checked()?;
     } else {
-        ctx.run_type()
-            .execute(&pacdef)
-            .arg("sync")
-            .arg(if ctx.config().yes(Step::System) {
-                "--noconfirm"
-            } else {
-                ""
-            })
-            .status_checked()?;
+        let mut cmd = ctx.run_type().execute(&pacdef);
+        cmd.arg("sync");
+        if ctx.config().yes(Step::System) {
+            cmd.arg("--noconfirm");
+        }
+
+        cmd.status_checked()?;
 
         println!();
         ctx.run_type().execute(&pacdef).arg("review").status_checked()?;
     }
     Ok(())
 }
 
@@ -612,23 +616,20 @@
             "use ~/.local/share/nushell/packer/start/packer.nu/api_layer/packer.nu; packer update",
         ])
         .status_checked()
 }
 
 fn upgrade_clearlinux(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
-    ctx.run_type()
-        .execute(sudo)
-        .args(["swupd", "update"])
-        .arg(if ctx.config().yes(Step::System) {
-            "--assume=yes"
-        } else {
-            ""
-        })
-        .status_checked()?;
+    let mut cmd = ctx.run_type().execute(sudo);
+    cmd.args(["swupd", "update"]);
+    if ctx.config().yes(Step::System) {
+        cmd.arg("--assume=yes");
+    }
+    cmd.status_checked()?;
 
     Ok(())
 }
 
 fn upgrade_exherbo(ctx: &ExecutionContext) -> Result<()> {
     let sudo = require_option(ctx.sudo().as_ref(), REQUIRE_SUDO.to_string())?;
     ctx.run_type().execute(sudo).args(["cave", "sync"]).status_checked()?;
```

### Comparing `topgrade-12.0.1/src/steps/os/macos.rs` & `topgrade-12.0.2/src/steps/os/macos.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/os/openbsd.rs` & `topgrade-12.0.2/src/steps/os/openbsd.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/os/os_release/fedora` & `topgrade-12.0.2/src/steps/os/os_release/fedora`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/os/os_release/fedoraremixforwsl` & `topgrade-12.0.2/src/steps/os/os_release/fedoraremixforwsl`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/os/unix.rs` & `topgrade-12.0.2/src/steps/os/unix.rs`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,23 @@
         .status_checked()
 }
 
 pub fn run_home_manager(ctx: &ExecutionContext) -> Result<()> {
     let home_manager = require("home-manager")?;
 
     print_separator("home-manager");
-    ctx.run_type().execute(home_manager).arg("switch").status_checked()
+
+    let mut cmd = ctx.run_type().execute(home_manager);
+    cmd.arg("switch");
+
+    if let Some(extra_args) = ctx.config().home_manager() {
+        cmd.args(extra_args);
+    }
+
+    cmd.status_checked()
 }
 
 pub fn run_tldr(ctx: &ExecutionContext) -> Result<()> {
     let tldr = require("tldr")?;
 
     print_separator("TLDR");
     ctx.run_type().execute(tldr).arg("--update").status_checked()
```

### Comparing `topgrade-12.0.1/src/steps/os/windows.rs` & `topgrade-12.0.2/src/steps/os/windows.rs`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use color_eyre::eyre::Result;
 use etcetera::base_strategy::BaseStrategy;
 use tracing::debug;
 
 use crate::command::CommandExt;
 use crate::execution_context::ExecutionContext;
 use crate::terminal::{print_separator, print_warning};
-use crate::utils::require;
+use crate::utils::{require, which};
 use crate::{error::SkipStep, steps::git::Repositories};
 use crate::{powershell, Step};
 
 pub fn run_chocolatey(ctx: &ExecutionContext) -> Result<()> {
     let choco = require("choco")?;
     let yes = ctx.config().yes(Step::Chocolatey);
 
@@ -65,14 +65,18 @@
         ctx.run_type().execute(&scoop).args(["cleanup", "*"]).status_checked()?;
     }
 
     Ok(())
 }
 
 pub fn update_wsl(ctx: &ExecutionContext) -> Result<()> {
+    if !is_wsl_installed()? {
+        return Err(SkipStep("WSL not installed".to_string()).into());
+    }
+
     let wsl = require("wsl")?;
 
     print_separator("Update WSL");
 
     let mut wsl_command = ctx.run_type().execute(wsl);
     wsl_command.args(["--update"]);
 
@@ -83,14 +87,38 @@
     if ctx.config().wsl_update_use_web_download() {
         wsl_command.args(["--web-download"]);
     }
     wsl_command.status_checked()?;
     Ok(())
 }
 
+/// Detect if WSL is installed or not.
+///
+/// For WSL, we cannot simply check if command `wsl` is installed as on newer
+/// versions of Windows (since windows 10 version 2004), this commmand is
+/// installed by default.
+///
+/// If the command is installed and the user hasn't installed any Linux distros
+/// on it, command `wsl -l` would print a help message and exit with failure, we
+/// use this to check whether WSL is install or not.
+fn is_wsl_installed() -> Result<bool> {
+    if let Some(wsl) = which("wsl") {
+        // Don't use `output_checked` as an execution failure log is not wanted
+        #[allow(clippy::disallowed_methods)]
+        let output = Command::new(wsl).arg("-l").output()?;
+        let status = output.status;
+
+        if status.success() {
+            return Ok(true);
+        }
+    }
+
+    Ok(false)
+}
+
 fn get_wsl_distributions(wsl: &Path) -> Result<Vec<String>> {
     let output = Command::new(wsl).args(["--list", "-q"]).output_checked_utf8()?.stdout;
     Ok(output
         .lines()
         .filter(|s| !s.is_empty())
         .map(|x| x.replace(['\u{0}', '\r'], ""))
         .collect())
@@ -111,14 +139,18 @@
         command.arg("-y");
     }
 
     command.status_checked()
 }
 
 pub fn run_wsl_topgrade(ctx: &ExecutionContext) -> Result<()> {
+    if !is_wsl_installed()? {
+        return Err(SkipStep("WSL not installed".to_string()).into());
+    }
+
     let wsl = require("wsl")?;
     let wsl_distributions = get_wsl_distributions(&wsl)?;
     let mut ran = false;
 
     debug!("WSL distributions: {:?}", wsl_distributions);
 
     for distribution in wsl_distributions {
```

### Comparing `topgrade-12.0.1/src/steps/powershell.rs` & `topgrade-12.0.2/src/steps/powershell.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/remote/ssh.rs` & `topgrade-12.0.2/src/steps/remote/ssh.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/remote/vagrant.rs` & `topgrade-12.0.2/src/steps/remote/vagrant.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/tmux.rs` & `topgrade-12.0.2/src/steps/tmux.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/toolbx.rs` & `topgrade-12.0.2/src/steps/toolbx.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/upgrade.vim` & `topgrade-12.0.2/src/steps/upgrade.vim`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/vim.rs` & `topgrade-12.0.2/src/steps/vim.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/steps/zsh.rs` & `topgrade-12.0.2/src/steps/zsh.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/sudo.rs` & `topgrade-12.0.2/src/sudo.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/terminal.rs` & `topgrade-12.0.2/src/terminal.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/src/utils.rs` & `topgrade-12.0.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `topgrade-12.0.1/PKG-INFO` & `topgrade-12.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topgrade
-Version: 12.0.1
+Version: 12.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Upgrade all the things
 Keywords: upgrade,update
 Author: Roey Darwish Dror <roey.ghost@gmail.com>, Thomas Schönauer <t.schoenauer@hgs-wt.at>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: topgrade Version: 12.0.1 Classifier: Programming
+Metadata-Version: 2.1 Name: topgrade Version: 12.0.2 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE Summary: Upgrade all the things Keywords: upgrade,update
 Author: Roey Darwish Dror
 ghost@gmail.com>, Thomas SchÃ¶nauer
 schoenauer@hgs-wt.at> Author-email: Roey Darwish Dror
 ghost@gmail.com>, Thomas SchÃ¶nauer
```

