# Better Grbl Support Plugin for Octoprint

![grbl](https://raw.githubusercontent.com/gnea/gnea-Media/master/Grbl%20Logo/Grbl%20Logo%20250px.png)

This plugin was largely developed based on Synmans Version of the same name.

This version allows streaming of any wireless IP camera(provided it is on your network) instead of the default in-built streamer. A new setting now appears in the settings panel that allows any IP Camera to be displayed.  

## Setup

Install manually using this URL:

    https://github.com/slmmnl/OctoPrint-Bettergrblsupport/archive/master.zip

## Configuration

There are some meaningful caveats regarding the installation and configuration of this plugin.  If you use it in a multi-printer / profile environment it will very likely cause problems for your other profiles as it makes **GLOBAL** configuration changes behind the scenes.  A future version may resolve this, but understand that currently multi-profile installations are not currently supported.

Furthermore, a number of global configuration changes are made blindly and I have no way of reverting these changes.  Be prepared to manually edit your config.yaml and/or manually revert global settings if you uninstall / disable this plugin to restore your Octoprint installation to its prior state.

Pay special attention to the following config.yaml configuration parameters:

* appearance / components / temperature tab
* controls (any / all customizations made to it)
* feature / temperatureGraph
* feature / gcodeVisualizer
* feature / modelSizeDetection
* serial / neverSendChecksum
* serial / checksumRequiringCommands
* serial / helloCommand
* plugins / _disabled / printer_safety_check
* appearance / components / disabled / tab

## Screenshots

![Main UI](https://plugins.octoprint.org/assets/img/plugins/bettergrblsupport/better_grbl_support_main.png)

![Configuration UI](https://plugins.octoprint.org/assets/img/plugins/bettergrblsupport/better_grbl_support_settings.png)
