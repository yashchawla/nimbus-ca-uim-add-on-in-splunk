#The custom add-on created for Splunk provides custom alert trigger functionality and is designed to send alerts to CA UIM using the 'nimalarm' utility. This add-on can be configured to monitor any type of data source within a Splunk environment, and when a specific event or condition occurs, it triggers an alert using 'nimalarm' to send it to the CA UIM system. The 'nimalarm' utility ensures that the alert is delivered in a timely and efficient manner, and can be customized to meet the specific needs of each user. With this add-on, users can proactively manage their data, detect and respond to issues quickly, and ensure that critical events are immediately communicated to the CA UIM system for further action. This can help users to improve their overall Splunk experience, and ensure that they are able to effectively manage their IT infrastructure.

Install this add-on as per the Splunk documented guidelines.

Usage:
1. Create a search and save it as an alert.
2. Select trigger condition: "Nimbus alert in Splunk"
3. Fill-in the required details and save it.

Note:
1. Should have Nimbus agent installed in your system.
2. Ensure 'nimalert' is stored under /opt/nimbus/bin/nimalarm, if not, you can change the path in TA-nimbusalerting/bin/nimbus.sh.
3. Supports only Linux x86-64.

Troubleshooting:
To check whether your alerts are getting triggered or not, verify under:

1. /tmp/nimbus_alerts_log.txt
2. <SPLUNK_HOME>/var/log/splunk/nimbus_alert_modalert.log
