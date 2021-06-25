# Zabbix Template for monitoring Active User Status by Zabbix Agent active

This template uses `system.run` to run `last` command on server and get logged in users information:

1. Monitor Items
    1. Logged in users List
        1. Num of Active(logged in) users
        1. Overstay users on the {HOST.NAME} > {$OVERSTAY_THRESHOLD} day(s)
            1. Num of overstay users on the {HOST.NAME} > {$OVERSTAY_THRESHOLD} day(s)
                - Triggers
                    Some users overstay on the {HOST.NAME} > {$OVERSTAY_THRESHOLD} day(s)

## Tested version

- Zabbix: `5.0.1`

## Useage

1. Import Templates: Zabbix Web Page --> [Configuration] --> [Templates] --> [Import] this xml file
1. Link this template to an existing host or a new host
1. Update the Macro to specify your Harbor info: [Configuration] --> your host --> [Macros] --> [Inherited and host macros]
    - {$OVERSTAY_THRESHOLD}
