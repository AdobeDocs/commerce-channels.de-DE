---
title: Verwalten von Listen
description: "Verwalten Sie Vertriebskanallisten für einen [!DNL Commerce] Speicher mit dem Kanal-Manager für Adobe Commerce und Magento Open Source."
feature: Sales Channels, Merchandising, Products
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Verwalten von Listen

Verwalten Sie Produktlisten für den Absatzkanal [!DNL Walmart Marketplace] über die Benutzeroberfläche des Kanalmanagers.

Der Status einer einzelnen Auflistung zeigt an, wo sich das Produkt im Workflow [!DNL Channel Manager] befindet, sodass Sie die nächsten Schritte bestimmen und Fehler beheben können.

![Listenseite für einen verbundenen Vertriebskanal](assets/listings-dashboard-view.png){width="500" zoomable="yes"}

Sie können die folgenden Aufgaben in der Listenansicht ausführen.

* Aktuelle Listen anzeigen
* Sortieren und Filtern von Listen
* Produkte hinzufügen
* Produkte abgleichen
* Status der Tracking-Liste
* Fehlerbeschreibung für Listen mit Fehlerstatus überprüfen

## Anzeigen von Produktlisten

1. Wechseln Sie vom Administrator zu [!UICONTROL **Marketing** > **Kanal-Manager**].

1. Wählen Sie in der Liste Store das Augensymbol in einer Store-Einstiegszeile aus, um die Store-Ansicht zu öffnen.

1. Wählen Sie [!UICONTROL **Auflistungen**] aus.

1. Sortieren Sie die Ansicht *Auflistung*, indem Sie eine beliebige Spaltenüberschrift in der Tabelle *Auflistung* auswählen.

1. Filtern Sie die Ansicht *Auflisten*, indem Sie eine der Statuszählungskarten auswählen.

1. Setzen Sie die Sortierreihenfolge zurück und entfernen Sie Filter, indem Sie **Produkte aktualisieren** auswählen.

## Hinzufügen von [!DNL Commerce] -Produkten zum Kanal-Manager

Erstellen Sie das Produktsortiment für den Kanal [!DNL Walmart Marketplace] , indem Sie die folgenden Aufgaben ausführen:

* [Produkte aus Ihrem [!DNL Commerce] Produktkatalog zu  [!DNL Channel Manager] hinzufügen](add-products-to-channel-store.md)

* [Katalogattribute zuordnen](map-catalog-attributes.md#configure-product-attribute-settings)

## Übereinstimmung mit Produkten mit [!DNL Walmart]

Sie können Produktangebote für die [!DNL Walmart Marketplace] erstellen, indem Sie die Produktübereinstimmung verwenden oder Produktlisten für neue Produkte manuell hochladen.

* **[Produkte in Walmart abgleichen](connect-listings-to-marketplace.md)** - Verbinden Sie Produktlisten von Ihrem Kanal zu [!DNL Walmart Marketplace], indem Sie vorhandene Listen aktualisieren, die dasselbe Produkt verkaufen. Übereinstimmungskriterien werden durch die [Konfiguration der Zuordnung von Attributen](map-catalog-attributes.md) für Ihren Kanal bestimmt.

* **[Manuelles Hochladen neuer Listen](connect-listings-to-marketplace.md#upload-new-product-listings)**: Verwenden Sie für Produkte, die nicht mit einer vorhandenen Liste auf [!DNL Walmart Marketplace] übereinstimmen, eine Excel-Vorlage der Produktkategorie [!DNL Walmart] , um Produktlisten stapelweise hochzuladen.

## Listen- und Spaltenbeschreibungen

In den folgenden Tabellen werden die für [!UICONTROL Listings] verfügbaren Steuerelemente und Spalten beschrieben.

**Steuerelemente für[!UICONTROL Listings]**

| **Kontrolle** | **Beschreibung** |
|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Öffnet die Seite &quot;[!UICONTROL Admin Product Catalog]&quot;, auf der Sie Produkte auswählen können, die Sie Ihrem [!DNL Walmart Marketplace]-Sortiment hinzufügen möchten, oder um Produktattribute zu aktualisieren, um die Anforderungen der Walmart Marketplace-Auflistung zu erfüllen. |
| [!UICONTROL Match products on Walmart] | Nachdem Sie ein oder mehrere Produkte mit dem Status [!UICONTROL Draft] ausgewählt haben, wählen Sie [!UICONTROL Match products on Walmart] aus, um nach Produktangeboten zu suchen, die einer vorhandenen [!DNL Walmart Marketplace]-Liste hinzugefügt werden können. |
| [!UICONTROL Refresh products] | Aktualisieren Sie die Anzeige mit der aktuellsten Liste und dem aktuellen Status. Dieses Steuerelement setzt auch die Listenansicht auf die standardmäßige Sortierreihenfolge zurück und entfernt alle Filter. |
| [!UICONTROL Filter by *Status*] | Zeigen Sie nur Listen mit einem bestimmten Status an, indem Sie eine der Statuskarten über der Tabelle Liste auswählen. Entfernen Sie den Filter durch Auswahl von **[!UICONTROL Refresh products]**. |
| [!UICONTROL Sort products] | Ändern Sie die Sortierreihenfolge für die Auflistung, indem Sie eine beliebige Spaltenüberschrift auswählen. |


**Spaltenbeschreibungen**

| **Feld** | **Beschreibung** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Name des Produkts aus dem [!DNL Commerce] Store-Katalog. |
| [!UICONTROL SKU (Unique ID)] | Die SKU, die dem Produkt im [!DNL Commerce] -Katalog zugewiesen ist. |
| [!UICONTROL  Quantity] | Umfang des in Adobe Commerce oder Magento Open Source verfügbaren Bestands. |
| [!UICONTROL Price] | Der Produktpreis aus dem [!DNL Commerce] -Store-Katalog. Aktualisierungen des Katalogpreises werden mit dem Kanal-Manager synchronisiert und dann an [!DNL Walmart Marketplace] gesendet, sodass die aufgelisteten Elemente den aktuellen Preis anzeigen. |
| [!UICONTROL Status] | Gibt den aktuellen Bestellstatus im Workflow [!DNL Commerce] Bestellung an. Der Status wird aktualisiert, wenn Sie erfolgreich Produkte zu [!DNL Channel Manager] hinzufügen und wenn Sie Produkte auf dem Marketplace zuordnen. Wenn ein Vorgang fehlschlägt, zeigt die Auflistung einen Fehlerstatus an. Nach Behebung des Fehlers versucht [!DNL Channel Manager] den Vorgang erneut und aktualisiert den Status. |
| [!UICONTROL Error Description] | Bietet zusätzliche Fehlerinformationen für Produkte mit dem Status `[!DNL Error]` . |

### Über den Listenstatus

Im Arbeitsbereich &quot;Auflisten&quot;zeigt die Bezeichnung Status an, wo sich ein Produkt im Arbeitsablauf [!DNL Channel Manager] befindet, sodass Sie die nächsten Schritte bestimmen und Fehler beheben können. Listen können die folgenden Statusbezeichnungen aufweisen:

* **[!UICONTROL Draft]**-Identifiziert Produkte, die nicht [zur Übereinstimmung an ](connect-listings-to-marketplace.md#match-products) gesendet wurden. [!DNL Walmart] 

* **[!UICONTROL Processing]**—Identifiziert Produkte, die zum Abgleich auf dem [!DNL Walmart Marketplace] gesendet wurden. Produkte bleiben im Status *Verarbeitung* , bis [!DNL Walmart] eine HTTP-Statusmeldung zurückgibt, die angibt, ob die Übereinstimmung erfolgreich war oder ob ein Fehler aufgetreten ist. Es kann bis zu 30 Minuten dauern, bis der Match-Vorgang mit dem [!DNL Walmart Marketplace] abgeschlossen ist.

* **[!UICONTROL Match]**-Identifiziert Produkte, die bei [!DNL Walmart] erfolgreich abgeglichen wurden.

  Eine Übereinstimmung tritt auf, wenn der Produktattributwert - z. B. der UPC-Code - mit dem UPC-Wert in einer vorhandenen [!DNL Walmart Marketplace]-Auflistung übereinstimmt. Wenn ein Produkt übereinstimmt, wird das Commerce-Produktangebot der vorhandenen Liste hinzugefügt.

  Überprüfen Sie das Dashboard [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) , um die aktualisierte Produktliste zu überprüfen und Produktdetails, Preis und Lagerbestandsmenge zu überprüfen.

* **[!UICONTROL Match - Match in Stage]**—Identifiziert Produkte, die mit [!DNL Walmart] übereinstimmen und erst dann verbunden werden können, wenn der [!DNL Walmart Marketplace]-Store live ist. Produkte mit diesem Status werden automatisch verbunden, wenn der [!DNL Walmart Marketplace]-Store live geschaltet wird.

* **[!UICONTROL Error]**—Identifiziert Produkte, die nicht mit einer vorhandenen [!DNL Walmart Marketplace]-Liste übereinstimmen.

* **[!UICONTROL Error description]** - Bietet detaillierte Informationen zum Listenfehler.

  Nachdem Sie den Fehler behoben haben, senden Sie das Produkt erneut zur Übereinstimmung. Siehe [Fehlerbehebung bei Produktübereinstimmungsfehlern](connect-listings-to-marketplace.md#troubleshoot-product-match-errors).
