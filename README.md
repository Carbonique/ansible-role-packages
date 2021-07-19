- [About](#about)
- [Installation](#installation)
- [Defaults](#defaults)
- [Variables](#variables)

# About

This role install specified apt and pip packages.

# Installation

Add the following to `requirements.yml`:

```
- src: git@gitlab.com:carbonique/ansible-role-packages.git
  scm: git
  name: packages
  version: #Leave empty for latest. To download a specific version: use the tag as listed in repo
```

For system wide installation:
`ansible-galaxy install -r requirements.yml`

For installation to the current directory:
`ansible-galaxy install --roles-path . -r requirements.yml`

# Defaults

Defaults have been prefilled. Variables have to be added by user

For defaults see: `defaults/main.yml`
For variables see: `vars/main.yml`






# Variables

For defaults see `defaults/main.yml`.

| Variable           | Description                                                                                                    | Default                  | Optional/Required |   |
|--------------------|----------------------------------------------------------------------------------------------------------------|--------------------------|-------------------|---|
| install_apt_packages    | List of packages to install                                 | null                     | Required          |   | Optional
| install_pip_packages      | List of packages to install                                                                                         |             | Optional          |   |