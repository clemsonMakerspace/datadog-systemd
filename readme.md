#Datadog-systemd
------

This repo contains the code used to start the datadog-agent on our TAM S1 Pro printers.

Installation:

1. Copy datadog-service into /lib/systemd/system/datadog-service
2. Enable the new service

  ```
  sudo systemctl enable mouselogger.service
  sudo systemctl start mouselogger.service
  ```
  
3. Restart to test
