# drug-information
Information about drugs in json format.
# python example
```python3
import json

f = open("drug-information.json", 'r')
info = f.read(); info = json.loads(info)
f.close()
for drug in info:
    hl = info.get(drug).get("half-life")
    if hl != None:
        print(f"half-life of {drug} is {hl}")
```
The above script would list the half-life of "all" the drugs.
