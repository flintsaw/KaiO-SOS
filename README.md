# Degoogling a Nokia 6300 4G
## Documenting attempts to degoogle KaiOS on a Nokia 6300 4G

- [ ] Enter debug mode - Need link to babanahackers
- [ ] Remove programs with ADB?
    - [ ] Need to list all google, facebook,whatsapp, etc. files here
- [ ] IPtables to block tracking domains?



## Notes and Reference

If the necessary partition is read only try
```
  adb shell
  su
  mount -o remount,rw /system
```

Nokia 6300 4G
https://www.nokia.com/phones/en_us/nokia-6300-4g?sku=16LIOW11A01
