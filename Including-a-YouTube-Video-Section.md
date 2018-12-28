This file is used to provide the wizard the necessary information to show a menu of YouTube videos, and is typically named `youtube.txt`.

Example `youtube.txt`:
```
name="Example Video"
section="no"
url="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
icon="http://"
fanart="http://"
description="An example video."

name="Example Section"
section="yes"
url="url.to.textfile"
icon="http://"
fanart="http://"
description="An example section."
```

The fields in this file are all required.

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| section | Whether this should open a separate section. Must be `"yes"` or `"no"`. |
| url | A URL that points to an YouTube video. If section=`"yes"`, then this should be a url that points to another `youtube.txt` file. |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |
| description | A short description of the video |