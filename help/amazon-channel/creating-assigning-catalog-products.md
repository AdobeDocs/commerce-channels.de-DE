---
title: Produkte erstellen und zuweisen
description: Amazon Sales Channel bietet [!UICONTROL New Third Party] , um die Erstellung und Zuweisung passender Commerce-Katalogprodukte mit Amazon-Auflistungen zu erleichtern.
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Produkte erstellen und zuweisen

Bei Ansicht _[!UICONTROL New Third Party]_, können Sie [!DNL Commerce] Produkte in eine bestehende Amazon-Liste zu katalogisieren. Für diese Übereinstimmung gibt es zwei Optionen. Sie können einem vorhandenen Katalogprodukt eine Liste zuweisen oder die Informationen aus der Liste zum Erstellen von Katalogprodukten verwenden. Diese Optionen sind hilfreich, wenn Ihre Amazon-Auflistungen nicht automatisch Ihren [!DNL Commerce] Katalog.

Um den vollen Funktionsumfang von Amazon Sales Kanal nutzen zu können, müssen Sie Ihre Produkte Ihren Amazon-Listen zuordnen (oder zuordnen).

Wenn Sie ein Katalogprodukt aus einer Amazon-Auflistung erstellen:

- Die **ASIN** wird [!DNL Commerce] SKU
- Die **Produktlistenname** wird der Name der Katalogliste
- Die **Preis** und **Menge** aus der Amazon-Liste importiert werden

Die übrigen notwendigen Einstellungen werden von der [!DNL Commerce] Produkteinstellungen, die Sie während der Erstellung auswählen.

Wenn erstellt und abgeglichen, werden die Auflistungen aus dem _[!UICONTROL New Third Party]_und erscheinen auf_[!UICONTROL Active]_ Tabulator.

## Zuweisen eines einzelnen Katalogprodukts zu einer Amazon-Liste

1. Ansicht der Produktauflistungen auf der [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) Tabulator.

1. Suchen Sie die Liste, die Sie in der Liste zuweisen möchten, und klicken Sie auf **[!UICONTROL Select]** in _[!UICONTROL Action]_und klicken Sie auf **[!UICONTROL Assign Catalog Product]**.

   Diese Aktion öffnet die _[!UICONTROL Assign Magento Catalog Product]_Seite.

1. Liste suchen oder filtern mit [Arbeitsbereichssteuerelemente](./workspace-controls.md) und suchen Sie das passende Katalogprodukt, das der Liste entspricht.

1. Wenn das richtige Produkt in der Liste angezeigt wird, klicken Sie auf **[!UICONTROL Assign Catalog Product]** in _[!UICONTROL Action]_Spalte.

Ihr Produkt und Ihre Auflistung sind nun übereinstimmen. Amazon Sales Kanal kann nun Produkt- und Listendaten für Amazon freigeben und Ihre Auflistung und die zugehörigen Informationen verwalten, einschließlich Listenpreis, Versandpreis, Lagerbestand/Menge, Bestellinformationen und Status und vieles mehr.

## Ein einzelnes Katalogprodukt mit den Amazon-Listungsinformationen erstellen

1. Ansicht der Produktauflistungen auf der [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) Tabulator.

1. Suchen Sie die Liste, die Sie in Ihrem [!DNL Commerce] Katalog, klicken Sie **[!UICONTROL Select]** in _[!UICONTROL Action]_und klicken Sie auf **[!UICONTROL Create New Catalog Product]**.

   Diese Aktion öffnet die _[!UICONTROL Create Magento Catalog Product]_Seite.

1. Füllen Sie die Katalogeinstellungen für das Produkt aus.

   - Festlegen **[!UICONTROL Enable Product(s)]** umschalten auf `Yes` oder `No` (erforderlich).

      |Ja|Wählen Sie aus, ob das Produkt für Ihre [!DNL Commerce] Schaufensterverkauf.| |Nein|Wählen Sie aus, ob das Produkt nicht für Ihre [!DNL Commerce] Ladengeschäft.|

   - für **[!UICONTROL Categories]**, eine Kategorie für das Produkt zuweisen (optional).

      Um die Kategorie des Produkts auszuwählen, klicken Sie auf den Pfeil nach unten und wählen Sie ein Kontrollkästchen Kategorie. Klick **[!UICONTROL Done]** wenn fertig.

   - für **[!UICONTROL Website Ids]**, wählen Sie die Website (Schaufenster), für die das Produkt zugeordnet werden soll.

      Die Optionen in dieser Liste hängen von Ihren [!DNL Commerce] [Speicherkonfiguration](https://docs.magento.com/user-guide/stores/websites-stores-views.html)Einstellungen für {Zielgruppe=&quot;_blank&quot;}.

   - für **[!UICONTROL Attribute Set Id]** (erforderlich), wählen Sie eine Option aus.

      `Default` ist die Standardauswahl. Die Optionen in dieser Liste hängen von Ihren [!DNL Commerce] [Attributsätze](https://docs.magento.com/user-guide/stores/attribute-sets.html)Sie haben {Zielgruppe=&quot;_blank&quot;} konfiguriert.

   - für **[!UICONTROL Visibility]**, wählen Sie eine Option für das neue Produkt aus.

      |**[!UICONTROL Not Visible Individually]** (Standard)|Das Produkt ist nicht in Ihren Schaufensterauflistungen enthalten, obwohl es als Variante eines anderen Produkts erhältlich sein kann.| |**[!UICONTROL Catalog]**|Das Produkt wird in Ihren Katalogeinträgen angezeigt.| |**[!UICONTROL Search]**|Das Produkt ist für Suchvorgänge verfügbar.| |**[!UICONTROL Catalog and Search]**| Das Produkt ist in Kataloglisten enthalten und für Suchvorgänge verfügbar.|

   - für **[!UICONTROL Assign Tax Class]**, wählen Sie eine Option für das Produkt aus.

      Die Optionen, die in dieser Liste angezeigt werden, hängen von der [Steuerklassen](https://docs.magento.com/user-guide/tax/tax-class.html)Sie haben {Zielgruppe=&quot;_blank&quot;} konfiguriert.

   - Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Create Catalog Products]**.

Das Katalogprodukt wird in Ihrer [!DNL Commerce] Katalog und der Amazon-Liste zugewiesen, aus der sie erstellt wurde. Da die Auflistung nun einer vorhandenen Amazon-Auflistung zugeordnet ist, wird die Liste aus der Liste gelöscht _[!UICONTROL New Third Party]_und erscheinen im_[!UICONTROL Active]_ Tabulator.

## Mehrere Katalogprodukte mithilfe der Amazon-Listeinformationen erstellen

1. Ansicht der Produktauflistungen auf der [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) Tabulator.

1. Wählen Sie die Einträge aus, für die Katalogprodukte erstellt werden sollen.

   Sie können einzelne Kontrollkästchen in der linken Spalte auswählen oder auf den Pfeil nach unten in der linken oberen Spalte klicken und die Option **[!UICONTROL Select All]** oder **[!UICONTROL Select All on this Page]**.

1. Unter _[!UICONTROL Actions]_, klicken **[!UICONTROL Create New Catalog Product(s)]**.

1. So akzeptieren Sie die Bestätigungsmeldung und öffnen die _[!UICONTROL Create Magento Catalog Product]_Seite, klicken **[!UICONTROL OK]**.

1. Füllen Sie die Katalogeinstellungen für die Produkte aus.

   >[!NOTE]
   >Beim Erstellen von Katalogprodukten für mehrere ausgewählte Auflistungen werden die eingegebenen Produkteinstellungen auf alle Auflistungen angewendet.

   - Festlegen **[!UICONTROL Enable Product(s)]** umschalten auf `Yes` oder `No` (erforderlich).

      |Ja|Wählen Sie aus, ob das Produkt für Ihre [!DNL Commerce] Schaufensterverkauf.| |Nein|Wählen Sie aus, ob das Produkt nicht für Ihre [!DNL Commerce] Ladengeschäft.|

   - für **[!UICONTROL Categories]**, eine Kategorie für das Produkt zuweisen (optional).

      Um die Kategorie des Produkts auszuwählen, klicken Sie auf den Pfeil nach unten und wählen Sie ein Kontrollkästchen Kategorie. Klick **Fertig** wenn fertig.

   - für **[!UICONTROL Website Ids]**, wählen Sie die Website (Schaufenster), für die das Produkt zugeordnet werden soll.

      Die Optionen in dieser Liste hängen von Ihren [!DNL Commerce] [Speicherkonfiguration](https://docs.magento.com/user-guide/stores/websites-stores-views.html)Einstellungen für {Zielgruppe=&quot;_blank&quot;}.

   - für **[!UICONTROL Attribute Set Id]** (erforderlich), wählen Sie eine Option aus.

      `Default` ist die Standardauswahl. Die Optionen in dieser Liste hängen von Ihren [!DNL Commerce] [Attributsätze](https://docs.magento.com/user-guide/stores/attribute-sets.html)Sie haben {Zielgruppe=&quot;_blank&quot;} konfiguriert.

   - für **[!UICONTROL Visibility]**, wählen Sie eine Option für das neue Produkt aus.

      |**[!UICONTROL Not Visible Individually]** (Standard)|Das Produkt ist nicht in Ihren Schaufensterauflistungen enthalten, obwohl es als Variante eines anderen Produkts erhältlich sein kann.| |**[!UICONTROL Catalog]**|Das Produkt wird in Ihren Katalogeinträgen angezeigt.| |**[!UICONTROL Search]**|Das Produkt ist für Suchvorgänge verfügbar.| |**[!UICONTROL Catalog and Search]**| Das Produkt ist in Kataloglisten enthalten und für Suchvorgänge verfügbar.|

   - für **[!UICONTROL Assign Tax Class]**, wählen Sie eine Option für das Produkt aus.

      Die Optionen, die in dieser Liste angezeigt werden, hängen von der [Steuerklassen](https://docs.magento.com/user-guide/tax/tax-class.html)Sie haben {Zielgruppe=&quot;_blank&quot;} konfiguriert.

   - Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Create Catalog Products]**.

Die Katalogprodukte werden in Ihrer [!DNL Commerce] Katalog und der Amazon-Liste zugewiesen, aus der sie erstellt wurde. Da die Auflistungen nun mit der jeweiligen Amazon-Auflistung übereinstimmen, werden die Auflistungen aus der Liste gelöscht [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) und erscheinen im [_[!UICONTROL Active]_](./active-listings.md) Tabulator.

![Commerce-Katalogprodukt erstellen](assets/amazon-magento-catalog-product.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Enable Product(s)] | (Erforderlich) Wenn aktiviert, wird das Produkt in Ihrer [!DNL Commerce] Schaufenster. Wenn deaktiviert, wird das Produkt nicht in Ihrer [!DNL Commerce] Schaufenster. |
| [!UICONTROL Categories] | Sie können den Namen der Kategorie für Ihr neues Produkt eingeben oder eine Kategorie auswählen, indem Sie auf den Pfeil nach unten klicken, um die Optionen anzuzeigen. Die Optionen hängen von Ihren [Kategorien](https://docs.magento.com/user-guide/catalog/category-create.html)Konfiguration von {Zielgruppe=&quot;_blank&quot;}. |
| [!UICONTROL Website Ids] | (Erforderlich) Wählen Sie die Website (Schaufenster) aus, der das Produkt zugeordnet werden soll. Die Optionen hängen von Ihren [!DNL Commerce] [Speicherkonfiguration](https://docs.magento.com/user-guide/stores/websites-stores-views.html)Einstellungen für {Zielgruppe=&quot;_blank&quot;} |
| Attributset-ID | Wählen Sie einen Attributsatz aus. Die Optionen hängen von der konfigurierten ab. [!DNL Commerce] [Attributsätze](https://docs.magento.com/user-guide/stores/attribute-sets.html){Zielgruppe=&quot;_blank&quot;}. |
| [!UICONTROL Visibility] | Optionen:<ul><li>**[!UICONTROL Not Visible Individually]** - Das Produkt ist in Ihrer [!DNL Commerce] Schaufenster (am häufigsten bei Variantenprodukten).</li><li>**[!UICONTROL Catalog]** - Ermöglicht den Zugriff auf das Produkt über die Kategorie, mit der es innerhalb der Website verbunden ist.</li><li>**Suchen** - Ermöglicht es, das Produkt nur über das Suchwerkzeug zu finden.</li><li>**[!UICONTROL Catalog and Search]** - Ermöglicht den Zugriff auf die Produkte über die Kategorie und über das Suchwerkzeug.</li></ul> |
| [!UICONTROL Assign Tax Class] | Weisen Sie dem neuen Produkt eine Steuerklasse zu. Die Optionen hängen von der konfigurierten ab. [Steuerklassen](https://docs.magento.com/user-guide/tax/tax-class.html){Zielgruppe=&quot;_blank&quot;}. |
