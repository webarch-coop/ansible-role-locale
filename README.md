# Ansible Locale Role

This role sets the value of `LANG` in `/etc/default/locale` and for the systemd
environment (`systemctl show-environment`) to the value of `locale_lang`, see 
the [defaults/main.yml](defaults/main.yml). 

