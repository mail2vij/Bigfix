Purpose:
BigFix can now monitor its own attributes (RAM, CPU, Disk, core services, etc.) without requiring an external monitoring tool.

Tools Used:
BigFix + ITSM (Incident Management)

Workflow:
A BigFix Fixlet sets the threshold values for the desired services or attributes to be monitored.
BigFix schedules self-monitoring to periodically check the threshold values.
If a threshold breach is detected, an incident is automatically triggered and assigned to the BigFix Admin group.
Alerts remain on hold until the current issue is resolved, ensuring that no duplicate incidents are created for the same issue.
The BigFix Admin resolves the incident and fixes the issue.
A second Fixlet is executed to automatically close the incident with relevant work notes.
Benefits:
Enables self-monitoring, reducing dependency on external monitoring tools.
Addresses the needs of mid-range customers who prefer not to invest in separate monitoring tools for BigFix infrastructure.
