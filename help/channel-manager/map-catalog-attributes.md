---
title: Katalogattribute zuordnen
description: Zuordnen von Attributen zum Abgleich [DNL! Commerce-] Produkte in bestehende [!DNL Walmart Marketplace] Auflistungen und Synchronisieren von Daten zwischen [!DNL Channel Manager] und [!DNL Walmart].
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: fac4bbd3985e07b919f986c877b8584da797e6fe
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Katalogattribute zuordnen

Vor der Veröffentlichung von Listen aus [!DNL Commerce] nach [!DNL Walmart Marketplace]müssen Sie mindestens eine eindeutige Kennung aus Ihrem [!DNL Commerce] Katalog zur entsprechenden Kennung von Walmart.
Dieser Schritt muss mit [!DNL Commerce] bereits [!DNL Walmart] Auflistungen und zum Synchronisieren von Produktdaten zwischen [!DNL Commerce] und [!DNL Walmart].

Für die Produktzuordnung muss das Commerce-Produkt über mindestens ein Produktattribut verfügen, das mit einer der folgenden für [!DNL Walmart].

**Erforderliche Walmart-Produkt-IDs**

| **Akzeptierter Typ** | **Name** | **Zweck** | **Zulässige Ziffern** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Globaler Handelsartikel | Allgemeine Verwendung weltweit | 14 Stellen |
| ISBN | Internationale Standardbuchnummer | Papiere, Hardcover und elektronische Bücher | 10 oder 13 Stellen |
| ISSN | Internationale Standardseriennummer | 8-stellige Seriennummer zur Identifizierung von Zeitschriften, Zeitschriften, Zeitungen und Zeitschriften aller Art, die auf allen gedruckten Medien und auf elektronischem Wege zugestellt werden | 8 Stellen |
| UPC | Universeller Produktcode | Standard-Tracking-Code für den Einzelhandel | 12 Stellen |

Wenn Ihr Katalog nicht über ein entsprechendes Attribut verfügt, [Hinzufügen oder Konvertieren eines vorhandenen Katalogattributs](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## Zuordnen eindeutiger Kennungen

1. Im [!UICONTROL Listings] Seite für den Verkaufskanalspeicher auswählen **[!UICONTROL Settings]**.

   - Suchen Sie nach dem Attribut Walmart Marketplace , das zugeordnet werden soll.

   - Wählen Sie das entsprechende Attribut aus der [!DNL Commerce] Katalog speichern.

      Im folgenden Beispiel wird das UPC-Attribut Walmart Marketplace dem Attribut UPC im Produktkatalog zugeordnet.
   ![Zuordnungsattribute für Produktübereinstimmungskriterien](assets/products-map-attributes-for-match.png)
   - Optional können Sie mehrere Attribute zuordnen, um Übereinstimmungen zu erhöhen. Wenn Sie mehr als ein Attribut zuordnen, wählen Sie eines als **Primäre Kennung**. Diese

   - Auswählen **[!UICONTROL Save]**.


## Zugeordnete Attributkonfiguration aktualisieren

Ändern Sie die Commerce-Produktkennung für übereinstimmende Produkte, indem Sie die zugeordneten Attributeinstellungen aktualisieren.

Anstatt beispielsweise Produkte auf Grundlage des Commerce UPC-Produktattribut-Codes zuzuordnen, können Sie eine Übereinstimmung anhand der SKU herstellen. Sie können auch zusätzliche Attribute zuordnen, um die Übereinstimmung zu verbessern.

1. Aus dem **[!UICONTROL Listings]** auswählen **[!UICONTROL Settings]**.

1. Ändern Sie im Formular Zuordnungsattribut die zugeordnete Attributkonfiguration nach Bedarf.
