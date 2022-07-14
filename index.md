## adb access by adding permission

### steps:
1. From the host pc.
        cat ~/.android/adbkey.pub
2. Copy the above pubkey.
3. From the target serial console
         cd /data/misc/adb
         echo "copied host pubkey"  >  adb_keys
         chmod 0644 adb_keys
         reboot 
4. after this you should able to access the device through adb
