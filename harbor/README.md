# Zabbix Template for Harbor

This template uses http agent to get informations from [Harbor](https://goharbor.io/) API, such as:

1. Monitor Items
    1. Health of services: Core, Jobservice, Redis, Database, Portal, ..., etc
    1. System information: Version, Regitstry URL, Has CA Root, ..., etc
    1. Statistic: Public/Private Project and Repository count
1. Triggers
    1. Unhealthy Services
    1. Every operations on Harbor (excluding pulling images `PULL_ARTIFACT`)

# Useage

Zabbix Web Page --> [Configuration] --> [Templates] --> [Import] this xml file

# Reference

- [View and Test the Harbor REST API via Swagger](https://goharbor.io/docs/1.10/build-customize-contribute/configure-swagger/)
- [Zabbix - HTTP AGENT](https://www.zabbix.com/documentation/current/manual/config/items/itemtypes/http)