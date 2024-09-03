# Documentación de la Orden de Compra y Artículos

## Estructura JSON

El JSON se divide en dos secciones principales: `purchaseOrder` y `item`. A continuación, se describen los campos incluidos en cada una de estas secciones.

---

### **Sección: purchaseOrder (Orden de Compra)**

| Variable                         | Tipo       | Descripción                                        | Ejemplo                                                   |
|----------------------------------|------------|----------------------------------------------------|-----------------------------------------------------------|
| `localization`                   | `string`   | Localización de la orden de compra                  | `"PANAMÁ"`                                                |
| `seller`                         | `string`   | Nombre del vendedor                                 | `"ASTR THE LABEL"`                                        |
| `companyName`                    | `string`   | Nombre de la empresa                                | `"IMPORTADORA MADURO"`                                    |
| `receivedAt`                     | `string`   | Fecha de recepción de la orden de compra            | `"2024-09-03T10:00:00Z"`                                  |
| `currencyTotalCashExcludingTax`  | `string`   | Código de divisa para el total sin impuestos        | `"USD"`                                                   |
| `direccion_tr`                   | `string`   | Dirección de entrega                                | `"Avenida Central, Panamá"`                               |
| `eta`                            | `date`     | Fecha estimada de entrega                           | `"2024-09-10"`                                            |
| `paymentTerms`                   | `string`   | Términos de pago                                    | `"NET 30"`                                                |
| `totalCashExcludingTax`          | `number`   | Valor total sin impuestos                           | `1000.00`                                                 |
| `destinationPoint`               | `object`   | Detalles del punto de destino                       | `{"country": "PA", "city": "Panamá", "addressLocation": "Avenida Central"}` |
| `hasBooking`                     | `boolean`  | Indica si tiene reserva                             | `true`                                                    |
| `currencyTotalTaxValue`          | `string`   | Código de divisa para el valor total del impuesto   | `"USD"`                                                   |
| `taxFree`                        | `boolean`  | Indica si está libre de impuestos                   | `false`                                                   |
| `currencyTotalCashIncludingTax`  | `string`   | Código de divisa para el total con impuestos        | `"USD"`                                                   |
| `orderDeliveryDate`              | `date`     | Fecha de entrega de la orden                        | `"2024-09-10"`                                            |
| `contactName`                    | `string`   | Nombre del contacto                                 | `"Juan Pérez"`                                            |
| `paymentInstructions`            | `string`   | Instrucciones de pago                               | `"Pagar mediante transferencia bancaria"`                 |
| `additionalCostsCode`            | `string`   | Código de costos adicionales                        | `"FLETE"`                                                 |
| `estimatedDeliveryDate`          | `date`     | Fecha estimada de entrega                           | `"2024-09-12"`                                            |
| `buyer`                          | `string`   | Nombre del comprador                                | `"Importadora S.A."`                                      |
| `additionalCostsValue`           | `number`   | Valor de costos adicionales                         | `150.00`                                                  |
| `incoterm`                       | `string`   | Términos de envío                                   | `"FOB"`                                                   |
| `paymentMethod`                  | `string`   | Método de pago                                      | `"Transferencia bancaria"`                                |
| `orderDate`                      | `date`     | Fecha de la orden                                   | `"2024-08-15"`                                            |
| `pickupPoint`                    | `object`   | Detalles del punto de recogida                      | `{"country": "US", "city": "Miami", "addressLocation": "NW 21st St"}` |
| `documentType`                   | `string`   | Tipo de documento                                   | `"Factura"`                                               |
| `origin`                         | `string`   | Punto de origen                                     | `"Miami"`                                                 |
| `destination`                    | `string`   | Punto de destino                                    | `"Panamá"`                                                |
| `uid`                            | `string`   | Identificador único                                 | `"4Trb64aDFRTbRivq2sQdtxwu6En2"`                          |
| `shipmentCarrier`                | `string`   | Transportista                                       | `"DHL"`                                                   |
| `incotermName`                   | `string`   | Nombre del incoterm                                 | `"Free on Board"`                                         |
| `shipmentVia`                    | `string`   | Método de envío                                     | `"Aéreo"`                                                 |
| `contactNumber`                  | `string`   | Número de contacto                                  | `"+507 123-4567"`                                         |
| `additionalCostsDescripiton`     | `string`   | Descripción de los costos adicionales               | `"Costo por flete"`                                       |
| `confirmCount`                   | `number`   | Número de confirmaciones                            | `1`                                                       |
| `documentStatus`                 | `string`   | Estado del documento                                | `"En proceso"`                                            |
| `requestedDate`                  | `date`     | Fecha requerida                                     | `"2024-08-20"`                                            |
| `sendedFrom`                     | `string`   | Enviado desde                                       | `"ASTR THE LABEL"`                                        |
| `sendedTo`                       | `string`   | Enviado a                                           | `"IMPORTADORA MADURO"`                                    |
| `buyerNameContactNumber`         | `string`   | Nombre y número de contacto del comprador           | `"Luis Rodríguez, +507 987-6543"`                        |
| `contactEmail`                   | `string`   | Correo electrónico de contacto                      | `"contacto@importadoramaduro.com"`                        |
| `approval`                       | `boolean`  | Aprobación                                          | `true`                                                    |
| `entityId`                       | `string`   | Código de entidad                                   | `"ENT12345"`                                              |
| `additionalDetails`              | `string`   | Detalles adicionales                                | `"Ninguno"`                                               |
| `buyerName`                      | `string`   | Nombre del comprador                                | `"Importadora Maduro S.A."`                               |
| `totalTaxValue`                  | `number`   | Valor total de impuestos                            | `120.00`                                                  |
| `confirmDate`                    | `date`     | Fecha de confirmación                               | `"2024-08-18"`                                            |
| `companyAddress`                 | `string`   | Dirección de la compañía                            | `"Avenida Central, Panamá"`                               |
| `purchaseOrder`                  | `string`   | Número de orden de compra                           | `"5100056042"`                                            |
| `totalCashIncludingTax`          | `number`   | Valor total incluyendo impuestos                    | `1120.00`                                                 |
| `createdAt`                      | `date`     | Fecha de creación                                   | `"2024-08-17T15:15:16Z"`                                  |
| `trakingNumber`                  | `string`   | Número de rastreo                                   | `"EbyKyKAF2M0yFCCW8epf"`                                  |
| `shipmentId`                     | `string`   | Identificador de envío                              | `"SHIP12345"`                                             |
| `shipmentNumber`                 | `string`   | Número de envío                                     | `"00000013"`                                              |
| `trackingNumber`                 | `string`   | Número de seguimiento                               | `"TRACK123456789"`                                        |
| `companyParent`                  | `string`   | Compañía matriz                                     | `"ATL"`                                                   |
| `company`                        | `string`   | Compañía filial                                     | `"IMPORTADORA MADURO"`                                    |
| `status`                         | `string`   | Estado de la orden                                  | `"DELIVERED"`                                             |


### Ejemplo Completo de JSON - Orden de Compra

```json
{
    "localization": "PANAMÁ",
    "seller": "ASTR THE LABEL",
    "companyName": "IMPORTADORA MADURO",
    "receivedAt": "2024-09-03T10:00:00Z",
    "currencyTotalCashExcludingTax": "USD",
    "direccion_tr": "Avenida Central, Panamá",
    "eta": "2024-09-10",
    "paymentTerms": "NET 30",
    "totalCashExcludingTax": 1000.00,
    "destinationPoint": {
        "country": "PA",
        "city": "Panamá",
        "addressLocation": "Avenida Central"
    },
    "hasBooking": true,
    "currencyTotalTaxValue": "USD",
    "taxFree": false,
    "currencyTotalCashIncludingTax": "USD",
    "orderDeliveryDate": "2024-09-10",
    "contactName": "Juan Pérez",
    "paymentInstructions": "Pagar mediante transferencia bancaria",
    "additionalCostsCode": "FLETE",
    "estimatedDeliveryDate": "2024-09-12",
    "buyer": "Importadora S.A.",
    "additionalCostsValue": 150.00,
    "incoterm": "FOB",
    "paymentMethod": "Transferencia bancaria",
    "orderDate": "2024-08-15",
    "pickupPoint": {
        "country": "US",
        "city": "Miami",
        "addressLocation": "NW 21st St"
    },
    "documentType": "Factura",
    "origin": "Miami",
    "destination": "Panamá",
    "uid": "4Trb64aDFRTbRivq2sQdtxwu6En2",
    "shipmentCarrier": "DHL",
    "incotermName": "Free on Board",
    "shipmentVia": "Aéreo",
    "contactNumber": "+507 123-4567",
    "additionalCostsDescripiton": "Costo por flete",
    "confirmCount": 1,
    "documentStatus": "En proceso",
    "requestedDate": "2024-08-20",
    "sendedFrom": "ASTR THE LABEL",
    "sendedTo": "IMPORTADORA MADURO",
    "buyerNameContactNumber": "Luis Rodríguez, +507 987-6543",
    "contactEmail": "contacto@importadoramaduro.com",
    "approval": true,
    "entityId": "ENT12345",
    "additionalDetails": "Ninguno",
    "buyerName": "Importadora Maduro S.A.",
    "totalTaxValue": 120.00,
    "confirmDate": "2024-08-18",
    "companyAddress": "Avenida Central, Panamá",
    "purchaseOrder": "5100056042",
    "totalCashIncludingTax": 1120.00,
    "createdAt": "2024-08-17T15:15:16Z",
    "trakingNumber": "EbyKyKAF2M0yFCCW8epf",
    "shipmentId": "SHIP12345",
    "shipmentNumber": "00000013",
    "trackingNumber": "TRACK123456789",
    "companyParent": "ATL",
    "company": "IMPORTADORA MADURO",
    "status": "DELIVERED"
}
```
---

### **Sección: item (Artículo)**

| Variable                         | Tipo       | Descripción                                        | Ejemplo                                                   |
|----------------------------------|------------|----------------------------------------------------|-----------------------------------------------------------|
| `itemNumber`                     | `number`   | Posición Material en OC                             | `1`                                                       |
| `pickupPoint`                    | `object`   | Detalles del punto de recogida                      | `{"country": "US", "city": "Miami", "addressLocation": "NW 21st St"}` |
| `currencyTaxRateBaseAmount`      | `number`   | Base imponible del impuesto en la divisa            | `71.75`                                                   |
| `taxRatePercentage`              | `number`   | Porcentaje del impuesto aplicado                    | `7`                                                       |
| `description`                    | `string`   | Descripción detallada del producto                  | `"MUJER-RS SEÑORA"`                                       |
| `packageType`                    | `string`   | Tipo de empaque utilizado para el artículo          | `"PIEZA"`                                                 |
| `pendingQuantity`                | `number`   | Cantidad pendiente                                  | `0`                                                       |
| `confirmPendingDate`             | `date`     | Fecha de confirmación de cantidad pendiente         | `null`                                                    |
| `additionalNotes`                | `string`   | Notas adicionales                                   | `"Ninguna"`                                               |
| `sku`                            | `string`   | Código único de identificación del producto         | `"000000150184850001"`                                    |
| `unitValue`                      | `number`   | Valor por unidad del artículo en la orden de compra | `71.75`                                                   |
| `totalValue`                     | `number`   | Valor total de la línea de artículos                | `71.75`                                                   |
| `destinationPoint`               | `object`   | Detalles del punto de destino                       | `{"country": "PA", "city": "Panamá", "addressLocation": "Avenida Central"}` |
| `lastConsignee`                  | `string`   | Último consignatario                                | `"IMPORTADORA MADURO"`                                    |
| `taxRateValue`                   | `number`   | Valor del impuesto aplicado                         | `5.02`                                                    |
| `releaseDate`                    | `date`     | Fecha de liberación del artículo                    | `2024-08-15`                                              |
| `center`                         | `string`   | Centro de distribución                              | `"CENTRAL"`                                               |
| `confirmQuantity`                | `number`   | Cantidad confirmada                                 | `1`                                                       |
| `warehouse`                      | `string`   | Almacén donde se encuentra el artículo              | `"ALMACEN 1"`                                             |
| `taxRateBaseAmount`              | `number`   | Base imponible del impuesto                         | `71.75`                                                   |
| `tariffItem`                     | `string`   | Partida Arancelaria                                 | `"1234567890"`                                            |
| `currencyTotalValue`             | `string`   | Código de divisa para el valor total                | `"USD"`                                                   |
| `confirmDate`                    | `date`     | Fecha de confirmación                               | `"2024-08-18"`                                            |
| `requiredAmount`                 | `number`   | Cantidad requerida                                  | `1`                                                       |
| `purchaseOrder`                  | `string`   | Número de orden de compra                           | `"5100056042"`                                            |
| `currencyUnitValue`              | `number`   | Valor unitario en divisa                            | `71.75`                                                   |
| `additionalInstructions`         | `string`   | Instrucciones adicionales                           | `"Ninguna"`                                               |
| `currencyTaxRateValue`           | `number`   | Valor del impuesto en divisa                        | `5.02`                                                    |
| `taxRateCode`                    | `string`   | Código de impuesto                                  | `"IMPUESTO7"`                                             |
| `companyParent`                  | `string`   | Compañía matriz                                     | `"ATL"`                                                   |
| `company`                        | `string`   | Compañía filial                                     | `"IMPORTADORA MADURO"`                                    |

### Ejemplo Completo de JSON - Item

```json
{
    "itemNumber": 1,
    "pickupPoint": {
        "country": "US",
        "city": "Miami",
        "addressLocation": "NW 21st St"
    },
    "currencyTaxRateBaseAmount": 71.75,
    "taxRatePercentage": 7,
    "description": "MUJER-RS SEÑORA",
    "packageType": "PIEZA",
    "pendingQuantity": 0,
    "confirmPendingDate": null,
    "additionalNotes": "Ninguna",
    "sku": "000000150184850001",
    "unitValue": 71.75,
    "totalValue": 71.75,
    "destinationPoint": {
        "country": "PA",
        "city": "Panamá",
        "addressLocation": "Avenida Central"
    },
    "lastConsignee": "IMPORTADORA MADURO",
    "taxRateValue": 5.02,
    "releaseDate": "2024-08-15",
    "center": "CENTRAL",
    "confirmQuantity": 1,
    "warehouse": "ALMACEN 1",
    "taxRateBaseAmount": 71.75,
    "tariffItem": "1234567890",
    "currencyTotalValue": "USD",
    "confirmDate": "2024-08-18",
    "requiredAmount": 1,
    "purchaseOrder": "5100056042",
    "currencyUnitValue": 71.75,
    "additionalInstructions": "Ninguna",
    "currencyTaxRateValue": 5.02,
    "taxRateCode": "IMPUESTO7",
    "companyParent": "ATL",
    "company": "IMPORTADORA MADURO"
}
```
