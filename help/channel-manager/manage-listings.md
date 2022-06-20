---
title: Verwalten von Listen
description: Verwalten von Verkaufskanallisten für eine [!DNL Commerce] mit dem Kanal-Manager für Adobe Commerce und Magento Open Source speichern.
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 690eeb5d03b23cac11f3c14b04601c514c76e0bd
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Listen verwalten

Produktlisten für die [!DNL Walmart Marketplace] Vertriebskanal über die Kanal-Manager-Benutzeroberfläche.

Der Status für eine einzelne Auflistung zeigt an, wo sich das Produkt im [!DNL Channel Manager] -Workflow, damit Sie die nächsten Schritte bestimmen und etwaige Fehler beheben können.

![Listenseite für einen verbundenen Vertriebskanal](assets/listings-dashboard-view.png)

Sie können die folgenden Aufgaben in der Listenansicht ausführen.

* Aktuelle Listen anzeigen
* Sortieren und Filtern von Listen
* Produkte hinzufügen
* Produkte abgleichen
* Status der Tracking-Liste
* Fehlerbeschreibung für alle Produktlisten mit Fehlerstatus

## Anzeigen von Produktlisten

1. Navigieren Sie vom Administrator zu [!UICONTROL **Marketing** > **Kanal-Manager**].

1. Wählen Sie in der Liste Store das Augensymbol in einer Store-Einstiegszeile aus, um die Store-Ansicht zu öffnen.

1. Auswählen [!UICONTROL **Auflistungen**].

1. Sortieren Sie die *Auflistung* Ansicht durch Auswahl einer Spaltenüberschrift im *Auflistung* Tabelle.

1. Filtern Sie die *Auflistung* anzeigen, indem Sie eine der Statuszählungskarten auswählen.

1. Die Sortierreihenfolge zurücksetzen und Filter durch Auswahl von **Produkte aktualisieren**.

## Hinzufügen von Commerce-Produkten zum Kanal-Manager

Erstellen Sie das Produktangebot für die [!DNL Walmart Marketplace] -Kanal durch Ausführen der folgenden Aufgaben:

* [Produkte aus Ihrem [!DNL Commerce] Produktkatalog [!DNL Channel Manager]](add-products-to-channel-store.md)

* [Katalogattribute zuordnen](map-catalog-attributes.md#configure-product-attribute-settings)

## Produkte abgleichen auf [!DNL Walmart]

Sie können Produktangebote auf der [!DNL Walmart Marketplace] durch Abgleich von Produkten oder manuelles Hochladen von Produktlisten für neue Produkte.

* **[Produkte bei Walmart abgleichen](connect-listings-to-marketplace.md)**—Produktlisten von Ihrem Kanal zu verbinden [!DNL Walmart Marketplace] durch Aktualisierung bestehender Listen, die dasselbe Produkt verkaufen. Übereinstimmungskriterien werden durch die [attribute-mapping-Konfiguration](map-catalog-attributes.md) für Ihren Kanal.

* **[Manuelles Hochladen neuer Listen](connect-listings-to-marketplace.md#upload-new-product-listings)**—Für Produkte, die nicht mit einer vorhandenen Liste auf übereinstimmen. [!DNL Walmart Marketplace], verwenden Sie eine [!DNL Walmart] Produktkategorie Excel-Vorlage zum Massen-Upload von Produktlisten.

## Listen- und Spaltenbeschreibungen

Die folgenden Tabellen beschreiben die verfügbaren Steuerelemente und Spalten für [!UICONTROL Listings].

**Steuerelemente für[!UICONTROL Listings]**

| **Kontrolle** | **Beschreibung** |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Öffnet die [!UICONTROL Admin Product Catalog] Seite zum Auswählen der Produkte, die Sie zu Ihrem [!DNL Walmart Marketplace] Sortierung oder Aktualisierung von Produktattributen, um die Anforderungen an die Auflistung von Walmart Marketplace zu erfüllen. |
| [!UICONTROL Match products on Walmart] | Nachdem Sie ein oder mehrere Produkte im Status Entwurf ausgewählt haben, wählen Sie Produkte abgleichen auf [!DNL Walmart] , um nach Produktangeboten zu suchen, die einem vorhandenen hinzugefügt werden können [!DNL Walmart Marketplace] Auflistung. |
| [!UICONTROL Refresh products] | Aktualisieren Sie die Anzeige mit der aktuellsten Liste und dem aktuellen Status. Dieses Steuerelement setzt auch die Listenansicht auf die standardmäßige Sortierreihenfolge zurück und entfernt alle Filter. |
| [!UICONTROL Filter by *Status*] | Zeigen Sie nur Auflistungen mit einem bestimmten Status an, indem Sie eine der Statuszählungskarten über der Listing-Tabelle auswählen. Verwenden Sie die *Produkte aktualisieren* , um den Filter zu entfernen. |
| [!UICONTROL Sort products] | Ändern Sie die Sortierreihenfolge für die Auflistung, indem Sie eine beliebige Spaltenüberschrift auswählen. |


**Spaltenbeschreibungen**

| **Feld** | **Beschreibung** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Name des Produkts aus der [!DNL Commerce] Katalog speichern. |
| [!UICONTROL SKU (Unique ID)] | Die SKU, die dem Produkt in der [!DNL Commerce] Katalog. |
| [!UICONTROL  Quantity] | Umfang des in Adobe Commerce oder Magento Open Source verfügbaren Bestands. |
| [!UICONTROL Price] | Der Produktpreis aus dem [!DNL Commerce] Katalog speichern. Aktualisierungen des Katalogpreises werden mit dem Kanal-Manager synchronisiert und dann an [!DNL Walmart Marketplace]  sodass die aufgelisteten Artikel den aktuellen Preis anzeigen. |
| [!UICONTROL Status] | Gibt den aktuellen Bestellstatus im [!DNL Commerce] Bestellworkflow. Der Status wird aktualisiert, wenn Sie erfolgreich Produkte zu [!DNL Channel Manager] und wenn Sie Produkte auf dem Markt finden. Wenn ein Vorgang fehlschlägt, zeigt die Auflistung einen Fehlerstatus an. Nachdem Sie den Fehler behoben haben, [!DNL Channel Manager] wiederholt den Vorgang und aktualisiert den Status. |
| [!UICONTROL Error Description] | Bietet zusätzliche Fehlerinformationen für Produkte mit einer `[!DNL Error]` Status. |
| [!UICONTROL Status Detail] | Bietet zusätzliche Informationen zu Produkten mit *Fehler* oder *Übereinstimmung* Status. |

### Über den Listenstand

Im Arbeitsbereich &quot;Listen&quot;zeigt die Bezeichnung Status an, wo sich ein Produkt im [!DNL Channel Manager] -Arbeitsablauf, damit Sie die nächsten Schritte bestimmen und Fehler beheben können. Listen können die folgenden Statusbezeichnungen aufweisen:

* **[!UICONTROL Draft]**- Identifiziert nicht vorhandene Produkte [eingereicht [!DNL Walmart] für Abgleich](connect-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**—Identifiziert Produkte, die zum Abgleich auf der [!DNL Walmart Marketplace]. Produkte verbleiben in *Verarbeitung* bis zum [!DNL Walmart] gibt eine HTTP-Statusmeldung zurück, die angibt, ob die Übereinstimmung erfolgreich war oder ob ein Fehler aufgetreten ist. Es kann bis zu 30 Minuten dauern, bis der Match-Vorgang am [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identifiziert Produkte, die erfolgreich zugewiesen wurden unter [!DNL Walmart].

   Eine Übereinstimmung tritt auf, wenn der Produktattributwert - z. B. der UPC-Code - mit dem UPC-Wert in einem vorhandenen übereinstimmt [!DNL Walmart Marketplace] Auflistung. Wenn ein Produkt übereinstimmt, wird das Commerce-Produktangebot dem vorhandenen hinzugefügt [!DNL Walmart] Auflistung.

   Überprüfen Sie die [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) Dashboard , um die aktualisierte Produktliste zu überprüfen und Produktdetails, Preise und Lagerbestände zu überprüfen.

* **[!UICONTROL Match - Match in Stage]**—Identifiziert Produkte, die übereinstimmen mit [!DNL Walmart] die erst dann verbunden werden können, wenn die [!DNL Walmart Marketplace] Store ist live. Produkte mit diesem Status werden automatisch verbunden, wenn die Variable [!DNL Walmart Marketplace] Store wird live geschaltet.

* **[!UICONTROL Error]**—Identifiziert Produkte, die nicht mit einem vorhandenen übereinstimmen [!DNL Walmart Marketplace] Auflistung.

* **[!UICONTROL Error description]**—Bietet detaillierte Informationen zum Listenfehler.

   Nachdem Sie den Fehler behoben haben, senden Sie das Produkt erneut zur Übereinstimmung. Siehe [Fehlerbehebung bei Produktübereinstimmungsfehlern](connect-listings-to-marketplace.md#troubleshoot-product-match-errors).
