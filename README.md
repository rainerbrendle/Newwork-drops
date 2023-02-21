# Newwork-Drops
Active Data Cluster Droplet Model 

A first try for a acitive cluster database using docker and GO-based Droplets on PostgreSQ-like databaseshards with eventual consistency guarantee.

We have a control plane, which manages the cluster's partitions ("shards") 
THe control has several droplets:
- Admin
- Control Plane Journal
- Yellow Pages : actual location of the shards and their purpose
- White Pages: business related information to shards
- Blues Pages: APIs, Objects and Interface directory
- Data Plane and Data Plane Journals
- Stable Views: "Ledgers" and Materialized Views
