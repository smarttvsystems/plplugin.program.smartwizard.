This file is used to provide the wizard the necessary information to install external add-ons, and is typically named `addons.json`.

Example `addons.json`:
```JSON
{
  "addons": [
    {
      "name": "YouTube w/o Repository",
      "type": "addon",
      "section": false,
      "plugin": "plugin.video.youtube",
      "url": "http://mirrors.kodi.tv/addons/leia/plugin.video.youtube/plugin.video.youtube-6.5.2.zip",
      "repository": "",
      "repositoryxml": "",
      "repositoryurl": "",
      "icon": "",
      "adult": false,
      "description": "The official YouTube add-on."
    },
    {
      "name": "Spotify w/ Repository",
      "type": "addon",
      "section": false,
      "plugin": "plugin.audio.spotify",
      "url": "https://kodi-community-addons.github.io/repository.marcelveldt/plugin.audio.spotify/",
      "repository": "repository.marcelveldt",
      "repositoryxml": "https://raw.githubusercontent.com/kodi-community-addons/repository.marcelveldt/master/addons.xml",
      "repositoryurl": "https://kodi-community-addons.github.io/repository.marcelveldt/repository.marcelveldt/",
      "icon": "",
      "adult": false,
      "description": "The official Spotify add-on."
    },
    {
      "name": "Example Section",
      "section": true,
      "url": "url.to.json",
      "description": "An Example Section."
    }
  ]
}
```
For installing an add-on directly from a `.zip`, the `name` and `url` tags here are the only ones which are **required**. When installing from a repository, the `name`, `url`, `repository`, `repositoryurl`, and `repositoryxml` tags are **all required**. Any other tags can be left as `""`, `null`, or simply omitted. Not having mandatory tags will not create an error, but the incorrectly formatted entry will not be shown in the wizard.

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| type  | This can be either `"addon"`, `"skin"`, or `"addonpack"`. Currently, only `"addon"` is supported. |
| section | This can be either `true` or `false`. If `true`, this entry will open a new section in the wizard. |
| plugin | The plugin id of the add-on to install |
| url | A URL that points to the folder containing the zipped add-on. If installing directly, this should be a URL pointing to the add-on `.zip` file. If `"section": true`, then this should be a URL that points to a *different* `addons.json` file for the section. |
| repository | The plugin id of the repository to install from |
| repositoryxml | A URL that points to the `'addons.xml'` file for the repository |
| respositoryurl | A URL that points to the folder containing the zipped repository |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 512x512 pixel `.png` file. |
| adult | Whether this add-on is an adult add-on. Must be either `true` or `false`. |
| description | A short description of the add-on |

As of OpenWizard 1.2.0, this file has been converted from the "old" plaintext solution, to the "new" JSON format, which makes them far more flexible, but more syntactically oriented. To verify that your JSON files are formatted correctly, I recommend https://jsoneditoronline.org/.