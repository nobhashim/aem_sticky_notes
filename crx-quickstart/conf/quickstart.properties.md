# quickstart.properties

## Where

- crx-quickstart/conf/quickstart.properties

## What

- Stores the build number of AEM

## Remarks

- AEM generates this file at the first launch from the quickstart JAR.
- The build number of this file determines INSTALL/UPGRADE/RESTART mode.
- In-place upgrade without this file fails because the mode will not become UPGRADE.

