This file is used to provide the wizard the necessary information to install external add-ons, and is typically named `addons.txt`.

Example `addons.xml`:
```
name="YouTube w/o Repository"
plugin="plugin.video.youtube"
url="http://mirrors.kodi.tv/addons/leia/plugin.video.youtube/plugin.video.youtube-6.2.3.zip"
repository="none"
repositoryxml="http://"
repositoryurl="http://"
icon="http://"
fanart="http://"
adult="no"
description="The official YouTube add-on."

name="Spotify w/ Repository"
plugin="plugin.audio.spotify"
url="https://marcelveldt.github.io/repository.marcelveldt/plugin.audio.spotify/"
repository="repository.marcelveldt"
repositoryxml="https://raw.githubusercontent.com/marcelveldt/repository.marcelveldt/master/addons.xml"
repositoryurl="https://marcelveldt.github.io/repository.marcelveldt/repository.marcelveldt/"
icon="http://"
fanart="http://"
adult="no"
description="The official Spotify add-on."

name="Example Section"
plugin="section"
url="url.to.textfile"
repository="none"
repositoryxml="http://"
repositoryurl="http://"
icon="http://"
fanart="http://"
adult="no"
description="An example section."
```

The fields in this file are all required.

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| plugin | The plugin id of the add-on to install. Use `"section"` to have this item open a new section. |
| url | A url that points to the folder containing the zipped add-on. If installing directly, this should be a url pointing to the add-on `.zip` file. If plugin=`'section'`, then this should be a url that points to a *different* `addons.txt` file for the section. |
| repository | The plugin id of the repository to install from. If installing directly, this should be set to `"none"`. |
| repositoryxml | A url that points to the `'addons.xml'` file for the repository. If installing directly, this should be set to `"http://"`. |
| respositoryurl | A url that points to the folder containing the zipped repository. If installing directly, this should be set to `"http://"`. |
| icon | The icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| fanart | The fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |
| adult | Whether this add-on is an adult add-on. Must be either `"yes"` or `"no"`. |
| description | A short description of the add-on |