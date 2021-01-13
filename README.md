# Speedtest Addon for Splunk Universal Forwarder(For Windows)

This is a Addon for Splunk Universal Forwarder, on Windows instances to obtain result tests from bandwidth quality in your workstations.

Dependencies:
- Splunk Universal Forwarder version 7.0.0 or higher.
- Splunk Enterprise 7 or higher or Splunk Cloud.
- Microsoft Windows x86_64 version.

Default Configuration:
- This addon will run speedtest every hour on minute zero.
- This addon will send results to index speedtest on indexers.
- This addon will use a global configuration of log forwarding present on outputs.conf file.

Customize addon configuration:
- You can use a local/inputs.conf file to customize configurations.
- In local/inputs.conf, you can change INTERVAL, SOURCE, HOST, INDEX and SOURCETYPE configs.
- You must use crontab format to configure INTERVAL.
- We recommend that you dont change SOURCE, SOURCETYPE and HOST configuration.
- You can change INDEX configurato to forwarding logs to a specific index.

