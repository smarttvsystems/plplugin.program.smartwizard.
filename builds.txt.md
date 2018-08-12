This file is used to supply your wizard with builds to install, as well as being responsible for auto-updating your wizard if there is no repository.

If there is no repository, and auto-updating is desired, the beginning of the file must contain the following three fields:

| Field | Description |
| ----- | ----------- |
| id | The plugin id for the wizard |
| version | The newest version to update to |
| zip | A url that points to the wizard '.zip' file |

For adding builds, simply add the following section for each build:

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| version | The version of the build |
| url | A url that points to the build '.zip' |
| minor | The minor version number for incrmental updates (THIS IS CURRENTLY NON-FUNCTIONAL) |
| gui | A url that points to a 'quisettings.xml' file for the build |
| kodi | The Kodi version number that the build is compatible with |
| icon | The icon to be shown in Kodi. This must be a 512x512 pixel '.png' file. Use "http://" for the default icon. |
| fanart | The fanart to be shown in Kodi. This must be a 512x512 pixel '.png' file. Use "http://" for the default fanart. |
| preview  | A url that points to a YouTube video to use as a build preview |
| adult | Whether this add-on is an adult add-on. Must be either 'yes' or 'no'.
| info | Info about the build |
| description | A short description of the add-on |