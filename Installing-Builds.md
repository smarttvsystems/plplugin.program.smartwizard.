This file is used to supply your wizard with builds to install, as well as being responsible for auto-updating your wizard if there is no repository, and is typically named `builds.txt`.

Example `builds.txt`:
```
id="plugin.program.aftermath"
version="0.4.5"
zip="url.to.wizard"

name="Example Build 1"
version="1.0"
url="url.to.build"
minor=""
gui="url.to.guisettings"
kodi="17.6"
theme="url.to.themes"
icon="http://"
fanart="http://"
preview="https://www.youtube.com/watch?v=djV11Xbc914"
adult="no"
info="url.to.info"
description="A short description of the build."

name="Example Build 2"
version="1.0"
url="url.to.build"
minor=""
gui="url.to.guisettings"
kodi="18.0"
theme="url.to.themes"
icon="http://"
fanart="http://"
preview="https://www.youtube.com/watch?v=L_jWHffIx5E"
adult="no"
info="url.to.info"
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
| minor | The minor version number for incremental updates (THIS IS CURRENTLY NON-FUNCTIONAL) |
| gui | A URL that points to a `quisettings.xml` file for the build |
| kodi | The Kodi version number that the build is compatible with |
| theme | A URL that points to a `themes.txt` file for this build |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |
| preview  | A URL that points to a YouTube video to use as a build preview |
| adult | Whether this build contains adult content. Must be either `"yes"` or `"no"`. |
| info | A URL that points to an info text file about the build. This file is generated *by* the wizard when creating a build. |
| description | A short description of the build |