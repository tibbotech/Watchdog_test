# Watchdog_test
'The watchdog is a powerful tool that can reboot your device in case it hangs up.
'On ARM-based platforms the watchdog is NOT running by default.
'This is because once the watchdog is enabled it can't be disabled except through reboot, and this will interfere with putting
'the device into the standby mode using sys.standby (the watchdog will keep resetting the device --
'sometimes you want this, and sometimes you don't).

'TiOS will take care of resetting the watchdog, unless you want your app to handle the watchdog "manually".
'This app demonstrates the switchover into the "manual" watchdog control.