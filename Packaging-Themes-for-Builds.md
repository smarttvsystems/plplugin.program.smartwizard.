This file is used to provide available themes to a build, and is typically named `themes.txt`.

## The fields in this file are all required, and removing any of them will **break** your wizard.

Example `themes.txt`:
```
name="Example Theme"
url="http://your.theme.url/"
icon="http://"
fanart="http://"
adult="no"
description="A short description of the theme."
```

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| url | A URL that points to a theme `.zip` file. |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |
| adult | Whether this theme contains adult content. Must be either `"yes"` or `"no"`. |
| description | A short description of the theme |