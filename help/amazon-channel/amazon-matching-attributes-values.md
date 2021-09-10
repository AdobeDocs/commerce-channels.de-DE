---
title: Anzeigen der Amazon-Attributzuordnung
description: Überprüfen Sie die Werte für Ihre verknüpften Commerce-Attribute, um die Commerce- und Amazon-Synchronisation korrekt durchzuführen.
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Anzeigen der Amazon-Attributzuordnung

Wenn Sie Amazon-Attribute [!DNL Commerce]-Attributen zuordnen, verfolgt der Amazon-Vertriebskanal und stellt eine filterbare Liste aller Amazon-Werte bereit. Verwenden Sie diese Seite, um die Werte für die verknüpften [!DNL Commerce]-Attribute zu überprüfen, die korrekt zwischen [!DNL Commerce] und Amazon synchronisiert werden. Sie können die synchronisierten Werte für Amazon-Attribute überprüfen, die mit einem [!DNL Commerce] -Attribut verknüpft sind oder nicht damit verknüpft sind. Informationen zum Erstellen oder Bearbeiten Ihrer Amazon-Attribute finden Sie unter [Erstellen und Bearbeiten von Attributen](./creating-attributes.md).

Der _Amazon-Wert_ unterscheidet sich je nach dem Attributtyp und dem von Ihnen angezeigten Amazon-Attribut. Ein aufgelisteter Amazon-Wert für `Label` wäre beispielsweise ein Textwert, während `AmazonListPrice` ein numerischer Wert wäre. Der Status gibt an, ob der Amazon-Wert importiert wurde.

## Anzeigen Ihrer Attributwerte

1. Navigieren Sie in der Seitenleiste _[!UICONTROL Admin]_zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Klicken Sie im Menü links auf **[!UICONTROL Attributes]**, suchen Sie ein Amazon-Attribut und klicken Sie in der Spalte _[!UICONTROL Action]_entweder auf **[!UICONTROL Create]**oder auf **[!UICONTROL Edit]**.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Matching Attribute Values]** .

   Auflistungen mit dem entsprechenden Katalogprodukt [!DNL Commerce] zeigen einen verknüpften Wert in der Spalte _Magento Product SKU_. Wenn Sie auf einen Link klicken, wird die entsprechende Seite mit den Katalogproduktdetails geöffnet. Änderungen an Amazon-Attributen auf der Produktdetailseite werden nicht wieder mit dem Amazon-Vertriebskanal synchronisiert.

>[!TIP]
>Informationen zum Bearbeiten oder Zuweisen der Zuordnung für eine Liste zu einem Katalogprodukt finden Sie unter [Erforderliche Informationen aktualisieren](./amazon-manually-update-incomplete-listing.md).

![Anzeigen von Attributwerten](assets/amazon-managing-attribute-values.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Region] | Die Region für Verkaufsaktivitäten, die während der Store-Integration in **[!DNL Amazon Marketplace]Land** definiert wurde. |
| [!UICONTROL Magento Product SKU] | Gibt die mit dem Amazon-Store synchronisierten [!DNL Commerce] Produkte an. Der Wert ist eine Produkt-ID, die von [!DNL Commerce] zugewiesen und mit einem Produkt im Katalog verknüpft ist. Um das Produkt in [!DNL Commerce] zu öffnen, klicken Sie auf den Link. |
| [!UICONTROL ASIN] | Gibt die Amazon Standard-Identifikationsnummer (ASIN) an, die dem Produkt von Amazon zur Produktidentifizierung eine 10-stellige alphanumerische eindeutige Kennung zugewiesen hat. |
| [!UICONTROL Amazon Value] | Gibt den Wert für das ausgewählte Attribut an. Der Amazon-Wert unterscheidet sich je nach dem Attributtyp und dem von Ihnen angezeigten Amazon-Attribut. Ein aufgelisteter Amazon-Wert für `Label` wäre beispielsweise ein Textwert, während `AmazonListPrice` ein numerischer Wert wäre. Der Status gibt an, ob der Amazon-Wert importiert wurde. |
| [!UICONTROL Status] | Gibt an, ob die Attributwerte in [!DNL Commerce] importiert und mit einem [!DNL Commerce] -Attribut verknüpft wurden. Optionen: `Not Imported` / `Imported` |
