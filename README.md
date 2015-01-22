# Play Game Services Magic Configuration
A tool that uses the [Play Game Services Publishing API](https://developers.google.com/games/services/publishing/) to automatically configure achievements and leaderboards for pre-configured samples.

# Description
The config-magic tool is a web interface for the [Play Game Services Publishing API](https://developers.google.com/games/services/publishing/). Using this tool, you can automatically create Leaderboards and Achievements for your Play Game Services projects. This makes it easier to get started with sample applications that may require you to create many achievements and leaderboards.

# Architecture

  * `index.html` and `index.js` - the main page and logic for the applicatio. Contains all of the UI and associated logic.
  * `config-form.html` and `config-form.js` - define the `<config-form>` Polymer element. Contains all of the logic for interacting with the Publishing API to create Leaderboards, Achievements, etc.
  * `info.js` - defines the `configs` variable which tells the application what Leaderboards and Achievements are required to configure a given sample. This is referenced in `index.html` in the `infofile` attribute of the `config-form` element.  When navigating to `index.html` the `sample?=...` query parameter is read from the URL and used to determine which sample the user would like to configure.

# Usage
The config-magic tool is currently deployed alonside the [android-basic-samples](https://github.com/playgameservices/android-basic-samples) repository in order to automatically configure leaderboards and samples. The tool is modeled as a static website that can be hosted on Github Pages or any other static hosting provider.

# More Information
For an example of how to use the Publshing API, visit the [management-tools sample](https://github.com/playgameservices/management-tools).
