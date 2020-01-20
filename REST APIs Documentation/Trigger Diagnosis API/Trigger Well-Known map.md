
## Trigger input parameter for verify application node

### Input parameters:

| Name | Type | Description |
|---|---|---|
|search_well_known_map_setting |object	|search Well-known map setting|
|search_well_known_map_setting.folder |string	|Customized folder path to save the well known map.|
|search_well_known_map_setting.map_count |integer	|Number of well-known maps allowed to be return. Max number can be 5.|
|search_well_known_map_setting.execute_runbook |bool	|Whether executing runbook on matched maps|
|search_well_known_map_setting.duplicate_map |bool	|Whether duplicate these maps in NetBrain.|

***Example：***


```python
task_parameter = {
    "domain_setting": {
        "tenant_id": "xxx-xxx-xxxx",
        "domain_id": "xxx-xxx-xxxx"
    },
    "basic_setting": {
        "triggered_by": "admin",
        "user": "admin",
        "device": "BJ-R1",
        "stub_name": "Default-Search Well Known Map" // this field is hard coded
    },
    "search_well_known_map_setting": {
        "folder": "Public/Well Known Map/Oracle DB",
        "map_count": 5, // allow up to five well-known maps return
        "execute_runbook": true, // whether executing runbook on matched maps
        "duplicate_map": false
    }
}
```
