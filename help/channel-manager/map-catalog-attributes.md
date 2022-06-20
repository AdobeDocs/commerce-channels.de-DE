---
title: Katalogattribute zuordnen
description: Zuordnen von Attributen zum Abgleich [DNL! Commerce-] Produkte in bestehende [!DNL Walmart Marketplace] Auflistungen und Synchronisieren von Daten zwischen [!DNL Channel Manager] und [!DNL Walmart].
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 97128dcf45d7672e958c771f88389aba40c6e39e
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Katalogattribute zuordnen

Vor der Verbindung von Listen aus [!DNL Commerce] nach [!DNL Walmart Marketplace]müssen Sie mindestens eine eindeutige Kennung aus Ihrem [!DNL Commerce] Katalog zur entsprechenden Kennung von Walmart.

Dieser Schritt muss mit [!DNL Commerce] bereits [!DNL Walmart] Auflistungen und zum Synchronisieren von Produktdaten zwischen [!DNL Commerce] und [!DNL Walmart]. Die [!DNL Commerce] Das Produkt muss über mindestens ein Produktattribut verfügen, das mit einer der folgenden Produkt-IDs (Product IDs) übereinstimmt, die für [!DNL Walmart].

**Erforderlich [!DNL Walmart] Produkt-IDs**

| **Akzeptierter Typ** | **Name** | **Zweck** | **Zulässige Ziffern** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Globaler Handelsartikel | Allgemeine Verwendung weltweit | 14 Stellen |
| ISBN | Internationale Standardbuchnummer | Papiere, Hardcover und elektronische Bücher | 10 oder 13 Stellen |
| ISSN | Internationale Standardseriennummer | 8-stellige Seriennummer zur Identifizierung von Zeitschriften, Zeitschriften, Zeitungen und Zeitschriften aller Art, die auf allen gedruckten Medien und auf elektronischem Wege zugestellt werden | 8 Stellen |
| UPC | Universeller Produktcode | Standard-Tracking-Code für den Einzelhandel | 12 Stellen |

Wenn Ihr Katalog nicht über ein entsprechendes Attribut verfügt, [Hinzufügen oder Konvertieren eines vorhandenen Katalogattributs](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## Zuordnen eindeutiger Kennungen

1. Aus dem **[!UICONTROL Listings]** oder **[!UICONTROL Orders]** Seite für den Verkaufskanalspeicher auswählen **[!UICONTROL Channel Settings]**.

1. on **[!UICONTROL Channel Settings]** auswählen **[!UICONTROL Shipping Carriers]**.

   - Suchen Sie die [!DNL Walmart Marketplace] -Attribut zuzuordnen.

   - Wählen Sie das entsprechende Attribut aus der [!DNL Commerce] Katalog speichern.

      Im folgenden Beispiel wird die [!UICONTROL Walmart Marketplace UPC] -Attribut dem UPC-Attribut im Produktkatalog.
   ![Zuordnungsattribute für Produktübereinstimmungskriterien](assets/products-map-attributes-for-match.png)

   - Auswählen **[!UICONTROL Save]**.


