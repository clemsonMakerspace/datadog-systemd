#Datadog-systemd
------

This repo contains the code used to start the datadog-agent on our TAM S1 Pro printers.

Installation:

```
sudo curl -o /lib/systemd/system/datadog.service https://raw.githubusercontent.com/clemsonMakerspace/datadog-systemd/master/datadog.service
sudo systemctl enable datadog.service
sudo systemctl start datadog.service
```
