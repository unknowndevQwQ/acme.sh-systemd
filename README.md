# acme.sh-systemd
systemd units for renew certificates acquired via acme.sh  
The timer unit should be enabled.

## How to use

1. `mkdir -pm 0700 /{etc,var/log}/acme.sh`

2. `add LOG_FILE=/var/log/acme.sh/acme.sh.log`

3. `# acme.sh --home /etc/acme.sh command ...[parameters]....`
