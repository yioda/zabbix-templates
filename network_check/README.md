# Template for Network Checking

These Templates uses for agent network checking.

1. `zbx_internet_check_templates.xml`
    1. Check internet available
        - Default, check Google DNS Server `8.8.8.8:53` per 5 minute, you could change by overriding macro `{$INTERNET_CHECK_TARGET_HOST}` & `{$INTERNET_CHECK_TARGET_PORT}`


## Reference

- [Zabbix - ZABBIX AGENT](https://www.zabbix.com/documentation/current/manual/config/items/itemtypes/zabbix_agent)