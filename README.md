# bldb
BiLi search engine DataBase utils

![](https://img.shields.io/pypi/v/bldb?label=bldb&color=blue&cacheSeconds=60)

## Install
```sh
pip install bldb --upgrade
```

## Usage

Run example:

```sh
python example.py
```

See: [example.py](./example.py)

```python
import sys
from pathlib import Path

sys.path.insert(0, str(Path(__file__).parent / "src"))

import bldb

from bldb import MongoOperator, MongoConfigsType


if __name__ == "__main__":
    mongo_configs = {
        "host": "localhost",
        "port": 27017,
        "dbname": "test",
    }
    mongo = MongoOperator(configs=mongo_configs)
```