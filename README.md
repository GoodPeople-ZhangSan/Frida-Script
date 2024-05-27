# Frida-Script

Some common frida scripts



- hook_RegisterNatives.js
  - 需要以span的方式hook：`frida -U --no-pause -f com.xxx.xxx -l hook_RegisterNatives.js`
  - 如果遇见Failed to spawn: unexpectedly timed out while waiting for app to launch的问题，如下解决
  - `adb shell`下输入`setprop persist.device_config.runtime_native.usap_pool_enabled false`

