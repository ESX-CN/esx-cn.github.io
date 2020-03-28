# F.A.Q

以下是一些常见问答

## FXServer 启动顺序

当你下载脚本的时候，特别是 **ESX脚本** 有“要求(Requirements)”。这对它们的正常运行至关重要。`server.cfg` 中脚本的开始顺序很 _**重要**_ 。脚本的安装要求必须高于需要它的脚本，如果在它之后加载，脚本可能无法正常工作。所以正确的开始顺序是至关重要的。

??? note "示例 server.cfg"
    ```
    endpoint_add_tcp "0.0.0.0:30120"
    endpoint_add_udp "0.0.0.0:30120"
    sv_listingIPOverride "YOUR_IP_ADRESS"

    set sv_licenseKey "XXXXXXXXXXXXXXXXXXX" # https://keymaster.fivem.net/
    set steam_webApiKey "none"
    set mysql_connection_string "server=adress;database=dbname;userid=user;password=psswd"

    sv_maxClients 5
    sv_hostname "Your Server Label"
    sv_scriptHookAllowed 0
    sv_endpointPrivacy true

    add_principal group.admin group.user
    add_ace resource.es_extended command.add_ace allow
    add_ace resource.es_extended command.add_principal allow
    add_ace resource.es_extended command.remove_principal allow

    #### FIVEM DEFAULT ####
        start chat
        start sessionmanager
        restart sessionmanager
        start hardcap

    #### ESSENTIAL
        start mysql-async
        start es_extended

    #### ESX REQUIRED MODS
        start instance
        start cron
        start skinchanger
        start esx_skin
        start esx_menu_default
        start esx_menu_list
        start esx_menu_dialog
        start esx_phone
        start esx_addonaccount
        start esx_addoninventory
        start esx_datastore
        start esx_society
        start esx_service
        start esx_billing

    #### ESX JOBS
        start esx_jobs
        start esx_joblisting
        start esx_taxijob
        start esx_mecanojob
        start esx_policejob
        start esx_property
        start esx_realestateagentjob
        start esx_bankerjob
        start esx_ambulancejob
        start esx_vehicleshop

    #### ESX ANY OTHER MODS
        start esx_status
        start esx_basicneeds
        start esx_clotheshop
        start esx_garage
        start esx_holdup
        start esx_drugs
        start esx_atm

    #### ANY NON ESX MODS
        #start nonESXmod
    ```
