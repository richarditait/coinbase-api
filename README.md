# coinbase api

Manually install the project or use ```pip```:
```python
pip install cbpro
#or
pip install git+git://github.com/danpaquin/coinbasepro-python.git
```

### Public Client
Only some endpoints in the API are available to everyone.  The public endpoints
can be reached using ```PublicClient```. In Python:

```python
import cbpro
public_client = cbpro.PublicClient()
```

### Order book at default level
public_client.get_product_order_book('currency-pairing'). For example Bitcoin against Euro:
```python
public_client.get_product_order_book('BTC-EUR')
```
### Order book at a specific level
```python
public_client.get_product_order_book('BTC-EUR', level=1)
```
### Ticker
```python
public_client.get_product_ticker(product_id='BTC-EUR')
```
