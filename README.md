1: Conectar no banco de dados
> isc_user=SYSDBA
> isc_password=masterkey

2: Verificação de corrupção da base
> gfix -v -f banco.fdb

3: Correção da corrupção da base
> gfix -n -i banco.fdb

4: Realização de backup da base
> gbak -g -b -z -l -v banco.fdb banco.fbk

5: Restauração de backup da base
> gbak -g -c -z -v banco.fbk banco.fdb
