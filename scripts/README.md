Scripts
=======

Use `collectValues.py` to collect unit, building and tech stats such as costs
from a json file generated by the aoe2dat project (https://github.com/HSZemi/aoe2dat).

Use `kvms2json.py` to turn a `key-value-modded-strings-utf8.txt` file into a json
formatted file to be uses as a source for the tech tree. You can also add the values from `collectValues.py`
as metadata. Neat!

Example invocation:

```
./collectValues.py full.json > /tmp/values.json
./kvms2json.py key-value-modded-strings-utf8.txt /tmp/values.json > ../data/data.json
```