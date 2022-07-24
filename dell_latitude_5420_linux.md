# Dell Latitude 5420

OS: Ubuntu 20.04

## Setup fingerprint reader

Download the latest driver from http://dell.archive.canonical.com/updates/pool/public/libf/libfprint-2-tod1-broadcom/ server.

For Ubuntu:

- Install the driver
  ```
  sudo dpkg -i libfprint-2-tod1-broadcom_5.8.012.0-0ubuntu1_oem2_amd64.deb
  ```
- Reboot
- Enroll your right index fingerprint
  ```
  fprintd-enroll
  ```

Note:

If you get the following error, which means the driver is not installed properly

```
Impossible to enroll: GDBus.Error:net.reactivated.Fprint.Error.NoSuchDevice: No devices available
```
