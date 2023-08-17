---
title: Katalogattribute zuordnen
description: 'Zuordnen von Attributen zum Abgleich [DNL! Commerce-] Produkte in bestehende [!DNL Walmart Marketplace] Auflistungen und Daten synchronisieren zwischen [!DNL Channel Manager] und [!DNL Walmart].'
feature: Sales Channels, Merchandising, Products
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Katalogattribute zuordnen

Vor der Verbindung von Listen aus [!DNL Commerce] nach [!DNL Walmart Marketplace]müssen Sie mindestens eine eindeutige Kennung aus Ihrem [!DNL Commerce] Katalog zur entsprechenden Kennung von Walmart.

Dieser Schritt muss mit [!DNL Commerce] bereits vorhandene Produkte [!DNL Walmart] Listen und zum Synchronisieren von Produktdaten zwischen [!DNL Commerce] und [!DNL Walmart]. Die [!DNL Commerce] Das Produkt muss über mindestens ein Produktattribut verfügen, das mit einer der folgenden Produkt-IDs (Product IDs) übereinstimmt, die für [!DNL Walmart].

**Erforderlich [!DNL Walmart] Produkt-IDs**

| **Akzeptierter Typ** | **Name** | **Zweck** | **Zulässige Ziffern** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Globaler Handelsartikel | Allgemeiner Verwendungszweck weltweit | 14 Stellen |
| ISBN | Internationale Standardbuchnummer | Papiere, Hardcover und elektronische Bücher | 10 oder 13 Stellen |
| ISSN | Internationale Standardseriennummer | 8-stellige Seriennummer zur Identifizierung von Zeitschriften, Zeitschriften, Zeitungen und Zeitschriften aller Art, die auf allen gedruckten Medien und auf elektronischem Wege zugestellt werden | 8 Stellen |
| UPC | Universeller Produktcode | Standard-Tracking-Code für den Einzelhandel | 12 Stellen |

Wenn Ihr Katalog nicht über ein entsprechendes Attribut verfügt, [Hinzufügen oder Konvertieren eines vorhandenen Katalogattributs](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

## Zuordnen eindeutiger Kennungen

1. Aus dem **[!UICONTROL Listings]** oder **[!UICONTROL Orders]** Seite für den Verkaufskanalspeicher auswählen **[!UICONTROL Channel Settings]**.

1. on **[!UICONTROL Channel Settings]** auswählen **[!UICONTROL Map Attributes]**.

   - Suchen Sie die [!DNL Walmart Marketplace] -Attribut zuzuordnen.

   - Wählen Sie das entsprechende Attribut aus der [!DNL Commerce] Store-Katalog.

     Im folgenden Beispiel wird die [!UICONTROL Walmart Marketplace UPC] -Attribut dem UPC-Attribut im Produktkatalog.

     ![Zuordnungsattribute für Produktübereinstimmungskriterien](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"}

   - Auswählen **[!UICONTROL Save]**.
