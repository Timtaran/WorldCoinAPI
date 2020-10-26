# WorldCoinAPI
Установка:
Я не знаю как создать установку, так что просто перенесите файл рядом с кодом :)
Если можете помочь - https://vk.com/timtaran_yt
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
Отправка монет игроку:
```python
wc.players_pay(to=кому отправить, amount=сумма, code=код оплаты)
```
Получение списка игроков:
```python
wc.players_info(players=[список игровов])
```
Используются все символы из https://worldcoin.docs.apiary.io/.
Если написано "amount", значит и тут "amount".
Если не указан ID, то все будет работать с 549204433, то есть со мной, так что не забывайте вводить ID.
