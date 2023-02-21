# Newwork-drops
Active Data Cluster Droplet Model 

A first try for a acitive cluster database using docker and GO-based Droplets on PostgreSQ-like databaseshards with eventual consistency guarantee.

We have a control plane, which manages the cluster's partitions ("shards") 
THe control has several droplets:
- Admin
- Control plane journal
- Yellow pages : actual location of the shards and their purpose
- White pages: business related information to shards
- Blues pages: APIs, Objects and Interface directory
- Data plane and data plane journals
- Stable Views
