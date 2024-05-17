# ST-my-package-control

- `repository-released.json` is for released plugins, which can be found on [Package Control][package-control].
- `repository.json` is more like for plugins just for myself. Not released on [Package Control][package-control].

## Usage

For plugins in `repository-released.json`, you can simply find them on [Package Control][package-control].

If you want to use those plugins which is in `repository.json`,

1. Make sure you are using Package Control v4 or later.
   You can simply execute the following command in ST console to upgrade to the latest Package Control.

   ```py
   from urllib.request import urlretrieve;urlretrieve(url="https://github.com/wbond/package_control/releases/latest/download/Package.Control.sublime-package", filename=sublime.installed_packages_path() + '/Package Control.sublime-package')
   ```

1. Execute `Package Control: Add Repository` in the command palette.
1. Add this custom repository URL:
   https://raw.githubusercontent.com/jfcherng-sublime/ST-my-package-control/master/repository.json
1. Restart Sublime Text.
1. You should be able to install packages with Package Control now.

[package-control]: https://packagecontrol.io
