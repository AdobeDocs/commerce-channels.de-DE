---
title: Verwalten von Amazon-Produktlisten nach Status/Tab
description: Bei der Verwaltung Ihrer Amazon-Listen können Sie je nach Status Aktionen auf Ihre Listen anwenden.
feature: Sales Channels, Products
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Verwalten von Amazon-Produktlisten nach Status/Tab

Die Seite &quot;_[!UICONTROL Product Listings]_&quot; enthält mehrere Registerkarten, über die Sie die Status aller Ihrer Auflistungen anzeigen und Ihre Produkte mit Amazon-Auflistungen abgleichen können.

Die verfügbaren Auflistungsaufgaben unterscheiden sich auf jeder Registerkarte geringfügig, aber die [Arbeitsbereichssteuerelemente](./workspace-controls.md) sind identisch und ermöglichen es Ihnen, die für Ihre Auflistungen angezeigten Daten anzupassen.

Optionen unter **[!UICONTROL Actions]** können die Aktion auf mehrere Auflistungen anwenden, während Optionen unter **[!UICONTROL Select]** in der Spalte _[!UICONTROL Action]_die Aktion nur auf die einzelne Auflistung anwenden.

Siehe auch [Verwalten von Auflistungen nach Aktion](./managing-listings-by-action.md).

![Registerkarten für Produktlisten](assets/amazon-product-listings-tabs.png){width="600" zoomable="yes"}

| Registerkarte | Beschreibung | Aktionen |
|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | Zeigt Ihre [!DNL Commerce] -Katalogprodukte an, die Ihren definierten Listeneinstellungen entsprechen, aber Informationen fehlen, die von Amazon für eine Auflistung benötigt werden.<br><br> Wenn _[!UICONTROL Automatic List Action]_in Ihren [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md)-Einstellungen auf `Automatically List Eligible Products` gesetzt ist, sind diese Elemente Ihre **[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | Zeigt Ihre vorhandenen Amazon-Listen (basierend auf von Amazon erhaltenen Informationen) an, die nicht mit einem Produkt in Ihrem [!DNL Commerce] -Katalog übereinstimmen. | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>Versuchen Sie eine automatische Übereinstimmung<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | Zeigt Ihre Katalogprodukte an, die bereit sind, Amazon-Listen zu erstellen. Ihr Store ist jedoch so eingestellt, dass neue Listen nicht automatisch veröffentlicht werden. Mit diesem Tab können Sie Ihre neuen Listen manuell veröffentlichen.<br><br> Wenn _[!UICONTROL Automatic List Action]_in Ihren [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md)-Einstellungen auf `Do Not Automatically List Eligible Products` gesetzt ist, sind diese Elemente Ihre **[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | Zeigt Ihre Katalogprodukte an, die in Amazon veröffentlicht wurden, Amazon jedoch die Auflistung für den Status &quot;Aktiv&quot;nicht genehmigt hat. | [Ende Listen in Amazon](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Umschalten auf Erfüllt durch Amazon/Händler<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | Zeigt Ihre Amazon-Auflistungen an, die mit einem Produkt in Ihrem [!DNL Commerce]-Katalog übereinstimmen, in Amazon veröffentlicht wurden und von Amazon für den Status &quot;Aktiv&quot;erstellt wurden. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Umschalten auf Erfüllt durch Amazon/Händler<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | Zeigt Ihre Amazon-Listen an, die die Kriterien für eine definierte Überschreibung erfüllen und auf die die Überschreibung angewendet wurde. Überschreibungen haben Vorrang vor allen anderen Kontoeinstellungen. | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | Zeigt Ihre vorhandenen Amazon-Listen an, die nicht mehr berechtigt sind, basierend auf Ihren definierten [Listeneinstellungen](./listing-settings.md). | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Umschalten auf Erfüllt durch Amazon/Händler<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | Zeigt Ihre Amazon-Listen an, die manuell aus Amazon beendet (entfernt) wurden. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## Produktlisten aufrufen

1. Wechseln Sie in der Seitenleiste _Admin_ zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicken Sie auf der Speicherkarte auf **[!UICONTROL View Store]**.

1. Klicken Sie im Store-Dashboard im Abschnitt _[!UICONTROL Store Listings]_auf **[!UICONTROL Manage Listings]**.
