*Trello Installation for Ubuntu 18.06*

Wget trello repo\
`$ wget https://github.com/danielchatfield/trello-desktop/releases/download/v0.1.9/Trello-linux-0.1.9.zip -O trello.zip`

Make Trello folder\
`$ sudo mkdir /opt/trello`

Unzip Trello in the folder\
`$ sudo unzip trello.zip -d /opt/trello/`

Create a symlink between the trello application a usr destination\
`$ sudo ln -sf /opt/trello/Trello /usr/bin/trello`

Create a desktop entry for trello. Then write the information to a trello.desktop file in the applications folder. -e enables backslash interpretations\
`$ echo -e '[Desktop Entry]\n Version=1.0\n Name=Trello\n Exec=/usr/bin/trello\n Icon=/opt/trello/resources/app/static/Icon.png\n Type=Application\n Categories=Application' | sudo tee /usr/share/applications/trello.desktop`

Set the x flag on the desktop entry. This enables execution\
`$ sudo chmod +x /usr/share/applications/trello.desktop`


*Errors*

Fixes for some common errors\
- trello: error while loading shared libraries: libgconf-2.so.4: cannot open shared object file: No such file or directory\
Install libgconf-2-4\
`$ sudo apt-get install libgconf-2-4`

- Failed to load module "canberra-gtk-module"\
Install module\
`$ sudo apt-get install libcanberra-gtk-module`