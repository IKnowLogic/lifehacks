*Redshift installation for Ubuntu 18.06*

Apt get Redshift\
`$ Sudo apt-get install redshift-gtk`


*Errors*

Fixes for some common errors\
- GDBus.Error:org.freedesktop.DBus.Error.AccessDenied: Access denied\
Add the following lines to /etc/geoclue/geoclue.conf \

[redshift]\
allowed=true\
system=false\
users=\

This can be done with the `tee -a` command:\
`$ echo -e '\n[redshift]\nallowed=true\nsystem=false\nusers=' | sudo tee -a /etc/geoclue/geoclue.conf`