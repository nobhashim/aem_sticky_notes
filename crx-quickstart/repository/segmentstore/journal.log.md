# jounral.log

## Where

- crx-quickstart/repository/segmentstore/journal.log

## What

- List of the segment ID which contains the root node in chronological order
- Format: Revision 'root' timestamp

```
$ head -3 journal.log
1387fc5c-0346-4ff0-a35b-2507b4d65f06:3134 root 1569820647376
4954257f-6161-4da6-ab9f-274eb1e539de:1285 root 1569820652398
fd4789f7-7ad6-4444-abde-404766022982:1949 root 1569820657412
$
$ tar tf data00000a.tar
141d77a8-da36-45b2-a49f-e2c3c3406fa9.8ce37cda
949d2bf9-1c17-4325-a247-5fce6eaa7a2a.e402b5df
5e0c371b-88fc-4a9e-a567-be435ba8d67b.3d0a8d62
ca3f4b15-903b-4716-ab61-f60787d74da7.07dcd65c
4f6b00d8-ecf9-4e70-a79c-326e87a29dd1.64d38fe7
68c91ca9-c9ce-4156-ac5c-61d4769f1eec.8545fca9
9ef40e10-6caa-4d0b-a971-48d388ff55ef.a562e88a
1c043fa7-db09-4051-aff4-5f6e8a48d9bd.325d75b3
947ef451-f0ff-4d9b-a8f5-3a5693b59e14.b1e83c3f
d882d4a6-39d6-45fe-a751-232dc1ae599f.2b79d0a7
b5b30bf1-7691-4b81-ad80-abfd5fab0ede.6ce8b9ee
5b328d9f-3707-49d1-aac1-a623a5a8c130.c41cf6f0
9386f6b1-c0df-41db-a3bf-8666752f5474.1528e690
1387fc5c-0346-4ff0-a35b-2507b4d65f06.48e9212c
...
data00000a.tar.brf
data00000a.tar.gph
data00000a.tar.idx
$
```

## Remarks

- The revision at the bottom is referred as "head state."

## References

- https://jackrabbit.apache.org/oak/docs/nodestore/segment/overview.html
- https://github.com/apache/jackrabbit-oak/blob/c6ddcc55bee3de915459af01e91edad32d538f3d/oak-segment-tar/src/main/java/org/apache/jackrabbit/oak/segment/file/TarRevisions.java
- https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16542.html

