# password-database

> TL;DR: privately hosted KeeWeb with KeePass database hosted over WebDav

This Ansible role is in charge of configuring necessary services for running a [KeeWeb](https://keeweb.info/) instance with WebDav.
The steps included are the following:
- Unpack the newest version of KeeWeb from the project's GitHub archive into the document root for KeeWeb
- Move over the KeeWeb configuration file and assign this as the configuration in the KeeWeb's `index.html`
- Setup an Apache2 virtual host through a provided template
- Restart the Apache2 SystemD service

### Note

The actual KeePass database file should exist under:

```
<DocumentRoot>/webdav/PWDB.kdbx
```

Moving over the database is not automated to ensure that it is not accidentally overwritten.
The database should be touched as little as possible, and only altered through an interface.
Please move the database file there manually (you can alter the name of the database file as long as you update the role).
