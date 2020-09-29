# Ansible Playbook Terraform module 
Terraform module which run a Ansible Playbook

## Terraform versions

Terraform 0.12

## Requirements

`ansible-playbook` ~> 2.9 on local machine.

## Providers

| Name | Version |
|------|---------|
| null | n/a |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| ansible\_host\_key\_checking | Ansible variable to host key checking | `bool` | `false` | no |
| ansible\_playbook\_path | ansible-playbook command path | `string` | `ansible-playbook` | no |
| ansible\_ssh\_retries | Ansible variable to retry SSH connection. This is important to wait SSH connections in new instances. | `number` | `30` | no |
| playbook | Path to playbook file. | `string` | n/a | yes |
| private\_key | Path to SSH private key file. | `string` | n/a | yes |
| remote\_host | Remote host IP or FQDN, for example, instance private IP. | `string` | n/a | yes |
| remote\_user | The remote user name. | `string` | n/a | yes |
| trigger | Information to trigger execution, for example, EC2 instance ID or some timestamp. | `string` | n/a | yes |

## Outputs

No output.

## Authors

Module managed by [Bruno Dias](https://github.com/brunordias).

## License

Apache 2 Licensed. See LICENSE for full details.