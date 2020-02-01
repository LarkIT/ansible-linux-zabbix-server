# Lark IT Ansible Zabbix Server Role

Install and configure Zabbix server

## Operating Systems
This role is known to work on the following operating systems:
- CentOS 7

## Dependencies
This role depends on the following Ansible Galaxy roles:
- dj-wasabi.zabbix-server (https://galaxy.ansible.com/dj-wasabi/zabbix-server)

## Variables
| Variable | Required? | Default Value | Type | Description |
|----------|--------|-------|------|--------|
| zabbix_version | Optional | 4.2 | String | Zabbix package major version |
| zabbix_server_opsgenie_integration | Optional | false | Boolean | Wheter or not to include OpsGenie integration configuration |
| zabbix_server_opsgenie_api_key | When zabbix_server_opsgenie_integration is true | N/A | Sring | OpsGenie API key |
| zabbix_server_opsgenie_command_url | When zabbix_server_opsgenie_integration is true | N/A | String | The Zabbix URL the OpsGenie plugin should use to execute commands on Zabbix |
| zabbix_server_opsgenie_user | When zabbix_server_opsgenie_integration is true | opsgenie | String | The Zabbix user that the OpsGenie plugin uses to authenticate 
| zabbix_server_opsgenie_password | When zabbix_server_opsgenie_integration is true | N/A | String | The Zabbix password that the OpsGenie plugin uses to authenticate |

Refer to Galaxy role documentation for other variables