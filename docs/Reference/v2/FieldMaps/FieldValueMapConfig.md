## FieldMaps: FieldValueMapConfig

>**_This documentation is for a preview version of the Azure DevOps Migration Tools._ If you are not using the preview version then please head over to the main [documentation](https://nkdagility.github.io/azure-devops-migration-tools).**

[Overview](../../../index.md) > [Reference](../../index.md) > [API v2](../index.md) > [FieldMaps](index.md)> **FieldValueMapConfig**

Need to map not just the field but also values? This is the default value mapper.

### Options

| Parameter name         | Type    | Description                              | Default Value                            |
|------------------------|---------|------------------------------------------|------------------------------------------|
| defaultValue | String | missng XML code comments | missng XML code comments |
| sourceField | String | missng XML code comments | missng XML code comments |
| targetField | String | missng XML code comments | missng XML code comments |
| valueMapping | Dictionary | missng XML code comments | missng XML code comments |
| WorkItemTypeName | String | missng XML code comments | missng XML code comments |


### Example JSON

```JSON
{
  "$type": "FieldValueMapConfig",
  "WorkItemTypeName": "*",
  "sourceField": "System.Status",
  "targetField": "System.Status",
  "defaultValue": "New",
  "valueMapping": {
    "$type": "Dictionary`2",
    "New": "New",
    "Active": "Committed",
    "Resolved": "Committed",
    "Closed": "Done"
  }
}
```