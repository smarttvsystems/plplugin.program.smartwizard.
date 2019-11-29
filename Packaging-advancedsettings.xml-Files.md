This file is used to provide the wizard the necessary information to install preconfigured `advancedsettings.xml` files, and is typically named `advanced.json`. Some very basic presets are included with the wizard via this file.

Example `advanced.json`:
```JSON
{
    "presets": [
        {
            "name": "Enable All Artwork",
            "section": false,
            "url": "https://raw.githubusercontent.com/drinfernoo/repository.openwizard/master/presets/artwork_preset.xml",
            "icon": "",
            "fanart": "",
            "description": "This preset adds all of the available arttypes, to be used with library scrapers which collect their own artwork. Only has any effect on Kodi 18+."
        },
        {
            "name": "Cache & Network Presets",
            "section": true,
            "url": "https://raw.githubusercontent.com/drinfernoo/repository.openwizard/master/presets/cache_presets.json",
            "icon": "",
            "fanart": "",
            "description": "All presets related to caching, network, and buffering."
        }
    ]
}
```
The `name` and `url` tags here are the only ones which are **required**. Any other tags can be left as `""`, `null`, or simply omitted. Not having mandatory tags will not create an error, but the incorrectly formatted preset will not be shown in the wizard.

| Field | Description |
| ----- | ----------- |
| name  | The name that will show in the wizard |
| section | This can be either `true` or `false`. If `true`, this entry will open a new section in the wizard. |
| url | A URL that points to an `advancedsettings.xml` file. If `"section": true`, then this URL should point to a *different* `advanced.json` file. |
| icon | A URL to an icon to be shown in Kodi. This must be a 512x512 pixel `.png` file. If omitted, the wizard will use `maintenance.png`. |
| fanart | A URL to the fanart to be shown in Kodi. This must be a 1920x1080 pixel file of any format. If omitted, the wizard will use `fanart.png`. |
| description | A short description of the file |

As of OpenWizard 1.1.0, this file has been converted from the "old" plaintext solution, to the "new" JSON format, which makes them far more flexible, but more syntactically oriented. To verify that your JSON files are formatted correctly, I recommend https://jsoneditoronline.org/.