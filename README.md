Syntax highlighting for Ansible files
=====================================

## Screenshot

With color scheme Monokai

![Screenshot](https://raw.githubusercontent.com/clifford-github/sublime-ansible/master/doc/images/ansible-syntax.png)

## Installation

I recommend install another package along with this one, "Apply Syntax" package since this syntax does not take ownership of yml nor yaml files.

### Package Control manager

First, install the Package Control plugin, instructions here: https://packagecontrol.io/installation.

Once you install Package Control, restart Sublime Text and bring up the Command Palette (`Command+Shift+P` on macOS, `Control+Shift+P` on GNU/Linux|Windows).

Select "Package Control: Install Package", wait while Package Control fetches the latest package list, then select "Ansible" when the list appears.

The advantage of using this method is that Package Control will automatically keep this package up to date with the latest version.

### Manual
Clone the repository in your Sublime Text "Packages" directory:

    git clone https://github.com/clifford-github/sublime-ansible.git Ansible

The "Packages" directory can be located from Command Palette:

* macOS: `Shift + Command + P`
* GNU/Linux | Windows: `Shift + Control + P`

Type `browse packages`

That should give you the location of your Packages directory.

### Apply Syntax helper

This is an example to automatic select Ansible Syntax

        "syntaxes": [
                {
                    "syntax": [
                        "Ansible/Ansible"
                    ],
                    "rules": [
                      {"file_path": ".*/(inventory|tasks|handlers|files|templates|roles|playbooks|.*_vars)/.*\\.y(a)?ml$"}
                    ]
                }
            ]
