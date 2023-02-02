# Zabbix Template: N2WS CPM Backup alerts monitoring

# Overview

This template creates new Zabbix items to get alerts from N2WS's CPM Backup thorugh its API.

Tested on: 
* Zabbix 6.2

# Setup
See [Zabbix template operation](https://www.zabbix.com/documentation/6.2/manual/config/templates_out_of_the_box/http) for basic instructions.

Before using the template, you need to obtain a N2WS's CPM Backup API key. To do so, refer to the [N2WS Backup API documentation](https://support.n2ws.com/portal/en/kb/articles/cpm-restful-api-guide). 

# Zabbix configuration
No specific Zabbix configuration is required.

## Macros used
| Name       | Description                  | Default   |
|------------|------------------------------|-----------|
| {$API_KEY} | The CPM Backup API key.      | `<empty>` | 
| {$CPM_URL} | The CPM Backup endpoint URL. | `<empty>` |

## Template links
There are no template links in this template.

## Discovery rules
There are no discovery rules in this template.

## Items collected
| Name                      | Description                                       | Type   | Key and additional info |
|---------------------------|---------------------------------------------------|--------|-------------------------|
| Number of errors in CPM   | Retrieve the number of error alerts in CPM API    | Script | cpm.errors              |
| Number of warnings in CPM | Retrieve the number of warining alerts in CPM API | Script | cpm.warning             |

## Triggers
There are no triggers in this template.

# Feedback
Please report any issues with the template at https://github.com/emnavarro02/zabbix-script-n2ws-monitoring/issues.

You can also provide feedback, discuss the template or ask for help with it at ZABBIX forums.
