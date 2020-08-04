# Ansible Locale Role

This role runs [tasks](tasks/main.yml) which set the Debconf default locale,
generates the specified locale, sets the value of `LANG` in
`/etc/default/locale` and sets the value of `LANG` for the systemd environment
(`systemctl show-environment`) to the value of `locale_lang`, see the
[defaults/main.yml](defaults/main.yml). 
