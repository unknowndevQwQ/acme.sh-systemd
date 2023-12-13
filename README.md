# acme.sh-systemd
systemd units for renew certificates acquired via acme.sh  
The timer unit should be enabled.

**Note: User units are not tested**
## How to use

1. `mkdir -pm 0700 /{etc,var/log}/acme.sh`
2. `add LOG_FILE=/var/log/acme.sh/acme.sh.log`
3. `mv system/* -t /etc/systemd/system` or `mv user/* -t "${XDG_CONFIG_HOME:-$HOME/.config}/systemd/user"`
4. `#systemctl enable acme.sh.timer` or `systemctl --user enable acme.sh.timer`
5. `# acme.sh --home /etc/acme.sh command...` or `$ acme.sh command...`
