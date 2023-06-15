postgresql
=================

Setup PostgreSQL

OS Platform
-----------------

### Debian

- bookworm
- bullseye

Role Variables
--------------

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードを参照してください。

### `postgresql_packages`

インストールするパッケージ

### `postgresql_default_charset`

デフォルトのcharset

### `postgresql_databases`

データベースの設定

### `postgresql_users`

ユーザーの設定

### `postgresql_max_connections`

max_connectionsの設定値

### `postgresql_shared_buffers_rate`

shared_buffersの設定値の自動算出に利用

### `postgresql_effective_cache_size_rate`

effective_cache_sizeの設定値の自動算出に利用

### `postgresql_maintenance_work_mem_rate`

maintenance_work_memの設定値の自動算出に利用

### `postgresql_strage_type`

random_page_costおよびeffective_io_concurrency設定値の自動設定に利用

### `postgresql_cfg`

postgresql.confの設定  
@see https://pgtune.leopard.in.ua/

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
