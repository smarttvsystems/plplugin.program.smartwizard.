This file is used to provide the wizard the necessary information to install external `.apk` files, and is typically named `apks.txt`. The wizard already comes with built in scrapers for the latest Kodi (stable *and* unstable) builds. The APK Installer menu is only shown if running on an Android device or when in developer mode.

Example `apks.txt`:
```
name="Example APK"
section="no"
url="url.to.apk"
icon="http://"
fanart="http://"
adult="no"
description="A short description of the APK."

name="Example Section"
section="yes"
url="url.to.textfile"
icon="http://"
fanart="http://"
adult="no"
description="An example section."
```

The fields in this file are all required.

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| section | Whether this should open a separate section. Must be `"yes"` or `"no"`. |
| url | A url that points to an `.apk` file. If section=`"yes"`, then this should be a url to another `apk.txt` file. |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |
| adult | Whether this '.apk' had adult content. Must be `"yes"` or `"no"` |
| description | A short description of the `.apk` |