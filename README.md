postgresql
=================

Setup PostgreSQL

OS Platform
-----------------

### Debian

- bullseye
- buster

Role Variables
--------------

### `postgresql_packages`

インストールするパッケージ

### `postgresql_default_charset`

デフォルトのcharset

### `postgresql_databases`

データベースの設定

### `postgresql_users`

ユーザーの設定

### `postgresql_cfg`

pg_hba.confの設定

### `postgresql_pg_hba_cfg`

pg_hba.confの設定

### `postgresql_pg_ident_cfg`

pg_ident.confの設定

### `postgresql_pg_ctl_cfg`

pg_ctl.confの設定

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: postgresql
```

License
--------------

Apache License 2.0
