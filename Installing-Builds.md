This file is used to supply your wizard with builds to install, as well as being responsible for auto-updating your wizard if there is no repository, and is typically named `builds.txt`.

## The fields in this file are all required, and removing any of them will **break** your wizard.

Example `builds.txt`:
```
id="plugin.program.openwizard"
version="1.0.0"
zip="url.to.wizard"

name="Example Build 1"
version="1.0"
url="http://your.build.url/"
minor="http://"
gui="http://your.guisettings.url/"
kodi="17.6"
theme="http://your.themes.url"
icon="http://"
fanart="http://"
preview="https://www.youtube.com/watch?v=djV11Xbc914"
adult="no"
info="http://your.info.url"
description="A short description of the build."

name="Example Build 2"
version="1.0"
url="http://your.build.url/"
minor="http://"
gui="http://your.guisettings.url/"
kodi="18.6"
theme="http://your.themes.url"
icon="http://"
fanart="http://"
preview="https://www.youtube.com/watch?v=L_jWHffIx5E"
adult="no"
info="http://your.info.url"
description="A short description of the build."
```

If there is no repository, and auto-updating is desired, the beginning of the file must contain the following three fields:

| Field | Description |
| ----- | ----------- |
| id | The plugin id for the wizard |
| version | The newest version to update to |
| zip | A url that points to the wizard `.zip` file |

For adding builds, simply add the following section for each build:

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| version | The version of the build |
| url | A URL that points to the build `.zip` |
| minor | A URL that points to a minor update `.zip`, not requiring a fresh install. This feature is currently **disabled** in the wizard. |
| gui | A URL that points to a `quisettings.xml` file for the build |
| kodi | The Kodi version number that the build is compatible with |
| theme | A URL that points to a `themes.txt` file for this build |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |
| preview  | A URL that points to a YouTube video to use as a build preview |
| adult | Whether this build contains adult content. Must be either `"yes"` or `"no"`. |
| info | A URL that points to a detailed info text file about the build. This file is generated *by* the wizard when creating a build. If this tag is left as `"http://"`, the wizard will still be able to show a condensed version of information about the build. |
| description | A short description of the build |