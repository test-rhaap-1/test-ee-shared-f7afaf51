# test-execution-environment-create-pull-request

Test execution environment to create a pull request

## What's included

### Ansible collections

| Collection | Version | Source |
|---|---|---|
| community.crypto | 2.15.1 | galaxy |

### Python packages

- `requests>=2.28.0`
- `pyyaml>=6.0`

### System packages

- `git`
- `openssh-clients`

## Details

- **Tags:** `execution-environment`, `test`, `existing-repo`


## Use this execution environment

To use this EE, build and push it to your container registry first, then add it in Ansible Automation Platform under Automation Execution > Infrastructure > Execution Environments.

To use it in Ansible Automation Platform:

1. Go to **Automation Execution** > **Infrastructure** > **Execution Environments**.
2. Click **Create execution environment** and enter the image URL.
3. Select this execution environment in your job templates.

## Build details

- **Base image:** `registry.redhat.io/ansible-automation-platform/ee-minimal-rhel9:2.18`
- **Definition file:** `test-execution-environment-create-pull-request.yml`
- **Template file:** `test-execution-environment-create-pull-request-template.yml` - import this into Ansible automation portal to let others create EEs from the same starting point.

To make changes, use this EE's template in Ansible automation portal or rebuild manually with `ansible-builder` and the definition file.
