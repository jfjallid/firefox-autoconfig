# Firefox-Autoconfig

## Description
This repo contains a collection of settings for Firefox which aims to improve
the signal-to-noise ratio for web traffic inspected through a proxy.

Firefox makes quite a lot of web requests in the background which can be
annoying when doing a security assessment as it tends to bury the interesting
stuff with traffic for telemetry, extension updates, network captivity portals,
etc.

There are also a number of settings included such as to not create popups and
ask if a page should be translated, and to not send things accidentally typed
in the address bar to a search engine.

## Contributions
Tips or pull requests with additional settings to apply which could improve
Firefox for a security assessment are welcome!

## Usage
Copy the two files autoconfig.js and autoconfig.cfg to the Firefox installation
directory:

```
<firfox install dir>/defaults/pref/autoconfig.js
<firfox install dir>/autoconfig.cfg
```

Restarting Firefox should apply the new settings to the existing profiles.
If not, try to create a new profile.
