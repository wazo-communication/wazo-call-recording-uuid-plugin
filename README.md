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

## Uninstallation

```sh
wazo-plugind-cli -c "uninstall wazocommunication/wazo-call-recording-uuid"
```
