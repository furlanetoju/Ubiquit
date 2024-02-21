# Ubiquit
Alguns comandos e como fazer alteração do endereço IP via SSH.

**Reiniciar o nano via SSH**
```
reboot
```

**Para resetar o nano via ssh**
```
cfgmtd -f /usr/etc/system.cfg -w && reboot
```

**Alterar uma configuração..ssid, nome do dispositivo, ip, etc...**
```
vi /tmp/system.cfg
```
Va até a linha q quer alterar e digite **i** depois para sair e salvar aperte **ESC** depois digite **:wq** para sair sem salvar nada aperte **ESC** depois digite **:q** depois de alterado o necessário, precisamos reiniciar o equipamento para aplicar as configurações com o comando abaixo:
```
save
/usr/etc/rc.d/rc.softrestart save
```
