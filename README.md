# wok_gpxviewer
This is a [TYPO3](https://typo3.org) extension, which provides a plugin for integration of [GPXViewer](https://www.j-berkemeier.de/GPXViewer) from Jürgen Berkemeier.

## What does it do?
With including the [GPXViewer](https://www.j-berkemeier.de/GPXViewer) javascript one can display GPX tracks, routes, waypoints in Google Maps or Openstreetmap. Please refer to the [GPXViewer website](https://www.j-berkemeier.de/GPXViewer) for more informations about the features of [GPXViewer](https://www.j-berkemeier.de/GPXViewer).

This extension/plugin for [TYPO3](https://typo3.org) integrate most of the features of [GPXViewer](https://www.j-berkemeier.de/GPXViewer). For some examples please refer to [my website](https://wolfgangkleinbach.de/test/GPXViewer). I will also try to do some documentation for the use of the extension there.

## What prerequisites are needed?
* [TYPO3](https://typo3.org) 9.5.x or above.
* The [bootstrap_package](https://www.bootstrap-package.com/) is highly recommended. I only use the extension/plugin with the bootstrap_package and it's ScssPHP compiler and therefore the layout might be broken if you don't.
* For some features you need [exiftool](https://exiftool.org) installed on your server.
* Probably you need API keys for use of Google maps or OSM. Find more information about API keys [here](https://www.j-berkemeier.de/GPXViewer/#Apikey).
* You don't necessarily need GPX files, you even can create a GPXViewer content element and add your own waypoints or waypoint images with GPS coordinates. You need to know the coordinates from another source. This extension does not provide a way to determine GPS coordinates from a map.
* Commercial use of [GPXViewer](https://www.j-berkemeier.de/GPXViewer) of Jürgen Berkemeier is restricted. Read more about this and other restrictions [here](https://www.j-berkemeier.de/GPXViewer/#Rechtliches).
* The use of this TYPO3 extension is only restricted insofar as [GPXViewer](https://www.j-berkemeier.de/GPXViewer) and other provided resources are underlying restrictions.

## How to set up?
* Download and install the extension [wok_gpxviewer](https://github.com/zeichensatz/wok_gpxviewer).
* Create a new page in [TYPO3](https://typo3.org) backend or edit an existing one.
* Create an extension template for that page or edit an existing template and `"Include static (from extensions)"` for `GPXViewer (wok_gpxviewer)`.
* Change to `Constant Editor` and edit the settings for GPXViewer if needed.
* Now you can create a content element of type `plugin` and then select `GPXViewer tracks display`.
* In the tab `Plug-in` you are able to add GPX files for display in the frontend. There are several tabs with settings to explore. Hopefully most of them are self explaining. If not, don't hesitate to contact me (see below).

## How can you give your feedback
* I would like to hear from you, how you're using the extension and what can be improved.
  * You can write me a mail, see [my website](https://wolfgangkleinbach.de) for contact data.
  * You can add issues or pull requests on [github](https://github.com/zeichensatz/wok_gpxviewer).

## Todos
* Check button formatting for imgdivs: perhaps change to a tag? This would mean changes in the javascript too.
* Check CSS file option and update CSS file
* Map+imgdiv+profiles: Some minor problems in display
* make each map/imgdiv/profiles scaleable from backend
* more examples
* more documentation
* create TER version
* make extension compatible to extension_builder
