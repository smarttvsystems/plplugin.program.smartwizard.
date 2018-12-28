This file is used to provide the wizard the necessary information to install preconfigured 'advancedsettings.xml' files, and is typically named `advanced.txt`.

Example `advanced.txt`:
```
name="Example advancedsettings.xml"
section="no"
url="url.to.advancedsettings"
icon="http://"
fanart="http://"
description="An example advancedsettings.xml."

name="Example section"
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
| url | A URL that points to an `advancedsettings.xml` file |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |
| description | A short description of the file |