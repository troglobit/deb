troglobit-archive-keyring
=========================

This GIT repo contains the key(s) used to sign Debian/Ubuntu packages
for http://deb.troglobit.com

* `/etc/apt/trusted.gpg.d/`: contains Each actively used key to be used
  by `apt` and `apt-key`.  The signatures of acquired Release files are
  checked against this key database.  It hence contains all keys of all
  releases that are still supported and need to be active.
* `/usr/share/keyrings/troglobit-archive-keyring.gpg`: the keyring of
  all keys actively used to sign Release files

You can list the keys within the keyring by issuing:

    $ gpg /usr/share/keyrings/troglobit-archive-keyring.gpg

More information about the archive authentication feature can be found
in the manpage apt-secure(8).

For information on the involved GPG commands and operations, please see:
https://www.gnupg.org/gph/de/manual/r1023.html

