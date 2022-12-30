# grafana-dashboards-backup

**This is the playbook/role for downloading all the dashboards from the grafana using ansible**


**Table of Content**
- [Prerquisite](#pre-requisite)
- [Passing inputs for the role](#passing-inputs-for-the-role)
- [Using main playbook that calls this roll](#using-main-playbook-that-calls-this-roll)
- [Executing playbook.yml](#executing-playbookyml)
- [Output files](#output-files)

## Pre-requisite ##

Python 3, ansible

## Passing inputs for the role ##

There is a postdeploy.yml file in the main dir -- replaced the grafana_base_url, SROuser, SROpassword value with your deployment details.

## Using main playbook that calls this roll ##

For ease of using roll added a playbook with name playbook.yml you can directly call with ansible-playbook command it will call the role by itself.

## Executing playbook.yml ##

> ansible-playbook playbook.yml

## Output files ##

All the dashboards will be dumped in the /tmp/dashboard dir