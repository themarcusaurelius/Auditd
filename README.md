# Collects and parses logs from the audit daemon (auditd).

When you run the module, it performs a few tasks under the hood:

- Sets the default paths to the log files (but don’t worry, you can override the defaults)
- Makes sure each multiline log event gets sent as a single event
- Uses ingest node to parse and process the log lines, shaping the data into a structure suitable for visualizing in Kibana
- Deploys dashboards for visualizing the log data

### Compatibility
The auditd module was tested with logs from auditd on OSes like CentOS 6 and CentOS 7.

This module is not available for Windows.

