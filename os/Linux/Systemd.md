# Systemd

Process manager for Linux

config example:

```ini
[Unit]
Description=MyApp Service
After=network.target

[Service]
ExecStart=/usr/bin/python /path/to/app.py
Restart=always
User=myuser

[Install]
WantedBy=multi-user.target
```

log search:

`journalctl -u myapp.service`
