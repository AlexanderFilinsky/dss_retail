# CashOperations
Связана с таблицей [Product Basket Headers](https://github.com/smpb05/DSS-Retail/wiki/Product-Basket-Headers#product-basket-headers)

предназначена для хранения операций с денежными средствами, как наличными, так и безналичными.

* docId - Уникальный идентификатор документа
* docTypeMain - Основной тип документа (возможные значения ПРИХОД или РАСХОД)
* docType - Тип документа
* docTypeSub - Под тип документа
* docCreatedUTC - TimeStamp создания
* docCoef  - Коэффициент операции (+1, -1) 
* docClosed  Закрыта / Не закрыта (1, 0) Закрыта, когда `docAmountRemain=0`
* isLast - Последний документ
* consumerId - Код покупателя
* supplierId - Код поставщика
* docAmount - Сумма документа
* docAmountRemain - Остаток суммы после применения к задолженности
* cashType - Тип оплаты, Наличный или Безналичный
* CashTotal - Накапливающийся остаток по наличным деньгам
* CashRef - опчиональный комментарий к наличной оплате
* bankTotal - Накпливающийся остаток по Банку
* bankRef - опционально номер банковского счета
* creditCardTotal - Накапливающийся остаток по кредитным картам
* creditCardRef - опционально номер кредитной карты
* dodDocId - [Ссылка на docId](https://github.com/smpb05/DSS-Retail/wiki/Product-Basket-Headers#product-basket-headers) - заголовок документа