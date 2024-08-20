# wazo-call-recording-uuid-plugin

Migrate the call recording UUIDs so that they match the file names on the file
system.

## Installation

```sh
wazo-plugind-cli -c "install git https://github.com/wazo-communication/wazo-call-recording-uuid-plugin"
```

Installing this plugin does not cause interruption of service.

This plugin adds a new CLI command `wazo-migrate-recording-uuid` that can be
used to synchronize recording UUIDs manually. This command will be executed
automatically upon installation and can be used afterwards.

After the migration, the call recording UUIDs exposed in the wazo-call-logd API
will be changed.

This plugin is only useful for Wazo servers installed before 24.12. Recording
UUIDs created after Wazo 24.12 are automatically synchronized and do not need
migration.

## Uninstallation

```sh
wazo-plugind-cli -c "uninstall wazocommunication/wazo-call-recording-uuid"
```
