# acme.sh-systemd
systemd service for automatic Let's Encrypt(for acme.sh) renewals
The timer unit should be enabled.

How to use

mkdir -pm 0700 "/{etc,var/log}/acme.sh"

add LOG_FILE='/var/log/acme.sh/acme.sh.log'

acme.sh --home /etc/acme.sh command ...[parameters]....
