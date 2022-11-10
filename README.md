# Degoogling a Nokia 6300 4G
## Documenting attempts to increase KaiOS privacy on a Nokia 6300 4G

- [ ] Enter debug mode - https://wiki.bananahackers.net/devices
    >*#*#33284#*#*
    
 **Use Temporary Root.** Per BananaHackers,
 ```
 NOTE that permanent root by replacing partitions voids the warranty and blocks updates, use at your own risk. Read and understand the guide carefully to be able to backup all partitions using the tools we provide, in case something goes wrong or if you want to re-enable official updates.
```



- [ ] Remove programs with ADB?
    Need to list all google, facebook,whatsapp, etc. files here
- [ ] IPtables to block tracking domains?
Does manifest.webapp contain anything useful for removing unwanted code?


## Notes and Reference

This process only works on non-US versions. **Use information below at your own risk.**
TA-1286 - I think this one works but cannot verify.
TA-1287 - I think this one works but cannot verify.
TA-1291 - I think this one works but cannot verify.
TA-1294 - I think this one works but cannot verify.
TA-1307 - Not sure...
TA-1324 - DOES NOT WORK!

If the necessary partition is read only try
```
  adb shell
  su
  mount -o remount,rw /system
```

Nokia 6300 4G - https://www.nokia.com/phones/en_us/nokia-6300-4g?sku=16LIOW11A01
BananaHackers debug mode - https://wiki.bananahackers.net/devices
BananaHackers EDL tools - https://wiki.bananahackers.net/development/edl
BananaHackers EDL downloads - https://edl.bananahackers.net/

https://developer.kaiostech.com/docs/getting-started/main-concepts/manifest/
https://developer.kaiostech.com/docs/getting-started/main-concepts/permissions/


Device
    Developer
        Debugger
            ADB and DevTools 

Hostile programs
Kaiads
Whatsapp
Facebook
Google

Directory           Permissions
/system/etc         ?

