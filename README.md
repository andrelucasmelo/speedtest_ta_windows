# Speedtest Addon for Splunk Universal Forwarder
Windows version.

This is a Addon for Splunk Universal Forwarder, on Windows instances to obtain result tests from bandwidth quality in your workstations.

Dependencies:
- Splunk Universal Forwarder version 7.0.0 or higher.
- Splunk Enterprise 7 or higher or Splunk Cloud.
- Microsoft Windows x86_64 version.

Default Configuration:
- This addon will run speedtest every hour at minute zero.
- All logs will be sended to index speedtest.
- We will use a global outputs configurations present on Universal Forwarder.

Customize addon configuration:
- You can use a local/inputs.conf file to customize configurations.
- In local/inputs.conf, you can change INTERVAL, SOURCE, HOST, INDEX and SOURCETYPE configs.
- You must use crontab format to configure INTERVAL.
- We recommend that you dont change SOURCE, SOURCETYPE and HOST configurations.
- You can change INDEX configurato to forwarding logs to a specific index.

