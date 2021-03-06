# Project: terra4aws64

```text
 ███████████                                        █████ █████       █████████   █████   ███   █████  █████████      ████████  █████ █████
░█░░░███░░░█                                       ░░███ ░░███       ███░░░░░███ ░░███   ░███  ░░███  ███░░░░░███    ███░░░░███░░███ ░░███
░   ░███  ░   ██████  ████████  ████████   ██████   ░███  ░███ █    ░███    ░███  ░███   ░███   ░███ ░███    ░░░    ░███   ░░░  ░███  ░███ █
    ░███     ███░░███░░███░░███░░███░░███ ░░░░░███  ░███████████    ░███████████  ░███   ░███   ░███ ░░█████████    ░█████████  ░███████████
    ░███    ░███████  ░███ ░░░  ░███ ░░░   ███████  ░░░░░░░███░█    ░███░░░░░███  ░░███  █████  ███   ░░░░░░░░███   ░███░░░░███ ░░░░░░░███░█
    ░███    ░███░░░   ░███      ░███      ███░░███        ░███░     ░███    ░███   ░░░█████░█████░    ███    ░███   ░███   ░███       ░███░
    █████   ░░██████  █████     █████    ░░████████       █████     █████   █████    ░░███ ░░███     ░░█████████    ░░████████        █████
   ░░░░░     ░░░░░░  ░░░░░     ░░░░░      ░░░░░░░░       ░░░░░     ░░░░░   ░░░░░      ░░░   ░░░       ░░░░░░░░░      ░░░░░░░░        ░░░░░
```

## Overview

Collection of Terraform AWS modules for deploying common infrastructure landscapes.

| Module                                                                        | Purpose                                                                                                 |
| ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| [terraform-aws-ami](https://github.com/terra4aws64/terraform-aws-ami)         | Terraform module for creating a curated catalog of AWS AMIs                                             |
| [terraform-aws-aurora](https://github.com/terra4aws64/terraform-aws-aurora)   | Terraform module for creating AWS RDS Aurora clusters                                                   |
| [terraform-aws-bastion](https://github.com/terra4aws64/terraform-aws-bastion) | Terraform module for creating a dedicated Bastion host for managing private hosts in the target AWS VPC |
| [terraform-aws-ec2](https://github.com/terra4aws64/terraform-aws-ec2)         | Terraform module for creating AWS EC2 instances                                                         |
| [terraform-aws-ec2-as](https://github.com/terra4aws64/terraform-aws-ec2-as)   | Terraform module for creating AWS EC2 Auto Scaling Groups                                               |
| [terraform-aws-vpc](https://github.com/terra4aws64/terraform-aws-vpc)         | Terraform module for creating AWS VPCs                                                                  |

## Development

### Repositories

- Project GIT repository: [https://github.com/serdigital64/terra4aws64](https://github.com/serdigital64/terra4aws64)
- Project Documentation: [https://github.com/serdigital64/terra4aws64](https://github.com/serdigital64/terra4aws64)
- Terraform Namespace: [https://registry.terraform.io/namespaces/terra4aws64](https://registry.terraform.io/namespaces/terra4aws64)

### Environment

- Prepare dev tools:
  - Install the latest version of the [Terraform CLI](https://www.terraform.io/downloads)
  - Install GIT
  - (Optional) Install Git Flow
- Clone GIT repositories

  ```shell
  # Create the main repository
  cd <YOUR_PROJECTS_PATH>
  git clone https://github.com/serdigital64/terra4aws64.git
  # Create module repositories as git submodules
  git submodule init
  # Update modules
  git submodule update
  # Enable main branch on submodules
  git submodule foreach "git checkout main"; git submodule foreach "git checkout develop"
  # (Optional) Initialize git flow. Production branch:main, use defaults for the remaining branches
  git submodule foreach "git flow init"
  ```

- Adjust environment variables to reflect your configuration:

  ```shell
  # Copy environment definition files from templates:
  cp dot.local .local
  cp dot.secrets .secrets
  # Review and update content for both files
  ```

- Initialize dev environment variables

  ```shell
  source bin/devta64-set
  ```

### Contributing

Help on implementing new features and maintaining the code base is welcomed.

[Contributor Covenant Code of Conduct](./CODE_OF_CONDUCT.md)

### License

[GPL-3.0-or-later](https://www.gnu.org/licenses/gpl-3.0.txt)

### Author

- [SerDigital64](https://serdigital64.github.io/)
