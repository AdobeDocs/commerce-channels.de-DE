---
title: Katalogattribute zuordnen
description: '''Zuordnen von Attributen zum Abgleich [DNL! Commerce]-Produkte in bestehende [!DNL Walmart Marketplace] Auflistungen aufnehmen und Daten zwischen [!DNL Channel Manager] und [!DNL Walmart] synchronisieren.'
feature: Sales Channels, Merchandising, Products
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Katalogattribute zuordnen

Bevor Sie Auflistungen von [!DNL Commerce] zu [!DNL Walmart Marketplace] verbinden, müssen Sie mindestens eine eindeutige Kennung aus Ihrem [!DNL Commerce]-Katalog der entsprechenden Kennung von Walmart zuordnen.

Dieser Schritt ist erforderlich, um [!DNL Commerce] -Produkte mit vorhandenen [!DNL Walmart] -Listen abzugleichen und die Produktdaten zwischen [!DNL Commerce] und [!DNL Walmart] zu synchronisieren. Das Produkt [!DNL Commerce] muss über mindestens ein Produktattribut verfügen, das mit einer der folgenden Produkt-IDs (Produkt-IDs) übereinstimmt, die für [!DNL Walmart] erforderlich sind.

**Erforderliche [!DNL Walmart] Produkt-IDs**

| **Akzeptierter Typ** | **Name** | **Zweck** | **Zulässige Ziffern** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | Globaler Handelsartikel | Allgemeiner Verwendungszweck weltweit | 14 Stellen |
| ISBN | Internationale Standardbuchnummer | Papiere, Hardcover und elektronische Bücher | 10 oder 13 Stellen |
| ISSN | Internationale Standardseriennummer | 8-stellige Seriennummer zur Identifizierung von Zeitschriften, Zeitschriften, Zeitungen und Zeitschriften aller Art, die auf allen gedruckten Medien und auf elektronischem Wege zugestellt werden | 8 Stellen |
| UPC | Universeller Produktcode | Standard-Tracking-Code für den Einzelhandel | 12 Stellen |

Wenn Ihr Katalog nicht über ein entsprechendes Attribut verfügt, fügen Sie [ein vorhandenes Katalogattribut hinzu oder konvertieren Sie es.](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)

## Zuordnen eindeutiger Kennungen

1. Wählen Sie auf der Seite **[!UICONTROL Listings]** oder **[!UICONTROL Orders]** für den Verkaufskanalspeicher die Option **[!UICONTROL Channel Settings]** aus.

1. Wählen Sie auf **[!UICONTROL Channel Settings]** **[!UICONTROL Map Attributes]** aus.

   - Suchen Sie das zuzuordnende [!DNL Walmart Marketplace] -Attribut.

   - Wählen Sie das entsprechende Attribut aus dem [!DNL Commerce] Store-Katalog aus.

     Im folgenden Beispiel wird das Attribut [!UICONTROL Walmart Marketplace UPC] dem Attribut UPC im Produktkatalog zugeordnet.

     ![Zuordnen von Attributen für Produktübereinstimmungskriterien](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"}

   - Wählen Sie **[!UICONTROL Save]** aus.
