# VSCode settings

## Setup
1. Make sure your VSCode settings are updated to install this repository
![VSCode Dotfile Settings](screenshots/dotfile-settings.png)

2. Add the extensions you want installed to the `extensions` file
3. Symlink your VSCode settings to `settings.json` in this repo. Changes here will be reflected in the dev containers as well.
  On macos, that would be
  ```bash
  # Create a backup of your existing settings. This command will likely change your theme/etc.
  # You need to copy this file to settings.json in this repository
  mv /Users/{USERNAME}/Library/Application\ Support/Code/User/settings.json /Users/{USERNAME}/Library/Application\ Support/Code/User/settings.json.backup

  # Symlink the settings.json from this repository to the VSCode location. This will restore your theme/settings.
  # NOTE: You need to use full paths here. `~/` expansion is no good with synlinks
  ln -sf /Users/{USERNAME}/{PATH-TO-THIS-REPO}/settings.json /Users/{USERNAME}/Library/Application\ Support/Code/User/settings.json
  ```
4. Repeat step3 for `keybindings.json` and the `snippets/` directory
