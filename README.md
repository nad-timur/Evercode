# Evercode
Тестовое задание на позицию QA Automation Engineer

Задача №1 - написать тест кейсы для 2 эндпоинтов публичной апи:

Сервис Fiat Market Rates отдает цены всех возможных криптомонет к фиатным валютам. В нем 2 эп:
Get Supported crypto-fiat currencies (Отдает список поддерживаемых валют)
Get Current crypto-fiat prices (Отдает цены всех возможных криптовалют к фиатным валютам)
Апи документация https://documenter.getpostman.com/view/10641191/2s8Z6vXtLX#d0c89495-686c-4c33-be04-c62410a19e26

Бизнес требования:
1) сервис поддерживает все криптовалюты, которые есть в эндпоинте партнера https://coinmarketcap.com/api/documentation/v1/#operation/getV1CryptocurrencyMap
2) цены можно запрашивать как по символам валют так и по специальным ID - coinmarketcap ID. Их также можно найти в эндпоинте партнера из пункта 1)
3) цены обновляются каждые 5 минут. Проверку цен можно осуществлять на ресурсе https://coinmarketcap.com/converter/
4)  Avg time response при нагрузке 30 параллельных запросов не больше 500 ms

Задача №2 - Используя эндпоинты, указанные выше, найти цену криптовалюты ETH к USD - записать время когда дернули запрос и значение из тела респонса
Данные для Авторизации:
Auth: Api key
Header name: x-api-key
Header value: 280cb789-2eba-405b-89f4-1b7ad920244b
