# Newwork-Drops
Active Data Cluster Droplet Model 

A first try for a acitive cluster database using docker and GO-based Droplets on PostgreSQ-like databaseshards with eventual consistency guarantee.

We have a control plane, which manages the cluster's partitions ("shards").

THe control has several droplets:
- Admin
- Control Plane Journal and a High-Water Mark
- Yellow Pages : actual location of the shards and their purpose
- White Pages: business related information to shards
- Blues Pages: APIs, Objects and Interface directory
- Data Plane and Data Plane Journals and approriate High-Water Marks
- Stable Views: "Ledgers" and Materialized Viewsd a

A Droplet is a colletion of a database schema, GO-based Web Server delivery layer for headless API acess and a database access layer basically per model data type.
