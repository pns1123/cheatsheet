##### read data.json to data_dict
```
import json
with open('data.json', 'r') as f:
    data_dict = json.load(f)

```

##### write data_dict to data.json
- use 4 spaces for indentation
- sort keys in ascending order
```
import json
with open('file.json', 'w') as f:
    data_dict = json.dump(data_dict, f, indent=4, sort_keys=True)

```

##### json.loads
##### json.dumps
