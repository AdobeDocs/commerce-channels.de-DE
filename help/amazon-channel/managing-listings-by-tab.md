---
title: Produktlisten nach Status/Register verwalten
description: Wenn Sie Ihre Amazon-Listen verwalten, können Sie Aktionen entsprechend dem Status auf Ihre Listen anwenden.
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# Produktauflistungen nach Status/Registerkarte verwalten

Die _[!UICONTROL Product Listings]_enthält mehrere Registerkarten, von denen Sie den Status aller Ihrer Auflistungen Ansicht haben und Ihre Produkte mit den Amazon-Auflistungen abgleichen können.

Die verfügbaren Aufgaben in der Auflistung unterscheiden sich auf den einzelnen Registerkarten geringfügig, aber die [Arbeitsbereichssteuerelemente](./workspace-controls.md) sind identisch und ermöglichen es Ihnen, die Daten, die für Ihre Auflistungen angezeigt werden, anzupassen.

Optionen unter **[!UICONTROL Actions]** kann die Aktion auf mehrere Auflistungen anwenden, während die Optionen unter **[!UICONTROL Select]** in _[!UICONTROL Action]_-Spalte die Aktion nur auf die einzelne Auflistung anwenden.

Siehe auch [Auflistungen nach Aktion verwalten](./managing-listings-by-action.md).

![Registerkarte &quot;Produktauflistungen&quot;](assets/amazon-product-listings-tabs.png)

| Tabulator | Beschreibung | Aktionen |
|--- |--- |--- |
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | Zeigt Ihre [!DNL Commerce] Katalogprodukte, die Ihren festgelegten Listenereinstellungen entsprechen, aber Informationen fehlen, die Amazon für eine Auflistung benötigt.<br><br>Falls _[!UICONTROL Automatic List Action]_ist eingestellt auf `Automatically List Eligible Products` in [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) Einstellungen, diese Elemente sind Ihre **[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | Zeigt Ihre vorhandenen Amazon-Auflistungen (basierend auf von Amazon erhaltenen Informationen) an, die keinem Produkt in Ihrem [!DNL Commerce] Katalog. | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>Automatische Übereinstimmung versuchen<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | Zeigt die Katalogprodukte an, die bereit sind, Amazon-Auflistungen zu erstellen. Ihr Store ist jedoch nicht so eingestellt, dass neue Auflistungen automatisch veröffentlicht werden. Diese Registerkarte wird verwendet, um Ihre neuen Einträge manuell zu veröffentlichen.<br><br>Falls _[!UICONTROL Automatic List Action]_ist eingestellt auf `Do Not Automatically List Eligible Products` in [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) Einstellungen, diese Elemente sind Ihre **[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | Zeigt Ihre Katalogprodukte an, die auf Amazon veröffentlicht wurden, aber Amazon hat die Auflistung für den Status &quot;Aktiv&quot;nicht genehmigt. | [Ende Liste(n) auf Amazon](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Von Amazon/Händler zu &quot;Erfüllt/Erfüllt&quot;wechseln<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | Zeigt Ihre Amazon-Auflistungen an, die mit einem Produkt in Ihrer [!DNL Commerce] , wurden auf Amazon veröffentlicht und wurden von Amazon für den Status &quot;Aktiv&quot;ausgewählt. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Von Amazon/Händler zu &quot;Erfüllt/Erfüllt&quot;wechseln<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | Zeigt Ihre Amazon-Auflistungen an, die die Kriterien für eine definierte Außerkraftsetzung erfüllen und auf die die Außerkraftsetzung angewendet wurde. Überschreibung hat Vorrang vor jeder anderen Kontoeinstellung. | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | Zeigt Ihre vorhandenen Amazon-Auflistungen an, die aufgrund Ihrer Definition nicht mehr förderfähig sind. [Listeneinstellungen](./listing-settings.md). | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Von Amazon/Händler zu &quot;Erfüllt/Erfüllt&quot;wechseln<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | Zeigt Ihre Amazon-Auflistungen an, die manuell aus Amazon beendet (entfernt) wurden. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## Auf Produktlisten zugreifen

1. Auf _Admin_ Sidebar, Gehe zu **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. Klick **[!UICONTROL View Store]** auf der Ladenkarte.

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Manage Listings]** in _[!UICONTROL Store Listings]_Abschnitt.
