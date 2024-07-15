---
title: Amazon-Vertriebskanal - Logik der Preispriorität
description: Der Amazon-Vertriebskanal wendet bei der Bestimmung des veröffentlichten Preises für eine Amazon-Auflistung eine Priorisierung an.
feature: Sales Channels, Price Rules
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 2%

---

# Preisprioritätslogik

Wie ermittelt das System im folgenden Beispiel, ob Sie $31.99, $24.99 oder $27.99 veröffentlichen sollten?

![Commerce-Preisbereich](assets/amazon-price-scope.png){width="400"}

Um zu bestimmen, welcher Preis verwendet wird, wenn sich ein Produkt auf zwei Websites befindet und einen variierenden Preis pro Website hat, verwenden Sie die Preisprioritätslogik (bestimmt durch den Wert [Sortierreihenfolge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) ).

Um die Sortierreihenfolge Ihrer Stores anzuzeigen, gehen Sie in der Seitenleiste _Admin_ zu **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** . Klicken Sie in der Spalte _[!UICONTROL Web Site]_auf den Namen der Website. Auf der Seite &quot;_[!UICONTROL Web Site Information]_&quot;wird die Einstellung &quot;_[!UICONTROL Sort Order]_&quot;für die Website angezeigt, die die Priorität der Website bestimmt. Der Wert `1` gibt die höchste Priorität an.

Wenn der Produktpreis auf `Use Default` gesetzt ist, wird anstelle des Website-Preiswerts der Standardpreis verwendet.

## Beispiel 1

|         | Website-Priorität | Preis (Website) | Use Default |
|---------|------------------|-----------------|-------------|
| Standard | 0 | 31,99 $ | — |
| Store 1 | 1 | 24,99 $ | Nein |
| Store 2 | 2 | 27,99 $ | Ja |

- Der **[!UICONTROL Magento Price Source]** (definiert in Ihrem [Listing Price](./listing-price.md)) ist auf das Attribut `Price` festgelegt.
- Sehen Sie sich die Website mit der höchsten Website-Priorität an, nämlich Store 1 (definiert durch den Wert [Sortierreihenfolge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) ).
- Da Store 1 auf die Verwendung des Website-Preises festgelegt ist (Use Default = No), beträgt der veröffentlichte Preis 24,99 USD.

## Beispiel 2

|         | Website-Priorität | Preiswebsite | Use Default |
|---------|------------------|---------------|-------------|
| Standard | 0 | 31,99 $ | — |
| Store 1 | 1 | 24,99 $ | Ja |
| Store 2 | 2 | 27,99 $ | Nein |

- Der **[!UICONTROL Magento Price Source]** (definiert in Ihrem [Listing Price](./listing-price.md)) ist auf das Attribut `Price` festgelegt.
- Sehen Sie sich die Website mit der höchsten Website-Priorität an, nämlich Store 1 (definiert durch den Wert [Sortierreihenfolge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) ).
- Da Store 1 **nicht** für die Verwendung des Website-Preises festgelegt ist (Use Default = Ja), sehen Sie sich die nächste Website in der Sortierreihenfolge an.
- Da Store 2 **auf** gesetzt ist, um den Website-Preis zu verwenden (Use Default = No), beträgt der veröffentlichte Preis 27,99 USD.

## Beispiel 3

|         | Website-Priorität | Preiswebsite | Use Default |
|---------|------------------|---------------|-------------|
| Standard | 0 | 31,99 $ | 30,00$ |
| Store 1 | 1 | 24,99 $ | — |
| Store 2 | 2 | 27,99 $ | 20,00$ |

In diesem Beispiel wird der Wert ohne Preis hinzugefügt, der verwendet wird, wenn Sie einen anderen Wert für _[!UICONTROL Magento Price Source_] auswählen (definiert in Ihren Einstellungen für [Listenpreis](./listing-price.md)). Der Wert ohne Preis verwendet immer den Preis als Ausweichpreis.

- Der **[!UICONTROL Magento Price Source]** (definiert in den [[!UICONTROL Listing Price]](./listing-price.md) Einstellungen) ist auf `Non-Price` gesetzt.
- Sehen Sie sich die Website mit der höchsten Website-Priorität an, nämlich &quot;`Store 1`&quot;(definiert durch den Wert &quot;[Sortierreihenfolge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)&quot;).
- Da Store 1 **nicht** für die Verwendung des Attributs `Non-Price` festgelegt ist, sehen Sie sich die nächste Website in der Sortierreihenfolge an.
- Da der Store 2 **auf** eingestellt ist, um das Attribut `Non-Price` zu verwenden (Non-Price [Website] = 20,00 USD), beträgt der veröffentlichte Preis 20,00 USD.
