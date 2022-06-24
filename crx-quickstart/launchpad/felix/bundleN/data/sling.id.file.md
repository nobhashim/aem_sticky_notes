# sling.id.file

## Where

- crx-quickstart/launchpad/felix/bundleN/data/sling.id.file

N is the bundle ID for Apache Sling Settings(org.apache.sling.settings).

Or, you can find the location with find command.

```
$ find crx-quickstart/launchpad/felix -name sling.id.file
```

## What 

- Stores Sling ID

## Remarks

- Sling ID matches with:
  - /var/discovery/oak/clusterInstances/\[UUID\]
  - /var/eventing/jobs/assigned/\[UUID\]
  - slingId property of /var/workflow/instances/server0
- Stop AEM, delete this file, restart AEM regenerated Sling ID.

## See Also

- [Sling > Topology Management](/localhost/system/console/topology.md)

## References

- https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16875.html

