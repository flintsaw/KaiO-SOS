# Degoogling a Nokia 6300 4G
## Documenting attempts to degoogle KaiOS on a Nokia 6300 4G

- [ ] Enter debug mode - https://wiki.bananahackers.net/devices
    >*#*#33284#*#*
    
 **Use Temporary Root.** Per BananaHackers,
 ```
 NOTE that permanent root by replacing partitions voids the warranty and blocks updates, use at your own risk. Read and understand the guide carefully to be able to backup all partitions using the tools we provide, in case something goes wrong or if you want to re-enable official updates.
```



- [ ] Remove programs with ADB?
    Need to list all google, facebook,whatsapp, etc. files here
- [ ] IPtables to block tracking domains?



## Notes and Reference

If the necessary partition is read only try
```
  adb shell
  su
  mount -o remount,rw /system
```

Nokia 6300 4G - https://www.nokia.com/phones/en_us/nokia-6300-4g?sku=16LIOW11A01
BananaHackers debug mode - https://wiki.bananahackers.net/devices
BananaHackers EDL tools - https://wiki.bananahackers.net/development/edl



Device
    Developer
        Debugger
            ADB and DevTools 
