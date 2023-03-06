---
title: Verwalten von Produktlisten nach Status/Registerkarte
description: Bei der Verwaltung Ihrer Amazon-Listen können Sie je nach Status Aktionen auf Ihre Listen anwenden.
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Verwalten von Produktlisten nach Status/Registerkarte

Die _[!UICONTROL Product Listings]_-Seite enthält mehrere Registerkarten, über die Sie die Status aller Ihrer Listen anzeigen und Ihre Produkte mit Amazon-Listen abgleichen können.

Die verfügbaren Auflistungsaufgaben unterscheiden sich auf den einzelnen Registerkarten geringfügig, die [Arbeitsbereichssteuerelemente](./workspace-controls.md) sind identisch und ermöglichen es Ihnen, die Daten anzupassen, die für Ihre Auflistungen angezeigt werden.

Optionen unter **[!UICONTROL Actions]** kann die Aktion auf mehrere Listen anwenden, während Optionen unter **[!UICONTROL Select]** im _[!UICONTROL Action]_-Spalte nur auf die einzelne Auflistung anwenden.

Siehe auch [Verwalten von Listen nach Aktion](./managing-listings-by-action.md).

![Registerkarten für Produktlisten](assets/amazon-product-listings-tabs.png)

| Registerkarte | Beschreibung | Aktionen |
|--- |--- |--- |
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | Zeigt Ihre [!DNL Commerce] -Katalogprodukte, die Ihren definierten Listeneinstellungen entsprechen, aber Informationen fehlen, die von Amazon für eine Auflistung benötigt werden.<br><br>Wenn _[!UICONTROL Automatic List Action]_auf `Automatically List Eligible Products` in [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) -Einstellungen, sind diese Elemente Ihre **[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | Zeigt Ihre vorhandenen Amazon-Listen (basierend auf von Amazon erhaltenen Informationen) an, die nicht mit einem Produkt in Ihrer [!DNL Commerce] Katalog. | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>Automatische Übereinstimmung versuchen<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | Zeigt Ihre Katalogprodukte an, die bereit sind, Amazon-Listen zu erstellen. Ihr Store ist jedoch so eingestellt, dass neue Listen nicht automatisch veröffentlicht werden. Mit diesem Tab können Sie Ihre neuen Listen manuell veröffentlichen.<br><br>Wenn _[!UICONTROL Automatic List Action]_auf `Do Not Automatically List Eligible Products` in [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) -Einstellungen, sind diese Elemente Ihre **[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | Zeigt Ihre Katalogprodukte an, die in Amazon veröffentlicht wurden, Amazon jedoch die Auflistung für den Status &quot;Aktiv&quot;nicht genehmigt hat. | [Ende Listen in Amazon](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Zu Amazon/Merchant wechseln<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | Zeigt Ihre Amazon-Listen an, die mit einem Produkt in Ihrer [!DNL Commerce] Katalog, wurden in Amazon veröffentlicht und wurden von Amazon für den Status &quot;Aktiv&quot;ausgewählt. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Zu Amazon/Merchant wechseln<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | Zeigt Ihre Amazon-Listen an, die die Kriterien für eine definierte Überschreibung erfüllen und auf die die Überschreibung angewendet wurde. Überschreibungen haben Vorrang vor allen anderen Kontoeinstellungen. | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | Zeigt Ihre vorhandenen Amazon-Listen an, die nicht mehr berechtigt sind, basierend auf Ihrer Definition. [Auflistungseinstellungen](./listing-settings.md). | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Zu Amazon/Merchant wechseln<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | Zeigt Ihre Amazon-Listen an, die manuell aus Amazon beendet (entfernt) wurden. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## Produktlisten aufrufen

1. Im _Admin_ Seitenleiste, navigieren Sie zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klicken **[!UICONTROL View Store]** auf der Speicherkarte.

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Manage Listings]** im _[!UICONTROL Store Listings]_Abschnitt.
