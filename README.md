# WorldCoinAPI
К сожалению вам придется порытся в файлах модуля, так как вместо .text надо использовать .json(), а PyPi выдает ошибку загрузки.
Установка:
```cmd
pip install worldcoinapi
```
Обновление:
```cmd
pip install --upgrade worldcoinapi
```
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
Получение информации об игроках в списке:
```python
wc.players_info(players=[список игровов])
```
Используются все символы из https://worldcoin.docs.apiary.io/.
Если написано "amount", значит и тут "amount".
Если не указан ID, то все будет работать с 549204433, то есть со мной, так что не забывайте вводить ID.
