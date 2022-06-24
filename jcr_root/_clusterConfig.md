# /:clusterConfig

## Where

- /:clusterConfig

## What

- Stores cluster view ID or cluster ID as :clusterId property

## Remarks

- This node is invisible with CRX/DE.
- Oak-run console or explore can access this node.
- The cluster view ID is a unique indentifier of each repository.
- OSGi console > Statys > Topology Management shows the cluster view ID.
- The cluster view ID is also used as repository-\[UUID\] in datastore.
- When you clone an AEM instance, you need to reset the cluster ID with oak-run tool.

```
$ java -jar oak-run.jar resetclusterid crx-quickstart/repository/segmentstore
```

## References

- https://experienceleague.adobe.com/docs/experience-manager-65/deploying/deploying/data-store-config.html
- https://sling.apache.org/documentation/bundles/discovery-api-and-impl.html
- https://github.com/apache/jackrabbit-oak/blob/c6ddcc55bee3de915459af01e91edad32d538f3d/oak-store-spi/src/main/java/org/apache/jackrabbit/oak/spi/cluster/ClusterRepositoryInfo.java
- https://github.com/apache/jackrabbit-oak/blob/c6ddcc55bee3de915459af01e91edad32d538f3d/oak-run/src/main/java/org/apache/jackrabbit/oak/run/ResetClusterIdCommand.java


