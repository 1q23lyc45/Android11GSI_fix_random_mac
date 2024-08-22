# Android11GSI_fix_random_mac
This module fixes the issue where the Android 11 GSI cannot use the random MAC address function on some phones.

## Software principle:
Modify the /system/system_ext/apex/com.android.wifi/priv-app/ServiceWifiResources/ServiceWifiResources.apk to change all resources.arsc bool options with 'mac_randomize' to true. 
Due to the inability to implement dynamic replacement, I put the modified file in advance.

This module only supports Android 11. For other Android versions, you can manually change the APK implementation according to my method.
