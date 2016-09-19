#Datadog-systemd
------

This repo contains the code used to start the datadog-agent on our TAM S1 Pro printers.

Install Datadog-Agent:
```
sudo apt update
sudo apt install ntp curl sysstat
DD_API_KEY=INSERT_KEY_HERE sh -c "$(curl -L https://raw.githubusercontent.com/DataDog/dd-agent/master/packaging/datadog-agent/source/setup_agent.sh)"
```
Install and enable Datadog service
```
sudo curl -o /lib/systemd/system/datadog.service https://raw.githubusercontent.com/clemsonMakerspace/datadog-systemd/master/datadog.service
sudo systemctl enable datadog.service
sudo systemctl start datadog.service
```
