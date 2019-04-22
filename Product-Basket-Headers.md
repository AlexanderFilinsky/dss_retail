### Product Basket Headers
[Product Basket Details](https://github.com/smpb05/DSS-Retail/wiki/Product-Basket-Details#product-basket-details)
* docId - Уникальный идентификатор документа
* docTypeMain - Основной тип документа (возможные значения ПРИХОД или РАСХОД)
* docType - Тип документа
* docTypeSub - Под тип документа
* docCreatedUTC - TimeStamp создания
>- [ ] docPaymentDueDate - Дата оплаты по документу. Для наличных оплат `=docCreatedUTC`
* docCoef  - Коэффициент операции (+1, -1) 
>* docClosed ~~Status~~ - Закрыта / Не закрыта (1, 0) Закрыта, когда `docAmountRemain=0`
* isLast - Последний документ
* consumerId - Код покупателя
* supplierId - Код поставщика
* docTotalQuantity - Сумма proQuantity

>~~* docTotalSumNet -  Сумма proPriceNet~~ - ALEF - не вижу смысла в данном поле.
* docTotalSumPurchase - Сумма proPricePurchase
* docTotalSumSale - Сумма proPriceSale
>- [ ] docAmountRemain - Остаток суммы после полученных или выданных оплат