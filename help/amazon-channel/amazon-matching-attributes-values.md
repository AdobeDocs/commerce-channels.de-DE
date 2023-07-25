---
title: Anzeigen der Amazon-Attributzuordnung
description: Überprüfen Sie die Werte für Ihre verknüpften Commerce-Attribute, um die Commerce- und Amazon-Synchronisation korrekt durchzuführen.
feature: Sales Channels, Products, Configuration
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Anzeigen der Amazon-Attributzuordnung

Beim Zuordnen von Amazon-Attributen zu [!DNL Commerce] -Attributen, verfolgt der Amazon-Vertriebskanal und bietet eine filterbare Liste aller Amazon-Werte. Verwenden Sie diese Seite, um die Werte für Ihre verknüpfte [!DNL Commerce] werden Attribute korrekt synchronisiert [!DNL Commerce] und Amazon. Sie können die synchronisierten Werte für Amazon-Attribute überprüfen, die mit einer [!DNL Commerce] -Attribut. Informationen zum Erstellen oder Bearbeiten Ihrer Amazon-Attribute finden Sie unter [Erstellen und Bearbeiten von Attributen](./creating-attributes.md).

Die _Amazon-Wert_ unterscheidet sich je nach dem angezeigten Attributtyp und dem angezeigten Amazon-Attribut. Beispielsweise einen aufgelisteten Amazon-Wert für `Label` wäre ein Textwert, während `AmazonListPrice` wäre ein numerischer Betrag. Der Status gibt an, ob der Amazon-Wert importiert wurde.

## Anzeigen Ihrer Attributwerte

1. Im _[!UICONTROL Admin]_Seitenleiste, navigieren Sie zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Klicken **[!UICONTROL Attributes]** Suchen Sie im Menü auf der linken Seite nach einem Amazon-Attribut und klicken Sie auf **[!UICONTROL Create]** oder **[!UICONTROL Edit]** im _[!UICONTROL Action]_Spalte.

1. Klicken Sie auf **[!UICONTROL Matching Attribute Values]** Registerkarte.

   Auflistungen mit einer entsprechenden [!DNL Commerce] Das Katalogprodukt zeigt einen verknüpften Wert im _[!UICONTROL Magento Product SKU]_Spalte. Wenn Sie auf einen Link klicken, wird die entsprechende Seite mit den Katalogproduktdetails geöffnet. Änderungen an Amazon-Attributen auf der Produktdetailseite werden nicht wieder mit dem Amazon-Vertriebskanal synchronisiert.

>[!TIP]
>Informationen zum Bearbeiten oder Zuweisen der Zuordnung für eine Liste zu einem Katalogprodukt finden Sie unter [Erforderliche Informationen aktualisieren](./amazon-manually-update-incomplete-listing.md).

![Anzeigen von Attributwerten](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Region] | Die Region, in der die Verkaufsaktivitäten definiert werden in **[!DNL Amazon Marketplace]Land** während der Store-Integration. |
| [!UICONTROL Magento Product SKU] | Gibt die [!DNL Commerce] mit dem Amazon Store synchronisierte Produkte. Der Wert ist eine Produkt-ID, die von [!DNL Commerce] und mit einem Produkt im Katalog verknüpft. So öffnen Sie das Produkt in [!DNL Commerce]klicken Sie auf den Link. |
| [!UICONTROL ASIN] | Gibt die Amazon Standard-Identifikationsnummer (ASIN) an, die dem Produkt von Amazon zur Produktidentifizierung eine 10-stellige alphanumerische eindeutige Kennung zugewiesen hat. |
| [!UICONTROL Amazon Value] | Gibt den Wert für das ausgewählte Attribut an. Der Amazon-Wert unterscheidet sich je nach dem Attributtyp und dem Amazon-Attribut, das Sie anzeigen. Beispielsweise einen aufgelisteten Amazon-Wert für `Label` wäre ein Textwert, während `AmazonListPrice` wäre ein numerischer Betrag. Der Status gibt an, ob der Amazon-Wert importiert wurde. |
| [!UICONTROL Status] | Gibt an, ob die Attributwerte in importiert wurden [!DNL Commerce] und mit einer [!DNL Commerce] -Attribut. Optionen: `Not Imported` / `Imported` |
