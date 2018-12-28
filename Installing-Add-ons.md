This file is used to provide the wizard the necessary information to install external add-ons, and is typically named `addons.txt`.

Example `addons.xml`:
https://github.com/drinfernoo/plugin.program.aftermath/blob/9a752a35cdbb28083b903b24207cc100efeacbb2/resources/text/addons.txt#L1-L21

The fields in this file are all required.

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| plugin | The plugin id of the add-on to install. Use `"section"` to have this item open a new section. |
| url | A URL that points to the folder containing the zipped add-on. If installing directly, this should be a URL pointing to the add-on `.zip` file. If plugin=`'section'`, then this should be a URL that points to a *different* `addons.txt` file for the section. |
| repository | The plugin id of the repository to install from. If installing directly, this should be set to `"none"`. |
| repositoryxml | A URL that points to the `'addons.xml'` file for the repository. If installing directly, this should be set to `"http://"`. |
| respositoryurl | A URL that points to the folder containing the zipped repository. If installing directly, this should be set to `"http://"`. |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |
| adult | Whether this add-on is an adult add-on. Must be either `"yes"` or `"no"`. |
| description | A short description of the add-on |