This file tells the wizard where to find the supplied [[Wizard Text Files]], among other customizations.

Editing other fields besides these listed *will likely break your wizard*.

| Field | Description |
| ----- | ----------- |
| ADDONTITLE  | The name that will show in the wizard |
| BUILDERNAME | The name that will be attached to uploaded log files |
| EXCLUDES | A list of add-ons that will be ignored by normal wizard operations |
| CACHETEXT | Whether or not to "cache" the specified text files. Can be either `'Yes'` or `'No'`. |
| CACHEAGE | How long to cache text files, in days. |
| BUILDFILE | A url that points to a `builds.txt` file. |
| UPDATECHECK | How often to check for wizard updates, in days. Setting this to `0` will check on every startup. |
| APKFILE | A url that points to an `apks.txt` file. |
| YOUTUBETITLE | The title of the YouTube section in the wizard. |
| YOUTUBEFILE | A url that points to a `youtube.txt` file. |
| ADDONFILE | A url that points to an `addons.txt` file. |
| ADVANCEDFILE | A url that points to an `advanced.txt` file. |

For icons used in the wizard, you'll only need to make sure the filenames are correct. If you aren;t using a particular icon, simply set the filed to `'http://'`.

| Section | Filename |
| ----- | ----------- |
| Builds | `builds.png` |
| Maintenance | `maintenance.png` |
| Speed Test | `speed.png` |
| APK Installer | `apkinstaller.png` |
| YouTube | `youtube.png` |
| Save Data | `savedata.png` |
| Keep Trakt | `keeptrakt.png` |
| Keep Debrid | `keepdebrid.png` |
| Keep Login Data | `keeplogin.png` |
| Contact | `information.png` |
| Settings | `settings.png` |

In terms of theming your wizard, a number of options are provided:

| Field | Description |
| ----- | ----------- |
| HIDESPACERS | Whether to hide spacers in the wizard. Can be either `'Yes'` or `'No'`. |
| SPACER | The character to use as a spacer. Must be surrounded by `''`. |
| COLOR1 | The primary accent color for your wizard. The default is `'dodgerblue'`. |
| COLOR2 | The secondary accent color for your wizard. The default is `white`. |
| THEME1 | The theme used when writing primary menu items. Make sure to include `%s`, so that the correct title will be used. |
| THEME2 | The theme used when writing build names. Make sure to include `%s`, so that the correct title will be used. |
| THEME3 | The theme used when writing alternate menu items. Make sure to include `%s`, so that the correct title will be used. |
| THEME4 | The theme used when writing the current build. Make sure to include `%s`, so that the correct title will be used. |
| THEME5 | The theme used when writing the curent theme. Make sure to include `%s`, so that the correct title will be used. |