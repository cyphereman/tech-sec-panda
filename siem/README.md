*TECH STACK*

*Log Analysis - Wazuh*
- Analyze logs received from endpoints / services
- Determine the seveirty of the logs ingested via log analysis. Supported abaility for custom rules
- Ability to discard boisy alerts to limit overflow of unncessary data

*Log Ingestion - Graylog*
- Collect logs originating on endpoint devices, network devices, or 3rd party services,
- Normalize log fields to a universale name so that faster searching and better visaulizations ca be built. Example, source_ip, source_ipv4 should both be rewritten to a src_ip field
- Ensure caching of logs if backed storage is busy or offline

*Backend Storage - Wazuh Indexer (Ioen Search Fork)*
- Store received logs for periods of time
- Fast searching and viewing of data
- Ability to rovide access control to stored logs

*Visualization - Grafana*
- Ability to view logs via widgets/dashboards/etc.
- Fast searching and viewing of data
- Support ability to read from multiple log storages (Elasticsearch, MyQL, Azure, etc,)

*Intelligence Enrichment - OpenCTI / MISP*
- Enrich received log with threat intelligence gathered from various providers
- Ability to parse and store selected responses so that only crucial data is stored
- Automated so that SOC analysts fo not manually have to attempt to enrich logs

*Case Management - TheHIVE / Cortex*
- Platform to view and high react to HIGH severity events
- Allow collaboration with multiple SOC analysts
- Allow reponsive actions so that analysts can trigger events on their endpoints

*Automate - Shuffle*
- SOAR Platform
- Ability to automate to workflows in response to critical alerts, failed healthchecks tr ticket analysis
- Fully customizable and fast

*Investigation - Velociraptor*
 - Similar to Wazuh Agent, it also sits on endpoints
 - Incident Response, Quarantine a device
 - Ability to remotely collect endpoint forensics like URLs, etc.

 *Health Monitoring - InfluxDB / Uptime Kuma*
 - Monitor resources and services consumed on endpoints
 - Monitor services / process whose stoppage would cause operational impact
 - Ability to alert in real time when health check thresholds are met
 - Checks if front end web apps are accessible

 ![image](https://github.com/Saif-Ur-Rehmn/tech-sec-panda/assets/62953610/b6bd0e9b-652a-458d-a60f-743fb0747f7b)

