# WorldCoinAPI
Инициализация:
```python
from worldcoinapi import api
wc = api(token='токен', merchant_id=ID мерчанта)
```
Получение баланса:
```python
wc.get_balance()
```
```python
wc.get_url(amount=сумма, code=код оплаты, lock=заблокированность)
```
