---
title: Amazon-Vertriebskanal - Logik der Preispriorität
description: Der Amazon-Vertriebskanal wendet bei der Bestimmung des veröffentlichten Preises für eine Amazon-Auflistung eine Priorisierung an.
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 077d680da3c98ef9a48958eb548a9d5c1612f74e
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 4%

---

# Preisprioritätslogik

Wie ermittelt das System im folgenden Beispiel, ob Sie $31.99, $24.99 oder $27.99 veröffentlichen sollten?

![Umfang der Handelspreise](assets/amazon-price-scope.png){width="400"}

Um zu bestimmen, welcher Preis verwendet wird, wenn sich ein Produkt auf zwei Websites befindet und einen variierenden Preis pro Website hat, verwenden Sie die Preisprioritätslogik (bestimmt durch die Variable [Sortierreihenfolge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) -Wert).

Um die Sortierreihenfolge Ihrer Stores anzuzeigen, gehen Sie zu **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** im _Admin_ Seitenleiste. Im _[!UICONTROL Web Site]_klicken Sie auf den Namen der Website. Die_[!UICONTROL Web Site Information]_ -Seite zeigt die _[!UICONTROL Sort Order]_-Einstellung für die Website, die die Priorität der Website bestimmt. Ein Wert von `1` gibt die höchste Priorität an.

Wenn der Produktpreis auf `Use Default`, wird der Standardwert anstelle des Website-Preiswerts zurückgesetzt.

## Beispiel 1

|  | Website-Priorität | Preis (Website) | Use Default |
|---|---|---|---|
| Standard | 0 | $31.99 | -- |
| Store 1 | 1 | $24.99 | Nein |
| Store 2 | 2 | $27.99 | Ja |

- Die **[!UICONTROL Magento Price Source]** (definiert in [Listenpreis](./listing-price.md) auf `Price` -Attribut.
- Sehen Sie sich die Website mit der höchsten Website-Priorität an, nämlich Store 1 (definiert durch [Sortierreihenfolge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) -Wert).
- Da Store 1 auf die Verwendung des Website-Preises festgelegt ist (Use Default = No), beträgt der veröffentlichte Preis 24,99 USD.

## Beispiel 2

|  | Website-Priorität | Preiswebsite | Use Default |
|---|---|---|---|
| Standard | 0 | $31.99 | -- |
| Store 1 | 1 | $24.99 | Ja |
| Store 2 | 2 | $27.99 | Nein |

- Die **[!UICONTROL Magento Price Source]** (definiert in [Listenpreis](./listing-price.md) auf `Price` -Attribut.
- Sehen Sie sich die Website mit der höchsten Website-Priorität an, nämlich Store 1 (definiert durch [Sortierreihenfolge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) -Wert).
- Seit Store 1 **ist nicht** auf den Website-Preis eingestellt ist (Use Default = Ja), sehen Sie sich die nächste Website in der Sortierreihenfolge an.
- Seit Store 2 **is** festgelegt ist, um den Website-Preis zu verwenden (Use Default = No), beträgt der veröffentlichte Preis 27,99 USD.

## Beispiel 3

|  | Website-Priorität | Preiswebsite | Use Default |
|---|---|---|---|
| Standard | 0 | $31.99 | $30.00 |
| Store 1 | 1 | $24.99 | -- |
| Store 2 | 2 | $27.99 | $20.00 |

In diesem Beispiel wird der Wert ohne Preis hinzugefügt, der verwendet wird, wenn Sie einen anderen Wert für _ auswählen[!UICONTROL Magento Price Source_] (definiert in [Listenpreis](./listing-price.md) -Einstellungen). Der Wert ohne Preis verwendet immer den Preis als Ausweichpreis.

- Die **[!UICONTROL Magento Price Source]** (definiert in [[!UICONTROL Listing Price]](./listing-price.md) Einstellungen) auf `Non-Price`.
- Sehen Sie sich die Website mit der höchsten Website-Priorität an, d. h. `Store 1`(definiert durch [Sortierreihenfolge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) -Wert).
- Seit Store 1 **ist nicht** , um `Non-Price` -Attribut, sehen Sie sich die nächste Website in der Sortierreihenfolge an.
- Seit Store 2 **is** , um `Non-Price` attribute (non-Price) [Webseite] = 20,00 USD), beträgt der veröffentlichte Preis 20,00 USD.
