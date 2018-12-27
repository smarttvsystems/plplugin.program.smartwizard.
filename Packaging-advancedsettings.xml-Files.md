This file is used to provide the wizard the necessary information to install preconfigured 'advancedsettings.xml' files, and is typically named `advanced.txt`.

The fields in this file are all required.

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| section | Whether this should open a separate section. Must be `"yes"` or `"no"`. |
| url | A url that points to an `advancedsettings.xml` file |
| icon | The icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | The fanart to be shown in Kodi. This must be a 1920x1080 pixel (or similar ratio) `.jpg` file. Use `"http://"` for the default fanart. |
| description | A short description of the file |