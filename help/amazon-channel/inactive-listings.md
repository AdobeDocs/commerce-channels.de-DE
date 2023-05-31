---
title: Inaktive Amazon-Listen
description: Der Amazon-Vertriebskanal stellt die [!UICONTROL Inactive] Registerkarte zur Überwachung Ihrer derzeit inaktiven [!DNL Amazon Marketplace] Auflistungen.
exl-id: 1d20e75f-3346-48cb-83f7-a9e7acb26a96
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Inaktive Amazon-Listen

Die _[!UICONTROL Inactive]_-Registerkarte zeigt Ihre Produkte an, die in Amazon veröffentlicht wurden, aber nicht auf der [!DNL Amazon Marketplace]. Ihre Auflistungen können aus verschiedenen Gründen inaktiv sein. Sie sind beispielsweise möglicherweise nicht berechtigt, diese Marke aufzulisten. Inaktive Auflistungen werden durch die Listenstandards von Amazon und Ihre [!DNL Amazon Seller Central] Kontoberechtigungen.

under _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: Wählen Sie aus, ob alle ausgewählten Listen aus dem [!DNL Amazon Marketplace]. Siehe [Beenden einer Amazon-Auflistung](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: Wählen Sie aus, die Einstellungen zum Außerkraftsetzen für die Auflistung zu ändern. Siehe [Überschreibungen](./overrides.md) oder [Bearbeiten oder Entfernen einer Überschreibung](./creating-editing-overrides.md#edit-override-single-listing).

under **[!UICONTROL Select]** im _[!UICONTROL Action]_column:

- **[!UICONTROL View Details]**: Wählen Sie aus, um Details zur Auflistung anzuzeigen, einschließlich der [Auflisten des Aktivitätsprotokolls](./product-listing-details.md#listing-activity-log), [Buy Box Konkurrentenpreise](./product-listing-details.md#buy-box-competitor-pricing)und [Niedrigste Preise für Wettbewerber](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur der Anzeige. In den Listendetails können keine Änderungen vorgenommen werden. Siehe [Details anzeigen](./product-listing-details.md).

- **[!UICONTROL Create Override]**: Wählen Sie aus, eine Überschreibung zu erstellen und sie auf diese Auflistung anzuwenden. Siehe [Erstellen einer Überschreibung](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: Wählen Sie die Änderung des Ihrem Katalogprodukt zugewiesenen ASIN aus. Diese Aktion wird verwendet, wenn ein Produkt in Ihrem Katalog mit dem falschen ASIN abgeglichen wurde. Siehe [Zugewiesenes ASIN bearbeiten](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: Wählen Sie die Erstellung einer Alias-SKU (Stock Keeping Unit), die zum Erstellen einer Amazon-Liste aus demselben Katalogprodukt verwendet werden kann. Siehe [Alias-Verkäufer-SKU erstellen](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: Wählen Sie aus, ob die mit der Bestellung verknüpfte Ausführungsmethode geändert werden soll. Siehe [Einstellungen für &quot;Erfüllt durch&quot;konfigurieren](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: Wählen Sie aus, die Liste aus dem [!DNL Amazon Marketplace]. Siehe [Beenden einer Amazon-Auflistung](./end-listings-manually.md).

>[!NOTE]
>
>Wenn Listen in Bearbeitung sind, wird oberhalb der Registerkarten eine Meldung angezeigt, die die Anzahl der Auflistungen angibt.

![Inaktive Amazon-Listen](assets/amazon-inactive-listings.png){width="600" zoomable="yes"}

Die Startseiten der Amazon-Vertriebskanäle teilen sich einige gemeinsame [Arbeitsbereichssteuerelemente](./workspace-controls.md) die es Ihnen ermöglichen, die angezeigten Daten anzupassen.

| Spalte | Beschreibung |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | Die SKU (Stock Keeping Unit, Bestandseinheit), die von Amazon einem Produkt zugewiesen wurde, um das Produkt, die Optionen, den Preis und den Hersteller zu identifizieren. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die Amazon Standard-Identifikationsnummern. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Erzeugnisses. |
| [!UICONTROL Landed Price] | Der Börsennotierungspreis für das Produkt zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die verfügbare Menge, wenn das Produkt aktiv in Amazon aufgeführt wird. |
| [!UICONTROL Status] | Der von Amazon definierte Status der Auflistung. |
| [!UICONTROL Inactive Reason (if provided by Amazon)] | Amazon bietet nicht immer einen Grund für inaktive Auflistungen und Sie können sich an den Support wenden, um Probleme mit der Auflistung zu beheben. In einigen Fällen benachrichtigt Sie Amazon über einen Grund. Um diese Antworten anzuzeigen, klicken Sie auf **[!UICONTROL View Details]** im _[!UICONTROL Action]_Spalte. Wenn diese Probleme behoben sind und Amazon den Fehler entfernt, werden die Produkte zum_[!UICONTROL Active]_ Registerkarte. |
| Aktion | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie auf **[!UICONTROL Select]** im _[!UICONTROL Action]_und wählen Sie die Option aus:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[[!UICONTROL Create Override]](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
