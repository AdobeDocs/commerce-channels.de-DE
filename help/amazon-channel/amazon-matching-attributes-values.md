---
title: Ansicht Amazon-Attributzuordnung
description: Überprüfen Sie die Werte der verknüpften Commerce-Attribute, um die korrekte Synchronisation zwischen Commerce und Amazon zu gewährleisten.
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Ansicht Amazon-Attributzuordnung

Während der Zuordnung von Amazon-Attributen zu [!DNL Commerce] Amazon Sales Kanal verfolgt und bietet eine filtrierbare Liste aller Amazon-Werte. Verwenden Sie diese Seite, um die Werte für Ihr verknüpftes Element zu überprüfen [!DNL Commerce] Attribute korrekt synchronisiert zwischen [!DNL Commerce] und Amazon. Sie können synchronisierte Werte für Amazon-Attribut überprüfen, das mit einem [!DNL Commerce] Attribut. Informationen zum Erstellen oder Bearbeiten von Amazon-Attributen finden Sie unter [Erstellen und Bearbeiten von Attributen](./creating-attributes.md).

Die _Amazon-Wert_ variiert je nach Attributtyp und Amazon-Attribut, das Sie Ansicht. Ein gelisteter Amazon-Wert beispielsweise für `Label` wäre ein Textwert während `AmazonListPrice` wäre ein numerischer Betrag. Der Status gibt an, ob der Amazon-Wert importiert wurde.

## Ansicht der Attributwerte

1. Auf _[!UICONTROL Admin]_Sidebar, Gehe zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Klick **[!UICONTROL Attributes]** im Menü auf der linken Seite ein Amazon-Attribut zu suchen, und klicken Sie auf **[!UICONTROL Create]** oder **[!UICONTROL Edit]** in _[!UICONTROL Action]_Spalte.

1. Klicken Sie auf **[!UICONTROL Matching Attribute Values]** Tabulator.

   Auflistungen mit entsprechender [!DNL Commerce] Katalogprodukt einen verknüpften Wert anzeigen in _Magento Product SKU_ Spalte. Wenn Sie auf einen Link klicken, wird die entsprechende Seite mit den Produktdetails des Katalogs geöffnet. Änderungen an Amazon-Attributen auf der Produktdetailseite werden nicht mit Amazon Sales Kanal synchronisiert.

>[!TIP]
>Informationen zum Bearbeiten oder Zuweisen der Zuordnung einer Liste zu einem Katalogprodukt finden Sie unter [Erforderliche Informationen aktualisieren](./amazon-manually-update-incomplete-listing.md).

![Ansicht-Attributwerte](assets/amazon-managing-attribute-values.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Region] | Die Region der Aktivität des Vertriebs **[!DNL Amazon Marketplace]Land** während der Speicherintegration. |
| [!UICONTROL Magento Product SKU] | Kennzeichnet die [!DNL Commerce] mit dem Amazon Store synchronisierte Produkte. Der Wert ist eine Produkt-ID, die von [!DNL Commerce] und mit einem Produkt im Katalog verknüpft. So öffnen Sie das Produkt in [!DNL Commerce], klicken Sie auf den Link. |
| [!UICONTROL ASIN] | Gibt die alphanumerische Amazon-Standardkennung (ASIN) an, die dem Produkt von Amazon zur Produktkennzeichnung zugewiesen wurde. |
| [!UICONTROL Amazon Value] | Gibt den Wert für das ausgewählte Attribut an. Der Amazon-Wert unterscheidet sich je nach Attributtyp und Amazon-Attribut, das Sie Ansicht. Ein gelisteter Amazon-Wert beispielsweise für `Label` wäre ein Textwert während `AmazonListPrice` wäre ein numerischer Betrag. Der Status gibt an, ob der Amazon-Wert importiert wurde. |
| [!UICONTROL Status] | Gibt an, ob die Attributwerte in importiert wurden [!DNL Commerce] und verknüpft mit [!DNL Commerce] Attribut. Optionen: `Not Imported` / `Imported` |
