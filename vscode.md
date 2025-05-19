## Important Key bindings
- `Ctrl` + `Shift` + `P` - command panel on top
- `Ctrl` + `` ` `` - toggle terminal and editor
- `Ctrl` + `Alt` + `M` - Maximize bottom panel
- `Ctrl + K` `Ctrl + S` -  for modifying keybindings
- `Ctrl + B` - Hide side panel -
- `Ctrl` + `K`

## Installation of automatic updates
```
sudo apt install apt-transport-https
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo install -o root -g root -m 644 microsoft.gpg /usr/share/keyrings/
sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/microsoft.gpg] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
rm microsoft.gpg
sudo apt update
sudo apt install code
```
