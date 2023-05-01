
# SGC Enhancement Suite
**The SGC Enhancement Suite is a custom-scoped application designed to help implement and test Service Graph Connectors by allowing admins to import and roll back their CMDB data and gain insights on where their data is landing in the CMDB after imports.**
## About
Service Graph Connectors are the primary methods to get CI data into  your ServiceNow CMDB. As apposed to your typical ServiceNow integration, the Service Graph Connector follows a specific framework laid out by ServiceNow to ensure that all integrations play by the same rules allowing for a consistent multi source CMDB. 

This framework primarily consist of using Flow Designer Data Stream Actions to load data into staging tables and then transforming that data through the Robust Transform Engine (RTE) which uses the Identification and Reconciliation Engine (IRE) to update and insert records into the CMDB while following ServiceNow best practices. 

Although Service Graph Connectors are meant to be easy to set up and start using, depending on the current state of your CMDB this isn't always the case, there are often custom identification rules in place or the source data is not 100% reliable. Once the data is in the CMDB and you find things aren't where they should be, its very hard to untangle.

The SGC Enhancement Suite helps with this by utilizing the out of box platform features to help admins run imports and get full visibility on where that data is going. And if things don't appear as expected, the SGC Enhancement Suite allows you to roll back entire import sets to make it like it never even happened.

**Features:**

 - Transform import sets.
 - Export import summaries for import sets.
 - Roll back import set runs.
 - Transform and roll back individual import set rows.
 - Review target data for each import set row.
 - Review source IDs on CI records.
