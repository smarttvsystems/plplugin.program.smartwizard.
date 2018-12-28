This file tells the wizard where to find the supplied [[Wizard Text Files]], among other customizations.

Editing other fields besides these listed *will likely break your wizard*.

# User Edit Variables

| Field | Description |
| ----- | ----------- |
| ADDONTITLE  | The name that will show in the wizard |
| BUILDERNAME | The name that will be attached to uploaded log files |
| EXCLUDES | A list of add-ons that will be ignored by normal wizard operations |
| CACHETEXT | Whether or not to "cache" the specified text files. Can be either `'Yes'` or `'No'`. |
| CACHEAGE | How long to cache text files, in days. |
| BUILDFILE | A URL that points to a `builds.txt` file. To ignore this field, set it to `'http://'`. |
| UPDATECHECK | How often to check for wizard updates, in days. Setting this to `0` will check on every startup. |
| APKFILE | A URL that points to an `apks.txt` file. To ignore this field, set it to `'http://'`. |
| YOUTUBETITLE | The title of the YouTube section in the wizard. |
| YOUTUBEFILE | A URL that points to a `youtube.txt` file. To ignore this field, set it to `'http://'`. |
| ADDONFILE | A URL that points to an `addons.txt` file. To ignore this field, set it to `'http://'`. |
| ADVANCEDFILE | A URL that points to an `advanced.txt` file. To ignore this field, set it to `'http://'`. |

# Theming Menu Items
For icons used in the wizard, you'll only need to make sure the filenames are correct. If you aren't using a particular icon, simply set the field to `'http://'`.

| Section | Filename |
| ------- | -------- |
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
| THEME5 | The theme used when writing the current theme. Make sure to include `%s`, so that the correct title will be used. |

You can also add a contact menu, to allow your users to get in contact with you more easily:

| Field | Description |
| ----- | ----------- |
| HIDECONTACT | Whether to hide the contact menu or not. Can be either `'Yes'` or `'No'`. |
| CONTACT | A simple contact message. This accepts `\n` for line breaks. |
| CONTACTICON | A URL to an icon to be shown in the contact menu. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default icon. |
| CONTACTFANART | A URL to the fanart to be shown in the contact menu. This must be a 512x512 pixel `.png` file. Use `"http://"` for the default fanart. |

# Auto Update For Those With No Repo

If you wish to have your wizard auto-update, and don't want to (or can't, for some reason) maintain a Kodi repository, you can configure your `uservar.py` accordingly, as well as updating your `builds.txt` file as mentioned on [[Installing Builds]].

| Field | Description |
| ----- | ----------- |
| AUTOUPDATE | Whether or not to activate this feature. Can be either `'Yes'` or `'No'`. |
| WIZARDFILE | A URL to a text file that contains the auto-updating information. This is typically found within ` builds.txt`, and can be left as the default. |

# Auto Install Repo If Not Installed

This feature can be used to automatically install your wizard's (or any other) Kodi repository, in the event that it isn't installed when the wizard is installed.

| Field | Description |
| ----- | ----------- |
| AUTOINSTALL | Whether or not to activate this feature. Can be either `'Yes'` or `'No'`. |
| REPOID | The plugin id of the desired repository |
| REPOADDONXML | A URL that points to the `addons.xml` associated with the desired repository |
| REPOZIPURL | A URL that points to the folder where the repository `.zip` is located |

# Notification Window

The notification window can be used to alert the user when there are build updates, or with any other alert defined in a `notify.txt`, as described on [[Update Notifications]].

| Field | Description |
| ----- | ----------- |
| ENABLE | Whether or not to activate this feature. Can be either `'Yes'` or `'No'`. |
| NOTIFICATION | A URL that points to a `notify.txt` file. To ignore this field, set it to `'http://'`. |
| HEADERTYPE | What type of header to use on the notification window. Can be either `'Text'` or `'Image'`. |
| FONTHEADER | Which font to use for the header, if HEADERTYPE=`'Text'`, as defined by the skin |
| HEADERMESSAGE | The message to use for the header, if HEADERTYPE=`'Text'` |
| HEADERIMAGE | A URL that points to an image to be used for the header, if HEADERTYPE=`'Image'`. Must be 424x180 pixels, or a similar ratio. |
| FONTSETTINGS | The font to be used for the text in the notification window, as defined by the skin |
| BACKGROUND | A URL that points to a fanart-style image to be shown as the background of the notification window. To ignore this field, set it to `'http://'`. |