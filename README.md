> isc_user=SYSDBA

> isc_password=masterkey

> gfix -v -f banco.fdb

> gfix -n -i banco.fdb

> gbak -g -b -z -l -v banco.fdb banco.fbk

> gbak -g -c -z -v banco.fbk banco.fdb
