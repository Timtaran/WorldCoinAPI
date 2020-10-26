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
Получение ссылки:
```python
wc.get_url(amount=сумма, code=код оплаты, lock=заблокированность изменения суммы)
```
Получение истории платежей:
```python
wc.get_history(filter=фильтр, count=число платежей, offset=смещение выборки)
```
Используются все символы из https://worldcoin.docs.apiary.io/.
Если написано "amount", значит и тут "amount"/
