# coinbase api

Manually install the project or use ```pip```:
```python
pip install cbpro
#or
pip install git+git://github.com/danpaquin/coinbasepro-python.git
```

### Public Client
Only some endpoints in the API are available to everyone.  The public endpoints
can be reached using ```PublicClient```

```python
import cbpro
public_client = cbpro.PublicClient()
```
