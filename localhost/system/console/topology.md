# Topology Management

- OSGi console > Sling > Topology Management
- http://server:port/system/console/topology

## What 

- View Sling ID/Cluster View ID/Leader status

## When 

- Find Sling ID and Cluster View ID
- Find the leader instance of a MongoMK cluster.

## Remarks

- Sling ID matches with:
  - /var/discovery/oak/clusterInstances/\[UUID\]
  - /var/eventing/jobs/assigned/\[UUID\]
  - slingId property of /var/workflow/instances/server0
- Cluster View ID matches with:
  - clusterId property of /:clusterConfig
  - crx-quickstart/repository/datastore/repository-\[UUID\]
  - The first half of login-token cookie

## See Also

- [Status > Topology Management](status-topology.md)
- [sling.id.file](/crx-quickstart/launchpad/felix/bundleN/data/sling.id.file.md)
- [/:clusterConfig](/jcr_root/_clusterConfig.md)

