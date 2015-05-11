This project is enhanced version of Code Comment plugin for Gedit. In addition to the normal methods of commenting/decommenting the code with either Edit-menu options or keyboard shortcuts, this version puts the commenting options in the right-click menu. There is also an option to enable commenting empty lines.

Note that this version uses Gconf for storing the preferences. Gconf is not part of Gnome 3. This version is primarily meant for Gnome 2.

Installation:

[gedit-codecomment.schemas](http://code.google.com/p/ld-gedit-code-comment-plugin/downloads/detail?name=gedit-codecomment.schemas)

[codecomment.py](http://code.google.com/p/ld-gedit-code-comment-plugin/downloads/detail?name=codecomment.py)

[codecommentconfig.py](http://code.google.com/p/ld-gedit-code-comment-plugin/downloads/detail?name=codecommentconfig.py)

Just download and copy above files to ~/.gnome2/gedit/plugins

If this is your first manually installed plugin, you probably don't have the "plugins" folder. Just create it. After that, just run Gedit and go enable the plugin from Preferences.

And if you want, there is also the Gconf .schema file in the downloads section. It can be installed with:

```
gconftool --install-schema-file=gedit-codecomment.schemas```

But it's not required. And if you don't know what it is, you don't need it.

Note: if you have gedit-plugins package installed (including the original Code Comment plugin), you can still use this plugin without uninstalling the gedit-plugins package. Gedit seems to prefer plugins in the users home directory, so this version will simply replace the old one. And if you want to go back to the original, just delete this version.