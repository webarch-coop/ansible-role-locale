# Webarchitects Ansible locale role

[![pipeline status](https://git.coop/webarch/locale/badges/master/pipeline.svg)](https://git.coop/webarch/locale/-/commits/master)

This role sets the `debconf` default locale, generates the specified locale, sets the value of `LANG` in `/etc/default/locale` and sets the value of `LANG` for the systemd environment (`systemctl show-environment`) to the value of `locale_lang`.

## Role variables

See the [defaults/main.yml](defaults/main.yml) file for the default variables and [meta/argument_spacs.yml](meta/argument_specs.yml) for the variable specification.

### locale

Set the `locale` variable to `false` to prevent any tasks in this role being run, this variable defaults to `true`.

### locale_lang

The `locale_lang` defaults to `en_GB.UTF-8`.

### locale_language

The `locale_language` defaults to `en_GB:en`.

## Requirements

This role requires [JC](https://github.com/kellyjonbrazil/jc) version [1.22.0](https://github.com/kellyjonbrazil/jc/releases/tag/v1.22.0) or greater, installed via `pip3`, to be present on the Ansible controller.

## Repository

The primary URL of this repo is [`https://git.coop/webarch/locale`](https://git.coop/webarch/locale) however it is also [mirrored to GitHub](https://github.com/webarch-coop/ansible-role-locale) and [available via Ansible Galaxy](https://galaxy.ansible.com/chriscroome/locale).
If you use this role please use a tagged release, see [the release notes](https://git.coop/webarch/locale/-/releases).

## License

This role is released under [the same terms as Ansible itself](https://github.com/ansible/ansible/blob/devel/COPYING), the [GNU GPLv3](LICENSE).

