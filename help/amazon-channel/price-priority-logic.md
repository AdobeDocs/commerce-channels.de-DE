---
title: Preisprioritätslogik
description: Amazon Sales Kanal setzt bei der Bestimmung des veröffentlichten Preises für eine Amazon-Auflistung Prioritäten.
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

---

# Logik der Preispriorität

Wie bestimmt das System im folgenden Beispiel, ob Sie $31.99, $24.99 oder $27.99 veröffentlichen sollten?

![Handelspreisdefinition](assets/amazon-price-scope.png)

Um zu bestimmen, welcher Preis verwendet wird, wenn ein Produkt auf zwei Websites ist und einen unterschiedlichen Preis pro Website hat, verwenden Sie die Preisprioritätslogik (ermittelt durch [Sortierreihenfolge](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){Zielgruppe=&quot;_blank&quot;} Wert).

Um die Sortierreihenfolge Ihrer Geschäfte Ansicht, gehen Sie zu **[!UICONTROL Stores]** > **[!UICONTROL All Stores]** in _Admin_ Sidebar. In _[!UICONTROL Web Site]_-Spalte, klicken Sie auf den Namen der Website. Die_[!UICONTROL Web Site Information]_ Seite zeigt die _[!UICONTROL Sort Order]_-Einstellung für die Website, die die Priorität der Website bestimmt. Ein Wert von `1` gibt die höchste Priorität an.

Wenn der Produktpreis auf `Use Default`, fällt er auf den Standardpreis anstatt auf den Preis der Website.

## Beispiel 1

|  | Website-Priorität | Preis (Website) | Standard verwenden |
|---|---|---|---|
| Standard | 0 | 31,99 $ | — |
| 1 lagern | 1 | 24,99 $ | Nein |
| Store 2 | 2 | 27,99 $ | Ja |

- Die **[!UICONTROL Magento Price Source]** (definiert in [Listingpreis](./listing-price.md) wird auf `Price` Attribut.
- Sehen Sie sich die Website mit der höchsten Priorität der Website an: Store 1 (definiert von [Sortierreihenfolge](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){Zielgruppe=&quot;_blank&quot;} Wert).
- Da Store 1 auf die Nutzung des Website-Preises eingestellt ist (Standard verwenden = Nein), beträgt der veröffentlichte Preis 24,99 US-Dollar.

## Beispiel 2

|  | Website-Priorität | Preiswebsite | Standard verwenden |
|---|---|---|---|
| Standard | 0 | 31,99 $ | — |
| 1 lagern | 1 | 24,99 $ | Ja |
| Store 2 | 2 | 27,99 $ | Nein |

- Die **[!UICONTROL Magento Price Source]** (definiert in [Listingpreis](./listing-price.md) wird auf `Price` Attribut.
- Sehen Sie sich die Website mit der höchsten Priorität der Website an: Store 1 (definiert von [Sortierreihenfolge](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){Zielgruppe=&quot;_blank&quot;} Wert).
- Seit Store 1 **ist nicht** gesetzt, um den Preis der Website zu verwenden (Standard verwenden = Ja), schauen Sie sich die nächste Website in der Sortierreihenfolge an.
- Seit Store 2 **ist** auf den Preis der Website (Verwenden Sie Standard = Nein) eingestellt, ist der veröffentlichte Preis $27.99.

## Beispiel 3

|  | Website-Priorität | Preiswebsite | Standard verwenden |
|---|---|---|---|
| Standard | 0 | 31,99 $ | 30,00 $ |
| 1 lagern | 1 | 24,99 $ | — |
| Store 2 | 2 | 27,99 $ | 20,00 $ |

In diesem Beispiel wird der Nicht-Preiswert hinzugefügt, der verwendet wird, wenn Sie einen anderen Wert für das _ auswählen[!UICONTROL Magento Price Source_] (definiert in [Listingpreis](./listing-price.md) Einstellungen). Der Non-Price-Wert verwendet immer den Preis als Fallback-Preis.

- Die **[!UICONTROL Magento Price Source]** (definiert in [[!UICONTROL Listing Price]](./listing-price.md) Einstellungen) auf `Non-Price`.
- Sehen Sie sich die Website mit der höchsten Priorität an. `Store 1`(definiert durch [Sortierreihenfolge](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){Zielgruppe=&quot;_blank&quot;} Wert).
- Seit Store 1 **ist nicht** zur Verwendung der `Non-Price` -Attribut, sehen Sie sich die nächste Website in der Sortierreihenfolge an.
- Seit Store 2 **ist** zur Verwendung der `Non-Price` Attribut (Nicht-Preis) [Webseite] = $20.00), der veröffentlichte Preis ist $20.00.
