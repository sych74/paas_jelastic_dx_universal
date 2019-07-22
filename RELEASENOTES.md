# Jahia Universal Package Release notes

## actual version: v1.5

### v1.5 (2019-07-22)
* [BUG]: `DX_VERSION` and `PACKAGE_TYPE` where not updated when upgrading an env
* [BUG]: `set_dd_tag.sh` was removing Datadog agent's `logs_enabled`

### v1.4 (2019-07-05)
* [NEW]: Add license if set
    * we can now fill a optional `license` setting with the base64 encoded license file
    * if not set, the 30 days demo license remain

### v1.3 (2019-07-02)
* [BUG][[PAAS-233](https://jira.jahia.org/browse/PAAS-233)] Add new parameters to `_JAVA_OPTIONS` to avoid some issues
    * `-XX:SurvivorRatio=8 `
    * `-Xmn1G`