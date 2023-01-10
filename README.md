# Logiops config

## Setup
[Install logiops from source](https://github.com/PixlOne/logiops#building)

## Usage

This config is not picked up by default. The default config sits at `/etc/logid.cfg`.
In order for this config to take effect, change the `ExecStart` option in `/usr/lib/systemd/logid.service` to point to this config file:

`ExecStart=/usr/bin/logid --config /home/olivier/.config/logid/logid.cfg`

Then restart the service:
`sudo systemctl daemon-reload && sudo systemctl restart logid.service`
