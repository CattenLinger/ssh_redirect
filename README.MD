A little script to make autossh works as a service.

To use:

0. Install `autossh` and `nc` first.
1. Copy files to `/opt/ssh_redirect` ,or somewhere you like, but remember to change the script path in service file.
2. Copy the example config, for example here "website.conf" and edit it.
3. Copy the ssh_redirect@.service to /lib/systemd/system and execute `systemctl daemon-refresh`.
4. Enable or start your daemon using `systemctl enable|start ssh_redirect@website`.

For details, see the `example.conf`.
