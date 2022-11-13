# custom-fox
This is my customized firefox build, using `local-settings.js` and `my_firefox.cfg` to set and lock preferences in Firefox. This is __not__ a complete build, as it is missing a number of extensions and other preferences/settings. This is just my own configuration, which I use on my own VMs and setups.

### Overview
Firefox preferences can be configured by using two configuration files: the `local-settings.js` and a configuration (*.cfg). The location of these files can vary depending the OS. More info can be found in the `my_firefox.cfg` file.

You can find online an endless library of configurations and methods for Firefox. Most of them will use the `user.js` file to make the changes per user profile. Since the `user.js` is soon-to-be deprecated, I adapted [arkenfox's `user.js`][1] to the AutoConf format, which allows me to configure Firefox on multiple VMs and different OSs. The original file was extremely detailed, so I didn't need to make many changes. It also streamlined my configuration to fit my wants/needs.


### Notes
1. Do not modify the contents of the `local-settings.js`, except if you wish to change the name from `my_firefox.cfg` to something else.
2. All the preferences are explained in detail in the `my_firefox.cfg` file. All credit goes to [arkenfox][2]
3. In Ubuntu and other Debian-based systems (i.e. Kali) the firefox default installation directory (not esr) is under `/usr/lib/firefox/`. You should put the `local-settings.js` file under `.../firefox/defaults/pref/` and the `myfox.cfg` in the root dir (`/usr/lib/firefox/`).


### Acknowledgements
The available resources on how to configure firefox are endless. For more information on the configuration parameters, you can follow the links provided by arkenfox and also what's inside the template.


[1]: <https://github.com/arkenfox/user.js/blob/master/user.js> "arkenfox user.js file"
[2]: <https://github.com/arkenfox> "arkenfox's github page"
