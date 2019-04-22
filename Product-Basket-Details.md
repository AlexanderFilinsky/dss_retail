[Product Basket Headers](https://github.com/smpb05/DSS-Retail/wiki/Product-Basket-Headers#product-basket-headers)
### Product Basket Details
* dodId - Уникальный идентификатор детали документа
* proId - код продукта
* proQuantity - количество продукта
* proPriceNet - себестоимость продуктана момент опреации
* proPricePurchase - Цена покупки
* proPriceSale - Цена продажи 
* proStock - Остаток по продукту ~~(калькулируемое, используем для закрытия документа - <docStatus>~~)
>- [ ] proClosed - Значения Закрыт/Открыт (1/0). Значение закрыт в момент когда `proStock = 0`
* dodDocId - [Ссылка на docId](https://github.com/smpb05/DSS-Retail/wiki/Product-Basket-Headers#product-basket-headers) - заголовок документа