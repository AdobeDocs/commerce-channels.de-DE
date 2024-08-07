---
title: Erstellen und Zuweisen von Produkten für den Amazon-Vertriebskanal
description: Amazon Sales Channel stellt die Registerkarte [!UICONTROL New Third Party] bereit, mit der Sie übereinstimmende Commerce-Katalogprodukte mit Amazon-Auflistungen erstellen und zuweisen können.
feature: Sales Channels, Products, Configuration
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# Erstellen und Zuweisen von Produkten

Beim Anzeigen der Registerkarte _[!UICONTROL New Third Party]_können Sie Ihre [!DNL Commerce] -Katalogprodukte mit einer vorhandenen Amazon-Liste abgleichen. Für diese Zuordnung gibt es zwei Optionen. Sie können einem vorhandenen Katalogprodukt eine Liste zuweisen oder die Informationen aus der Liste verwenden, um Katalogprodukte zu erstellen. Diese Optionen sind hilfreich, wenn Ihre Amazon-Listen nicht automatisch mit Ihrem [!DNL Commerce] -Katalog übereinstimmen.

Um den gesamten Funktionsumfang des Amazon-Vertriebskanals nutzen zu können, ist es erforderlich, Ihre Produkte Ihren Amazon-Auflistungen zuzuordnen (oder zuzuweisen).

Wenn Sie ein Katalogprodukt aus einer Amazon-Auflistung erstellen:

- Der **ASIN** wird zur [!DNL Commerce] SKU
- Der **Name der Produktliste** wird zum Namen der Katalogliste.
- Die **Preis** und die **Menge** werden aus der Amazon-Liste importiert

Die restlichen erforderlichen Einstellungen werden durch die [!DNL Commerce] -Produkteinstellungen bestimmt, die Sie während der Erstellung auswählen.

Wenn sie erstellt und abgeglichen werden, werden die Auflistungen aus der Registerkarte _[!UICONTROL New Third Party]_entfernt und auf der Registerkarte_[!UICONTROL Active]_ angezeigt.

## Zuweisen eines einzelnen Katalogprodukts zu einer Amazon-Liste

1. Zeigen Sie Ihre Produktlisten auf der Registerkarte [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) an.

1. Suchen Sie die Liste, die Sie zuweisen möchten, klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**und klicken Sie auf **[!UICONTROL Assign Catalog Product]**.

   Durch diese Aktion wird die Seite _[!UICONTROL Assign Magento Catalog Product]_geöffnet.

1. Suchen oder filtern Sie die Liste mithilfe der [Arbeitsbereichssteuerelemente](./workspace-controls.md) und suchen Sie nach dem entsprechenden Katalogprodukt, das mit der Auflistung übereinstimmt.

1. Wenn das richtige Produkt in der Liste angezeigt wird, klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Assign Catalog Product]**.

Ihr Produkt und Ihre Liste wurden nun abgeglichen. Der Amazon-Vertriebskanal kann jetzt Produkt- und Listendaten für Amazon freigeben und Ihre Liste und die zugehörigen Informationen verwalten, einschließlich Listenpreis, Versandpreis, Lager/Menge, Bestellinformationen und -status und mehr.

## Erstellen eines einzelnen Katalogprodukts mit Amazon-Listendaten

1. Zeigen Sie Ihre Produktlisten auf der Registerkarte [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) an.

1. Suchen Sie die Liste, die Sie erstellen möchten, in Ihrem [!DNL Commerce]-Katalog, klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**und klicken Sie auf **[!UICONTROL Create New Catalog Product]**.

   Durch diese Aktion wird die Seite _[!UICONTROL Create Magento Catalog Product]_geöffnet.

1. Füllen Sie die Katalogeinstellungen für das Produkt aus.

   - Setzen Sie den Umschalter **[!UICONTROL Enable Product(s)]** auf `Yes` oder `No` (erforderlich).

     |Ja|Entscheiden Sie, ob Sie das Produkt für Ihren [!DNL Commerce] Store-Umsatz qualifizieren möchten.|
|Nein|Wählen Sie aus, dass das Produkt nicht für Ihre [!DNL Commerce] Storefront-Verkäufe infrage kommt.|

   - Weisen Sie für **[!UICONTROL Categories]** eine Kategorie für das Produkt zu (optional).

     Um die Produktkategorie auszuwählen, klicken Sie auf den Abwärtspfeil und wählen Sie ein Kategorie-Kontrollkästchen aus. Klicken Sie zum Abschluss auf **[!UICONTROL Done]** .

   - Wählen Sie für **[!UICONTROL Website Ids]** die Website (Storefront) aus, der das Produkt zugeordnet werden soll.

     Die Optionen in dieser Liste hängen von Ihren [!DNL Commerce] [Speicherkonfigurationseinstellungen](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) ab.

   - Wählen Sie für **[!UICONTROL Attribute Set Id]** (erforderlich) eine Option aus.

     `Default` ist die Standardauswahl. Die Optionen in dieser Liste hängen von den von Ihnen konfigurierten [!DNL Commerce] [Attributsätzen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) ab.

   - Wählen Sie für **[!UICONTROL Visibility]** eine Option für das neue Produkt aus.

     |**[!UICONTROL Not Visible Individually]** (Standard)|Das Produkt ist nicht in Ihren Storefront-Auflistungen enthalten, obwohl es möglicherweise als Variante eines anderen Produkts verfügbar ist.|
|**[!UICONTROL Catalog]**|Das Produkt wird in Ihren Kataloglisten angezeigt.|
|**[!UICONTROL Search]**|Das Produkt ist für Suchvorgänge verfügbar.|
|**[!UICONTROL Catalog and Search]**|Das Produkt ist in Kataloglisten enthalten und für Suchvorgänge verfügbar.|

   - Wählen Sie für **[!UICONTROL Assign Tax Class]** eine Option für das Produkt aus.

     Die in dieser Liste angezeigten Optionen hängen von den konfigurierten [Steuerklassen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) ab.

   - Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Create Catalog Products]**.

Das Katalogprodukt wird in Ihrem [!DNL Commerce] -Katalog erstellt und der Amazon-Liste zugewiesen, aus der es erstellt wurde. Da die Liste nun mit einer vorhandenen Amazon-Liste übereinstimmt, wird die Liste aus der Registerkarte _[!UICONTROL New Third Party]_entfernt und auf der Registerkarte_[!UICONTROL Active]_ angezeigt.

## Erstellen mehrerer Katalogprodukte mithilfe der Amazon-Listendaten

1. Zeigen Sie Ihre Produktlisten auf der Registerkarte [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) an.

1. Wählen Sie die Listen aus, für die Sie Katalogprodukte erstellen möchten.

   Sie können einzelne Kontrollkästchen in der linken Spalte auswählen oder auf den Pfeil nach unten in der Spalte oben links klicken und **[!UICONTROL Select All]** oder **[!UICONTROL Select All on this Page]** auswählen.

1. Klicken Sie unter _[!UICONTROL Actions]_auf **[!UICONTROL Create New Catalog Product(s)]**.

1. Um die Bestätigungsnachricht zu akzeptieren und die Seite _[!UICONTROL Create Magento Catalog Product]_zu öffnen, klicken Sie auf **[!UICONTROL OK]**.

1. Füllen Sie die Katalogeinstellungen für die Produkte aus.

   >[!NOTE]
   >Beim Erstellen von Katalogprodukten für mehrere ausgewählte Listen werden die eingegebenen Produkteinstellungen auf alle Listen angewendet.

   - Setzen Sie den Umschalter **[!UICONTROL Enable Product(s)]** auf `Yes` oder `No` (erforderlich).

     |Ja|Entscheiden Sie, ob Sie das Produkt für Ihren [!DNL Commerce] Store-Umsatz qualifizieren möchten.|
|Nein|Wählen Sie aus, dass das Produkt nicht für Ihre [!DNL Commerce] Storefront-Verkäufe infrage kommt.|

   - Weisen Sie für **[!UICONTROL Categories]** eine Kategorie für das Produkt zu (optional).

     Um die Produktkategorie auszuwählen, klicken Sie auf den Abwärtspfeil und wählen Sie ein Kategorie-Kontrollkästchen aus. Klicken Sie zum Abschluss auf **Fertig** .

   - Wählen Sie für **[!UICONTROL Website Ids]** die Website (Storefront) aus, der das Produkt zugeordnet werden soll.

     Die Optionen in dieser Liste hängen von Ihren [!DNL Commerce] [Speicherkonfigurationseinstellungen](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) ab.

   - Wählen Sie für **[!UICONTROL Attribute Set Id]** (erforderlich) eine Option aus.

     `Default` ist die Standardauswahl. Die Optionen in dieser Liste hängen von den von Ihnen konfigurierten [!DNL Commerce] [Attributsätzen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) ab.

   - Wählen Sie für **[!UICONTROL Visibility]** eine Option für das neue Produkt aus.

     |**[!UICONTROL Not Visible Individually]** (Standard)|Das Produkt ist nicht in Ihren Storefront-Auflistungen enthalten, obwohl es möglicherweise als Variante eines anderen Produkts verfügbar ist.|
|**[!UICONTROL Catalog]**|Das Produkt wird in Ihren Kataloglisten angezeigt.|
|**[!UICONTROL Search]**|Das Produkt ist für Suchvorgänge verfügbar.|
|**[!UICONTROL Catalog and Search]**|Das Produkt ist in Kataloglisten enthalten und für Suchvorgänge verfügbar.|

   - Wählen Sie für **[!UICONTROL Assign Tax Class]** eine Option für das Produkt aus.

     Die in dieser Liste angezeigten Optionen hängen von den konfigurierten [Steuerklassen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) ab.

   - Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Create Catalog Products]**.

Die Katalogprodukte werden in Ihrem [!DNL Commerce] -Katalog erstellt und der Amazon-Liste zugewiesen, aus der sie erstellt wurden. Da die Auflistungen nun mit der jeweiligen Amazon-Liste übereinstimmen, werden die Auflistungen aus der Registerkarte [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) entfernt und auf der Registerkarte [_[!UICONTROL Active]_](./active-listings.md) angezeigt.

![Commerce-Katalogprodukt erstellen](assets/amazon-magento-catalog-product.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Product(s)] | (Erforderlich) Wenn diese Option aktiviert ist, ist das Produkt in Ihrer [!DNL Commerce] -Storefront sichtbar. Wenn diese Option deaktiviert ist, wird das Produkt nicht in Ihrer [!DNL Commerce] -Storefront angezeigt. |
| [!UICONTROL Categories] | Sie können den Namen der Kategorie für Ihr neues Produkt eingeben oder eine Kategorie auswählen, indem Sie auf den Abwärtspfeil klicken, um Ihre Optionen anzuzeigen. Die Optionen hängen von Ihrer [categories](https://experienceleague.adobe.com/docs/commerce-admin/catalog/categories/create/category-create.html) -Konfiguration ab. |
| [!UICONTROL Website Ids] | (Erforderlich) Wählen Sie die Website (Storefront) aus, der das Produkt zugeordnet werden soll. Die Optionen hängen von Ihren [!DNL Commerce] [Speicherkonfigurationseinstellungen](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) ab |
| Attributset-ID | Wählen Sie einen Attributsatz aus. Die Optionen hängen von den konfigurierten [!DNL Commerce] [Attributsätzen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) ab. |
| [!UICONTROL Visibility] | Optionen:<ul><li>**[!UICONTROL Not Visible Individually]** - Das Produkt ist nicht in Ihrer [!DNL Commerce] Storefront sichtbar (am häufigsten bei Variantenprodukten).</li><li>**[!UICONTROL Catalog]** - Ermöglicht den Zugriff auf das Produkt über die Kategorie, mit der es auf der Website verknüpft ist.</li><li>**Suche** - Ermöglicht, dass das Produkt nur über das Suchwerkzeug gefunden wird.</li><li>**[!UICONTROL Catalog and Search]** - Ermöglicht den Zugriff auf die Produkte über die Kategoriestruktur und das Suchwerkzeug.</li></ul> |
| [!UICONTROL Assign Tax Class] | Weisen Sie dem neuen Produkt eine Steuerklasse zu. Die Optionen hängen von den konfigurierten [Steuerklassen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) ab. |
