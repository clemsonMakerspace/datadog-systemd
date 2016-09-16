#Datadog-systemd
------

This repo contains the code used to start the datadog-agent on our TAM S1 Pro printers.

Installation:

1. Copy datadog-service into /lib/systemd/system/datadog-service
2. Enable the new service

  ```
  sudo systemctl enable datadog.service
  sudo systemctl start datadog.service
  ```
  
3. Restart to test
