```bash
sudo ./tuya-cloudcutter.sh
```
```
Loading options, please wait...
[?] Select your custom firmware file: OpenBK7231N_UG_1.15.523.bin
 > OpenBK7231N_UG_1.15.523.bin
 ```
 
 ```bash
[?] How do you want to choose the device?: By firmware version and name
   By manufacturer/device name
 > By firmware version and name
   From device-profiles (i.e. custom profile)
```

```bash
[?] Select the firmware version and name: 1.1.8 - BK7231N / oem_bk7231n_plug
   1.1.6 - BK7231T / oem_bk7231s_switch1_zero_kjd
   1.1.7 - BK7231N / CL_DREAM_RGB_STRIP_19KEY_1KEY_5V_BK7231N
   1.1.7 - BK7231N / oem_bk7231n_ceiling_light_ty
   1.1.7 - BK7231N / oem_bk7231n_plug
   1.1.7 - BK7231T / oem_bk7231s_light_pir_ty
   1.1.71 - BK7231T / bk7231t_common_user_config_ty
 > 1.1.8 - BK7231N / oem_bk7231n_plug
   1.1.8 - BK7231T / oem_bk7231s_rnd_switch
   1.1.80 - BK7231T / bk7231t_common_user_config_ty
   1.1.9 - BK7231N / oem_bk7231n_water_sensor_plus
   1.1.9 - BK7231T / bk7231s_common_iot_config_ty
   1.1.9 - BK7231T / oem_bk7231s_ceiling_light_ty
   1.2.1 - BK7231N / oem_bk7231n_control_switch
```

```bash
[?] Select the brand of your device: Tuya Generic
   Atarm
   Aubess
   Baytion
   Nous
   QNCX
   Topgreener
 > Tuya Generic
```

```bash
[?] Select the article number of your device: LSPA7 Plug
   BSD48 16A UK Smart Plug
 > LSPA7 Plug
```

```bash
Selected Device Slug: tuya-generic-lspa7-plug
Selected Profile: oem-bk7231n-plug-1.1.8-sdk-2.3.1-40.00
Selected Firmware: /work/custom-firmware/OpenBK7231N_UG_1.15.523.bin
```

```bash
================================================================================
Place your device in AP (slow blink) mode.  This can usually be accomplished by either:
Power cycling off/on - 3 times and wait for the device to fast-blink, then repeat 3 more times.  Some devices need 4 or 5 times on each side of the pause
Long press the power/reset button on the device until it starts fast-blinking, then releasing, and then holding the power/reset button again until the device starts slow-blinking.
See https://support.tuya.com/en/help/_detail/K9hut3w10nby8 for more information.
================================================================================

Scanning for open Tuya SmartLife AP
............
Found access point name: "SmartLife-8398", trying to connect...
Device 'wlo1' successfully activated with 'da693edb-478c-4236-9c87-0d6d43459b4a'.
Connected to access point.
Waiting 1 sec to allow device to set itself up...
Running initial exploit toolchain...
Exploit run, saved device config too!
output=/work/configured-devices/uAtHaXVDgCTp.deviceconfig
Saved device config in /work/configured-devices/uAtHaXVDgCTp.deviceconfig

================================================================================
Power cycle and place your device in AP (slow blink) mode again.  This can usually be accomplished by either:
Power cycling off/on - 3 times and wait for the device to fast-blink, then repeat 3 more times.  Some devices need 4 or 5 times on each side of the pause
Long press the power/reset button on the device until it starts fast-blinking, then releasing, and then holding the power/reset button again until the device starts slow-blinking.
See https://support.tuya.com/en/help/_detail/K9hut3w10nby8 for more information.
================================================================================

Scanning for open Tuya SmartLife AP
.........
Found access point name: "A-8398", trying to connect...
Device 'wlo1' successfully activated with '0c19d87c-f0c7-4d1e-b899-d788c491bf58'.
Connected to access point.
Configured device to connect to 'cloudcutterflash'
Device is connecting to 'cloudcutterflash' access point. Passphrase for the AP is 'abcdabcd' (without ')
Checking UDP port 53... Occupied by systemd-resolve with PID 661.
Port 53 is needed to resolve DNS queries
Do you wish to terminate systemd-resolve? [y/N] y
```

```bash
Attempting to stop systemd-resolved.service
Checking UDP port 67... Available.
Checking TCP port 80... Available.
Checking TCP port 443... Available.
Checking TCP port 1883... Available.
Checking TCP port 8886... Available.
Flashing custom firmware...

================================================================================
Wait for up to 10-120 seconds for the device to connect to 'cloudcutterflash'. This script will then show the firmware upgrade requests sent by the device.
================================================================================

Using WLAN adapter: wlo1
Configuration file: /dev/stdin
Using interface wlo1 with hwaddr 6c:6a:77:42:37:36 and ssid "cloudcutterflash"
wlo1: interface state UNINITIALIZED->ENABLED
wlo1: AP-ENABLED 
Using PSK v1 - Received PSK ID version 01
Processing endpoint /v2/url_config
Processing endpoint tuya.device.active
Processing endpoint tuya.device.dynamic.config.get
Processing endpoint tuya.device.uuid.pskkey.get
[MQTT Sending] Triggering firmware update message.
Processing endpoint tuya.device.upgrade.get
Processing endpoint tuya.device.upgrade.status.update
Processing endpoint /files/OpenBK7231N_UG_1.15.523.bin
Firmware update progress: 30%
Firmware update progress: 60%
Firmware update progress: 89%
[Firmware Upload] /files/OpenBK7231N_UG_1.15.523.bin send complete, request range: bytes=0-620511/620512
Processing endpoint tuya.device.upgrade.silent.get
Processing endpoint atop.online.debug.log
Processing endpoint tuya.device.dynamic.config.get
Processing endpoint tuya.device.dynamic.config.ack
Processing endpoint tuya.device.timer.count
Firmware update progress: 98%
Firmware file has been sent and MQTT reported a progress of nearly complete.  Waiting 15 seconds to ensure flashing completes.
Flashing should be complete.  It takes about 15 seconds for the device to reboot and verify the flash was valid.
Please wait about 30 seconds then look for signs of activity from the firmware you supplied (either watch for AP mode or check if it joined your network).
Device MAC address: 1c:90:ff:76:83:98
```
