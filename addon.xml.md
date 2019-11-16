The `addon.xml` file is [used by Kodi to get information about an add-on](https://kodi.wiki/view/Addon.xml), in this case, your wizard. There are a number of fields that can be changed inside, but only a couple are really necessary to make your wizard unique.

Example `addon.xml`:
```xml
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<addon id="plugin.program.openwizard" name="[COLOR limegreen][B]Open[/B][/COLOR]Wizard" version="1.0.0" provider-name="drinfernoo">
  <requires>
    <import addon="xbmc.python" version="2.1.0"/>
  </requires>
  <extension point="xbmc.python.pluginsource" library="default.py">
    <provides>executable</provides>
  </extension>
  <extension point="xbmc.service" library="startup.py" start="startup" />
  <extension point="xbmc.addon.metadata">
    <summary lang="en">[COLOR limegreen][B]Open[/B][/COLOR]Wizard</summary>
    <description lang="en">[COLOR limegreen][B]Open[/B][/COLOR]Wizard offers many maintenance features, selective add-on data saving, and automated build installs.</description>
    <platform>all</platform>
  </extension>
</addon>
```

Editing other fields besides these listed will *likely break your wizard*.

| Tag | Parameter | Description |
| --- | ------ | ----------- |
| `addon` | `id` | Your wizard's plugin id to be used by Kodi |
| | `name` | The name that will be displayed inside of Kodi |
| | `version` | Your wizard's version number |
| | `provider-name` | The name of the developer of your wizard |
| `summary` | | A simple summary of your wizard's functions |
| `description` | | A short description of your wizard |