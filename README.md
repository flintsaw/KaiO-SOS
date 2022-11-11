# WORK IN PROCESS AND MAY NOT WORK! Documenting attempts to increase KaiOS privacy on a Nokia 6300 4G. <br />


### This guide is for Linux but Windows and Mac users can follow along and reference the guides at the end if they get stuck. <br />

####NON-ROOT app removal
"removable": false,
- [ ] Install ADB
- [ ] Install WebIDE - https://sites.google.com/view/bananahackers/development/webide
- [ ] Enter debug mode
    >*#*#33284#*#*
- [ ] Use Wallace-Lite to get Temporary Root
- [ ] Pull existing webapps.json file
    >adb pull adb pull data/local/webapps/webapps.json
- [ ] For every app you want to remove, change the "removable": false value to true.
- [ ] 





This process only works on non-US versions. **Use at your own risk.** <br />
:heavy_check_mark: TA-1286 - I think this one works but cannot verify. <br />
:heavy_check_mark: TA-1287 - I think this one works but cannot verify. <br />
:heavy_check_mark: TA-1291 - I think this one works but cannot verify. <br />
:heavy_check_mark: TA-1294 - I think this one works but cannot verify. <br />
:question: TA-1307 - Not sure... <br />
:x: TA-1324 - DOES NOT WORK! <br />
















 **Use Temporary Root.** Per BananaHackers,
 ```
 NOTE that permanent root by replacing partitions voids the warranty and blocks updates, use at your own risk. Read and understand the guide carefully to be able to backup all partitions using the tools we provide, in case something goes wrong or if you want to re-enable official updates.
```



- [ ] Remove programs with ADB?
    Need to list all google, facebook,whatsapp, etc. files here
- [ ] IPtables to block tracking domains?
Does manifest.webapp contain anything useful for removing unwanted code?

##Apps worth adding/replacing https://store.bananahackers.net/ <br />
Wallace Toolbox <br />
AppBuster <br />
FastContact <br />
FastLog <br />
KaiAuth <br />
RSS Reader by N4NO <br />
Store Client <br />
Users Weather <br />



## Notes and Reference


If the necessary partition is read only try
```
  adb shell
  su
  mount -o remount,rw /system
```

Nokia 6300 4G - https://www.nokia.com/phones/en_us/nokia-6300-4g?sku=16LIOW11A01 <br />
BananaHackers debug mode - https://wiki.bananahackers.net/devices <br />
BananaHackers EDL tools - https://wiki.bananahackers.net/development/edl <br />
BananaHackers EDL downloads - https://edl.bananahackers.net/ <br />
Firefox Browser Toolbox - https://firefox-source-docs.mozilla.org/devtools-user/browser_toolbox/index.html <br />
Kaptein Sideload Guide - https://kaptein.me/blog/sideloading-and-deploying-apps-to-kai-os/ <br />
Keptein Webapp Conversion Guide - https://kaptein.me/blog/porting-converting-web-apps-website-to-kai-os/ <br />
App Buster - https://github.com/minhduc-bui1/AppBuster <br />
Luxferre's CrossTweak - https://gitlab.com/suborg/crosstweak <br />
If you can't sideload a particular app - https://www.reddit.com/r/KaiOS/comments/ugg97c/any_way_to_remove_bloatware_on_nokia_6300_4g/ <br />

https://developer.kaiostech.com/docs/getting-started/main-concepts/manifest/
https://developer.kaiostech.com/docs/getting-started/main-concepts/permissions/


Device <br />
    Developer <br />
        Debugger <br />
            ADB and DevTools <br /> 

Hostile programs
Kaiads
Whatsapp
Facebook
Google

Directory           Permissions
/system/etc         ?

