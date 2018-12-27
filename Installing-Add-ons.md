##addons.txt

This file is used to provide the wizard the necessary information to install external add-ons.

The fields in this file are all required.

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| plugin | The plugin id of the add-on to install. Use 'section' to have this item open a new section. |
| url | A url that points to the folder containing the zipped add-on. If plugin='section', then this should be a url that points to a *different* addons.txt file for the section. |
| repository | The plugin id of the repository to install from |
| repositoryxml | A url that points to the 'addons.xml' file for the repository |
| respositoryurl | A url that points to the folder containing the zipped repository |
| icon | The icon to be shown in Kodi. This must be a 512x512 pixel '.png' file. Use "http://" for the default icon. |
| fanart | The fanart to be shown in Kodi. This must be a 512x512 pixel '.png' file. Use "http://" for the default fanart. | adult | Whether this add-on is an adult add-on. Must be either 'yes' or 'no'.
| description | A short description of the add-on |