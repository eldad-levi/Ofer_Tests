# Ofer_Tests

OTA distribution for OFER6.1 test devices.

Devices read `ota/version.json` on branch `main`. `enabled: 0` pauses updates.
When publishing an update, upload the application `.bin` first and update
`version.json` last. The manifest must contain `enabled`, `version`, `bin_url`,
`size` and `sha256`; its version must match `FW_VERSION` in the compiled firmware.
Use a version strictly newer than the installed firmware.

This repository is public. Do not upload the firmware configuration, API keys,
credentials, or the full private source ZIP. A compiled application can also
contain embedded credentials; treat published binaries accordingly.
