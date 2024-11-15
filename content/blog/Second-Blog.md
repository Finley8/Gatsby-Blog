---
title: Pipx Commands and How to Use Them
date: "2024-11-11T22:40:32.169Z"
description: This is a description of commands that you can use in Pipx and what these commands will do.
---

## Introduction

This blog will help you learn about pipx commands and will give you a description of what each command does. Pipx is a really simple and powerful tool for running commands as an executable from an isolated environment. Those commands should be associated with a python package that has CLI. In pipx, we install the package once and we can use the package anywhere on our system isolated from other virtual environments.

## How to Install Pipx

It is very simple to install. All you will need to do is navigate to your terminal and type `pip install pipx`.

You can check if it is installed by running `pipx --version`. If you do not get an error then you have successfully installed pipx.

## Primary Commands

```python
  PIPX_HOME              Overrides default pipx location. Virtual Environments
                        will be installed to $PIPX_HOME/venvs.
  PIPX_GLOBAL_HOME       Used instead of PIPX_HOME when the `--global` option
                        is given.
  PIPX_BIN_DIR           Overrides location of app installations. Apps are
                        symlinked or copied here.
  PIPX_GLOBAL_BIN_DIR    Used instead of PIPX_BIN_DIR when the `--global`
                        option is given.
  PIPX_MAN_DIR           Overrides location of manual pages installations.
                        Manual pages are symlinked or copied here.
  PIPX_GLOBAL_MAN_DIR    Used instead of PIPX_MAN_DIR when the `--global`
                        option is given.
  PIPX_DEFAULT_PYTHON    Overrides default python used for commands.
  USE_EMOJI              Overrides emoji behavior. Default value varies based
                        on platform.
  PIPX_HOME_ALLOW_SPACE  Overrides default warning on spaces in the home path

options:
  -h, --help            show this help message and exit
  --quiet, -q           Give less output. May be used multiple times
                        corresponding to the ERROR and CRITICAL logging
                        levels. The count maxes out at 2.
  --verbose, -v         Give more output. May be used multiple times
                        corresponding to the INFO, DEBUG and NOTSET logging
                        levels. The count maxes out at 3.
  --global              Perform action globally for all users.
  --version             Print version and exit

subcommands:
  Get help for commands with pipx COMMAND --help
    install             Install a package
    install-all         Install all packages
    uninject            Uninstall injected packages from an existing Virtual
                        Environment
    inject              Install packages into an existing Virtual Environment
    pin                 Pin the specified package to prevent it from being
                        upgraded
    unpin               Unpin the specified package
    upgrade             Upgrade a package
    upgrade-all         Upgrade all packages. Runs `pip install -U <pkgname>`
                        for each package.
    upgrade-shared      Upgrade shared libraries.
    uninstall           Uninstall a package
    uninstall-all       Uninstall all packages
    reinstall           Reinstall a package
    reinstall-all       Reinstall all packages
    list                List installed packages
    interpreter         Interact with interpreters managed by pipx
    run                 Download the latest version of a package to a
                        temporary virtual environment, then run an app from
                        it. Also compatible with local `__pypackages__`
                        directory (experimental).
    runpip              Run pip in an existing pipx-managed Virtual
                        Environment
    ensurepath          Ensure directories necessary for pipx operation are in
                        your PATH environment variable.
    environment         Print a list of environment variables and paths used
                        by pipx.
    completions         Print instructions on enabling shell completions for
                        pipx
```

You can also find this list of commands inside of your terminal by typing `pipx -h`.
