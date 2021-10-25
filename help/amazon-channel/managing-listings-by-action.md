---
title: Produktauflistungen nach Aktion verwalten
description: Wenn Sie Ihre Amazon-Listen verwalten, können Sie eine Aktion auf einzelne oder mehrere Auflistungen anwenden.
exl-id: 1cbf16fb-15eb-484b-bea7-28017a0d0c60
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Produktauflistungen nach Aktion verwalten

Die _[!UICONTROL Product Listings]_enthält mehrere Registerkarten, von denen Sie den Status aller Ihrer Auflistungen Ansicht haben und Ihre Produkte mit den Amazon-Auflistungen abgleichen können.

Die verfügbaren Aufgaben in der Auflistung unterscheiden sich auf den einzelnen Registerkarten geringfügig, aber die [Arbeitsbereichssteuerelemente](./workspace-controls.md) sind identisch und ermöglichen es Ihnen, die Daten, die für Ihre Auflistungen angezeigt werden, anzupassen.

Optionen unter **[!UICONTROL Actions]** kann die Aktion auf mehrere Auflistungen anwenden, während die Optionen unter **[!UICONTROL Select]** in _[!UICONTROL Action]_-Spalte die Aktion nur auf die einzelne Auflistung anwenden.

Siehe auch [Listen nach Status/Register verwalten](./managing-listings-by-tab.md).

| Aktion | Beschreibung | Registerkarten |
|--- |--- |--- |
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | Wird verwendet, um die unvollständigen Produkte durch den Übereinstimmungsprozess zurück zu verschieben. Um eine Anpassung zu versuchen, müssen Sie Ihre [Auflistung](./listing-settings.md) und [Katalogsuche](./catalog-search.md) -Einstellungen, um das Potenzial für die automatische Zuordnung zu erhöhen. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | Passen Sie Ihre Katalogprodukte manuell an Amazon-Auflistungen an, indem Sie eine passende Liste auswählen, ein passendes ASIN eingeben oder eine fehlende Bedingung zuweisen. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | Ansicht zusätzlicher Informationen zu Ihren aktiven Produkten, einschließlich des Listing Aktivität Log, das die Änderungen an einer einzelnen SKU/Produkt anzeigt. | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | Erstellen Sie eine [!DNL Commerce] Katalogprodukt mit den mit der Amazon-Auflistung importierten Informationen. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| Automatische Übereinstimmung versuchen | Versuchen Sie, eine automatische Übereinstimmung zwischen Ihrem [!DNL Commerce] -Katalog und Ihre Amazon-Einträge auf der Grundlage der Suchkriterien-Einstellungen. Um eine Anpassung zu versuchen, müssen Sie Ihre [Auflistung](./listing-settings.md) und [Katalogsuche](./catalog-search.md) -Einstellungen, um das Potenzial für die automatische Zuordnung zu erhöhen. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | Wählen Sie ein bestehendes Produkt manuell in Ihrem [!DNL Commerce] und ordnen Sie es der Amazon-Auflistung zu. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | Erstellen Sie eine [!DNL Commerce] Katalogprodukt mit den mit der Amazon-Auflistung importierten Informationen. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | (Massenaktion) Wird verwendet, um eine Liste neu aufzulisten, die beendet wurde, oder um ein Produkt manuell Liste, das Ihre Berechtigung für die Aufnahme von Regeln erfüllt, aber Ihre _[!UICONTROL Product Listing Actions]_ist nicht festgelegt auf `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | (Einzelauflistungsaktion) Wird verwendet, um eine beendete Auflistung neu aufzulisten. Diese Aktion wird auch verwendet, um ein Produkt manuell Liste, das Ihre Berechtigung für die Auflistung von Regeln erfüllt, wenn _[!UICONTROL Product Listing Actions]_ist nicht festgelegt auf `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | (Massenaktion) Wird zum manuellen Beenden und Entfernen von Auflistungen für Ihre auf Amazon vorhandenen Produkte verwendet. Ended listings können zuverlässig sein, solange sie Ihre Berechtigung zur Auflistung der Regeln erfüllen. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | (Massenaktion) Bearbeiten Sie manuell eine vorhandene &quot;Außerkraftsetzung&quot;, die den Preis, die Bearbeitungszeit, die Bedingung und den Hinweis des Verkäufers für eine einzelne Auflistung festlegt. Dabei werden andere Standardwerte, Einstellungen und Regeln für die Auflistung ignoriert. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | Erstellen Sie manuell eine &quot;Außerkraftsetzung&quot;, die den Preis, die Bearbeitungszeit, die Bedingungen und den Händlernotentext für eine einzelne Auflistung festlegt. Dabei werden andere Standardwerte, Einstellungen und Regeln für die Auflistung ignoriert. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | Wird verwendet, wenn die ASIN, die Ihrem Katalogprodukt entspricht, geändert werden muss (Beispiel: wenn das Produkt der falschen ASIN-Auflistung zugeordnet wurde). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | Kann zwei Funktionen erfüllen:<br><br>Kann verwendet werden, um eine 1:2-Beziehung zwischen Ihrem Katalogprodukt und zwei Amazon-Auflistungen zu erstellen. Beispiel: Amazon hat das Produkt mit verschiedenen ASIN-Werten aufgelistet. Sie können Ihr Katalogprodukt mit beiden ASIN-Auflistungen für das Produkt abgleichen.<br><br>Kann verwendet werden, um eine Auflistung in verschiedenen Amazon-Regionen zu kontrollieren. Beispiel: Sie verfügen über ein Katalogprodukt, dessen Versandmethoden je nach Region Amazon unterschiedlich definiert sind (US-Region ist FBA und Kanada ist FBM). Zur Kontrolle von Bestand/Menge können Sie einen Alias-Verkäufer SKU erstellen und dasselbe Produkt in dieser Region mit einer anderen Verkäufer-SKU neu auflisten. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | Wird verwendet, um die mit Ihrem Produkt verknüpfte Fulfillment-Methode zu ändern (Amazon: FBA oder vom Händler ausgefüllt: FBM). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | (Einzelauflistungsaktion) Wird verwendet, um Auflistungen für Ihre auf Amazon vorhandenen Produkte manuell zu beenden und zu entfernen. Ended listings können zuverlässig sein, solange sie Ihre Berechtigung zur Auflistung der Regeln erfüllen. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | (Einzellistungsaktion) Bearbeiten Sie manuell eine vorhandene &quot;Außerkraftsetzung&quot;, die den Preis, die Bearbeitungszeit, die Bedingungen und den Händlernotentext für eine einzelne Auflistung festlegt, und ignorieren Sie dabei andere Standardwerte, Einstellungen und Regeln für die Auflistung. | [[!UICONTROL Overrides]](./overrides.md) |

## Auf Produktlisten zugreifen

1. Auf _Admin_ Sidebar, Gehe zu **Marketing** > _Kanal_ > **Amazon Sales Channel**.

1. Klick **Ansicht Store** auf der Ladenkarte.

1. Klicken Sie im Store-Dashboard auf **Listen verwalten** in _Filialauflistungen_ Abschnitt.
