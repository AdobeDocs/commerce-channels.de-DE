---
title: Erstellen und Zuweisen von Produkten für den Amazon-Vertriebskanal
description: Amazon Sales Channel stellt die [!UICONTROL New Third Party] -Tab, um die Erstellung und Zuweisung von entsprechenden Commerce-Katalogprodukten zu Amazon-Auflistungen zu erleichtern.
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 077d680da3c98ef9a48958eb548a9d5c1612f74e
workflow-type: tm+mt
source-wordcount: '1094'
ht-degree: 0%

---

# Erstellen und Zuweisen von Produkten

Beim Anzeigen _[!UICONTROL New Third Party]_-Registerkarte, können Sie Ihre [!DNL Commerce] -Produkte in eine bestehende Amazon-Liste zu katalogisieren. Für diese Zuordnung gibt es zwei Optionen. Sie können einem vorhandenen Katalogprodukt eine Liste zuweisen oder die Informationen aus der Liste verwenden, um Katalogprodukte zu erstellen. Diese Optionen sind hilfreich, wenn Ihre Amazon-Listen nicht automatisch mit Ihren [!DNL Commerce] Katalog.

Um den gesamten Funktionsumfang des Amazon-Vertriebskanals nutzen zu können, ist es erforderlich, Ihre Produkte Ihren Amazon-Auflistungen zuzuordnen (oder zuzuweisen).

Wenn Sie ein Katalogprodukt aus einer Amazon-Auflistung erstellen:

- Die **ASIN** wird [!DNL Commerce] SKU
- Die **Name der Produktliste** wird zum Kataloglistennamen
- Die **Preis** und **Menge** aus der Amazon-Liste importiert werden

Die übrigen erforderlichen Einstellungen werden durch die Variable [!DNL Commerce] Produkteinstellungen, die Sie während der Erstellung auswählen.

Bei der Erstellung und Übereinstimmung werden die Listen aus der _[!UICONTROL New Third Party]_und werden auf der Registerkarte_[!UICONTROL Active]_ Registerkarte.

## Zuweisen eines einzelnen Katalogprodukts zu einer Amazon-Liste

1. Anzeigen Ihrer Produktlisten auf der [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) Registerkarte.

1. Suchen Sie die Liste, die Sie zuweisen möchten, und klicken Sie auf **[!UICONTROL Select]** im _[!UICONTROL Action]_und klicken Sie auf **[!UICONTROL Assign Catalog Product]**.

   Diese Aktion öffnet die _[!UICONTROL Assign Magento Catalog Product]_Seite.

1. Suchen oder filtern Sie die Liste mithilfe der [Arbeitsbereichssteuerelemente](./workspace-controls.md) und suchen Sie das passende Katalogprodukt, das mit der Auflistung übereinstimmt.

1. Wenn das richtige Produkt in der Liste angezeigt wird, klicken Sie auf **[!UICONTROL Assign Catalog Product]** im _[!UICONTROL Action]_Spalte.

Ihr Produkt und Ihre Liste wurden nun abgeglichen. Der Amazon-Vertriebskanal kann jetzt Produkt- und Listendaten für Amazon freigeben und Ihre Liste und die zugehörigen Informationen verwalten, einschließlich Listenpreis, Versandpreis, Lager/Menge, Bestellinformationen und -status und mehr.

## Erstellen eines einzelnen Katalogprodukts mit Amazon-Listendaten

1. Anzeigen Ihrer Produktlisten auf der [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) Registerkarte.

1. Suchen Sie die Liste, die Sie erstellen möchten, in Ihrer [!DNL Commerce] Katalog, klicken **[!UICONTROL Select]** im _[!UICONTROL Action]_und klicken Sie auf **[!UICONTROL Create New Catalog Product]**.

   Diese Aktion öffnet die _[!UICONTROL Create Magento Catalog Product]_Seite.

1. Füllen Sie die Katalogeinstellungen für das Produkt aus.

   - Satz **[!UICONTROL Enable Product(s)]** Umschalten auf `Yes` oder `No` (erforderlich).

      |Ja|Wählen Sie aus, das Produkt für Ihre [!DNL Commerce] Storefront-Verkäufe.| |Nein|Wählen Sie aus, ob das Produkt für Ihre [!DNL Commerce] Storefront-Verkäufe.|

   - Für **[!UICONTROL Categories]**, eine Kategorie für das Produkt zuweisen (optional).

      Um die Produktkategorie auszuwählen, klicken Sie auf den Abwärtspfeil und wählen Sie ein Kategorie-Kontrollkästchen aus. Klicken **[!UICONTROL Done]** wenn fertig.

   - Für **[!UICONTROL Website Ids]**, wählen Sie die Website (Storefront) aus, der das Produkt zugeordnet werden soll.

      Die Optionen in dieser Liste hängen von Ihrer [!DNL Commerce] [Store-Konfiguration](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) -Einstellungen.

   - Für **[!UICONTROL Attribute Set Id]** (erforderlich), wählen Sie eine Option aus.

      `Default` ist die Standardauswahl. Die Optionen in dieser Liste hängen von Ihrer [!DNL Commerce] [Attributsätze](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) Sie haben konfiguriert.

   - Für **[!UICONTROL Visibility]**, wählen Sie eine Option für das neue Produkt aus.

      |**[!UICONTROL Not Visible Individually]** (Standard)|Das Produkt ist nicht in Ihren Storefront-Listen enthalten, obwohl es als Variante eines anderen Produkts verfügbar sein kann.| |**[!UICONTROL Catalog]**|Das Produkt wird in Ihren Kataloglisten angezeigt.| |**[!UICONTROL Search]**|Das Produkt ist für Suchvorgänge verfügbar.| |**[!UICONTROL Catalog and Search]**|Das Produkt ist in Kataloglisten enthalten und für Suchvorgänge verfügbar.|

   - Für **[!UICONTROL Assign Tax Class]**, wählen Sie eine Option für das Produkt aus.

      Die in dieser Liste angezeigten Optionen hängen von der [Steuerklassen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) Sie haben konfiguriert.

   - Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Create Catalog Products]**.

Das Katalogprodukt wird in Ihrer [!DNL Commerce] und der Amazon-Liste zugewiesen, aus der sie erstellt wurde. Da die Liste nun mit einer vorhandenen Amazon-Liste übereinstimmt, wird die Liste aus dem _[!UICONTROL New Third Party]_und in der_[!UICONTROL Active]_ Registerkarte.

## Erstellen mehrerer Katalogprodukte mithilfe der Amazon-Listendaten

1. Anzeigen Ihrer Produktlisten auf der [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) Registerkarte.

1. Wählen Sie die Listen aus, für die Sie Katalogprodukte erstellen möchten.

   Sie können einzelne Kontrollkästchen in der linken Spalte auswählen oder auf den Abwärtspfeil in der Spalte oben links klicken und die Option **[!UICONTROL Select All]** oder **[!UICONTROL Select All on this Page]**.

1. under _[!UICONTROL Actions]_klicken **[!UICONTROL Create New Catalog Product(s)]**.

1. Um die Bestätigungsnachricht zu akzeptieren, öffnen Sie die _[!UICONTROL Create Magento Catalog Product]_Seite, klicken Sie auf **[!UICONTROL OK]**.

1. Füllen Sie die Katalogeinstellungen für die Produkte aus.

   >[!NOTE]
   >Beim Erstellen von Katalogprodukten für mehrere ausgewählte Listen werden die eingegebenen Produkteinstellungen auf alle Listen angewendet.

   - Satz **[!UICONTROL Enable Product(s)]** Umschalten auf `Yes` oder `No` (erforderlich).

      |Ja|Wählen Sie aus, das Produkt für Ihre [!DNL Commerce] Storefront-Verkäufe.| |Nein|Wählen Sie aus, ob das Produkt für Ihre [!DNL Commerce] Storefront-Verkäufe.|

   - Für **[!UICONTROL Categories]**, eine Kategorie für das Produkt zuweisen (optional).

      Um die Produktkategorie auszuwählen, klicken Sie auf den Abwärtspfeil und wählen Sie ein Kategorie-Kontrollkästchen aus. Klicken **Fertig** wenn fertig.

   - Für **[!UICONTROL Website Ids]**, wählen Sie die Website (Storefront) aus, der das Produkt zugeordnet werden soll.

      Die Optionen in dieser Liste hängen von Ihrer [!DNL Commerce] [Store-Konfiguration](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) -Einstellungen.

   - Für **[!UICONTROL Attribute Set Id]** (erforderlich), wählen Sie eine Option aus.

      `Default` ist die Standardauswahl. Die Optionen in dieser Liste hängen von Ihrer [!DNL Commerce] [Attributsätze](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) Sie haben konfiguriert.

   - Für **[!UICONTROL Visibility]**, wählen Sie eine Option für das neue Produkt aus.

      |**[!UICONTROL Not Visible Individually]** (Standard)|Das Produkt ist nicht in Ihren Storefront-Listen enthalten, obwohl es als Variante eines anderen Produkts verfügbar sein kann.| |**[!UICONTROL Catalog]**|Das Produkt wird in Ihren Kataloglisten angezeigt.| |**[!UICONTROL Search]**|Das Produkt ist für Suchvorgänge verfügbar.| |**[!UICONTROL Catalog and Search]**|Das Produkt ist in Kataloglisten enthalten und für Suchvorgänge verfügbar.|

   - Für **[!UICONTROL Assign Tax Class]**, wählen Sie eine Option für das Produkt aus.

      Die in dieser Liste angezeigten Optionen hängen von der [Steuerklassen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) Sie haben konfiguriert.

   - Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Create Catalog Products]**.

Die Katalogprodukte werden in Ihrer [!DNL Commerce] und der Amazon-Liste zugewiesen, aus der sie erstellt wurde. Da die Auflistungen nun mit der entsprechenden Amazon-Auflistung übereinstimmen, werden die Auflistungen aus dem [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) und in der [_[!UICONTROL Active]_](./active-listings.md) Registerkarte.

![Commerce-Katalogprodukt erstellen](assets/amazon-magento-catalog-product.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Enable Product(s)] | (Erforderlich) Wenn diese Option aktiviert ist, ist das Produkt in Ihrer [!DNL Commerce] Storefront. Wenn diese Option deaktiviert ist, wird das Produkt nicht in Ihrer [!DNL Commerce] Storefront. |
| [!UICONTROL Categories] | Sie können den Namen der Kategorie für Ihr neues Produkt eingeben oder eine Kategorie auswählen, indem Sie auf den Abwärtspfeil klicken, um Ihre Optionen anzuzeigen. Die Optionen hängen von Ihrer [categories](https://experienceleague.adobe.com/docs/commerce-admin/catalog/categories/create/category-create.html) Konfiguration. |
| [!UICONTROL Website Ids] | (Erforderlich) Wählen Sie die Website (Storefront) aus, der das Produkt zugeordnet werden soll. Die Optionen hängen von Ihrer [!DNL Commerce] [Store-Konfiguration](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) settings |
| Attributset-ID | Wählen Sie einen Attributsatz aus. Die Optionen hängen von Ihrer Konfiguration ab [!DNL Commerce] [Attributsätze](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html). |
| [!UICONTROL Visibility] | Optionen:<ul><li>**[!UICONTROL Not Visible Individually]** - Das Produkt ist in der [!DNL Commerce] Storefront (am häufigsten bei Variantenprodukten).</li><li>**[!UICONTROL Catalog]** - Ermöglicht den Zugriff auf das Produkt über die Kategorie, mit der es auf der Website verknüpft ist.</li><li>**Suche** - Ermöglicht es, das Produkt nur über das Suchwerkzeug zu finden.</li><li>**[!UICONTROL Catalog and Search]** - Ermöglicht den Zugriff auf die Produkte über die Kategoriestruktur und das Suchwerkzeug.</li></ul> |
| [!UICONTROL Assign Tax Class] | Weisen Sie dem neuen Produkt eine Steuerklasse zu. Die Optionen hängen von Ihrer Konfiguration ab [Steuerklassen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html). |
