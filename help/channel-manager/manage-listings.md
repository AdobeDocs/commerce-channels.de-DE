---
title: Verwalten von Listen
description: Verwalten von Verkaufskanallisten für eine [!DNL Commerce] mit dem Kanal-Manager für Adobe Commerce und Magento Open Source speichern.
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 71ad5e3bc9ff6b909943a161472e4db7d375683f
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 0%

---

# Listen verwalten

Produktlisten für die [!DNL Walmart Marketplace] Vertriebskanal aus [!UICONTROL Listings] in der Kanalspeicheransicht. Der Status für eine einzelne Auflistung zeigt an, wo sich das Produkt im [!DNL Channel Manager] -Workflow, damit Sie die nächsten Schritte bestimmen und etwaige Fehler beheben können.

Der Status für eine einzelne Auflistung zeigt an, wo sich das Produkt im [!DNL Channel Manager] -Workflow, damit Sie die nächsten Schritte bestimmen und etwaige Fehler beheben können.

![Listenseite für einen verbundenen Vertriebskanal](assets/product-listing-landing.png)

Sie können die folgenden Aufgaben in der Listenansicht ausführen.

* Aktuelle Listen anzeigen
* Sortieren und Filtern von Listen
* Produkte hinzufügen
* Produkte abgleichen
* Status der Tracking-Liste

## Anzeigen von Produktlisten

1. Navigieren Sie vom Administrator zu [!UICONTROL **Marketing** > Kanäle > **Kanal-Manager**].

1. Wählen Sie in der Liste &quot;Channel Store&quot;das Stiftsymbol in einer Store-Einstiegszeile aus, um die Store-Ansicht zu öffnen.

1. Auswählen [!UICONTROL **Auflistungen**].

1. Sortieren Sie die *Auflistung* Ansicht durch Auswahl einer Spaltenüberschrift im *Auflistung* Tabelle.

1. Filtern Sie die *Auflistung* anzeigen, indem Sie eine der Statuszählungskarten auswählen.

1. Die Sortierreihenfolge zurücksetzen und Filter durch Auswahl von **Produkte aktualisieren**.

## Hinzufügen von Commerce-Produkten zum Kanal-Manager

Erstellen Sie das Produktsortiment für den Kanal Walmart Marketplace , indem Sie die folgenden Aufgaben ausführen:

* [Hinzufügen von Produkten aus Ihrem Commerce-Produktkatalog zum Channel Manager](add-products-to-channel-store.md)

* [Katalogattribute zuordnen](map-catalog-attributes.md#configure-product-attribute-settings)

## Produkte in Walmart veröffentlichen

Sie können Produktangebote im Walmart Marketplace erstellen, indem Sie Produktabgleiche verwenden oder Produktlisten für neue Produkte manuell hochladen.

* **[Produkte bei Walmart abgleichen](publish-listings-to-marketplace.md)**—Veröffentlichen Sie Produktlisten von Ihrem Kanal in [!DNL Walmart Marketplace] durch Aktualisierung bestehender Listen, die dasselbe Produkt verkaufen. Übereinstimmungskriterien werden durch die [attribute-mapping-Konfiguration](map-catalog-attributes.md) für Ihren Kanal.

* **[Manuelles Hochladen neuer Listen](publish-listings-to-marketplace.md#upload-new-product-listings)**—Verwenden Sie für Produkte, die nicht mit einer vorhandenen Liste auf dem Walmart Marketplace übereinstimmen, eine Excel-Vorlage der Walmart-Produktkategorie, um Produktlisten stapelweise hochzuladen.

## Listen- und Spaltenbeschreibungen

Die folgenden Tabellen beschreiben die verfügbaren Steuerelemente und Spalten für [!UICONTROL Listings].

**Steuerelemente für[!UICONTROL Listings]**

| **Kontrolle** | **Beschreibung** |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | Öffnet die [!UICONTROL Admin Product Catalog] Seite zum Auswählen der Produkte, die Sie zu Ihrem [!DNL Walmart Marketplace] Sortierung oder Aktualisierung von Produktattributen, um die Anforderungen an die Auflistung von Walmart Marketplace zu erfüllen. |
| [!UICONTROL Match products on Walmart] | Nachdem Sie ein oder mehrere Produkte im Status Entwurf ausgewählt haben, wählen Sie Produkte in Walmart abgleichen aus, um nach Produktangeboten zu suchen, die einem vorhandenen hinzugefügt werden können. [!DNL Walmart Marketplace] Auflistung. |
| [!UICONTROL Refresh products] | Aktualisieren Sie die Anzeige mit der aktuellsten Liste und dem aktuellen Status. Dieses Steuerelement setzt auch die Listenansicht auf die standardmäßige Sortierreihenfolge zurück und entfernt alle Filter. |
| [!UICONTROL Filter by *Status*] | Zeigen Sie nur Auflistungen mit einem bestimmten Status an, indem Sie eine der Statuszählungskarten über der Listing-Tabelle auswählen. Verwenden Sie die *Produkte aktualisieren* , um den Filter zu entfernen. |
| [!UICONTROL Sort products] | Ändern Sie die Sortierreihenfolge für die Auflistung, indem Sie eine beliebige Spaltenüberschrift auswählen. |


**Spaltenbeschreibungen**

| **Feld** | **Beschreibung** |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Name des Produkts aus der [!DNL Commerce] Katalog speichern. |
| [!UICONTROL SKU (Unique ID)] | Das zugeordnete Attribut, das zum Abgleichen von Produkten auf dem Marketplace verwendet wird. Dieser Feldname hängt von der zugeordneten Attributkonfiguration für [!DNL Channel Manager] Auflistungen. In diesem Fall verwendet der Produktabgleichsvorgang die Produkt-SKU aus der [!DNL Commerce] Katalog zum Auffinden einer [!DNL Walmart Marketplace]  Liste mit einem SKU-Wert, der mit dem SKU-Wert aus der [!DNL Commerce] Produktattribute. |
| [!UICONTROL  Quantity] | Umfang des in Adobe Commerce oder Magento Open Source verfügbaren Bestands. |
| [!UICONTROL Price] | Der Produktpreis aus dem [!DNL Commerce] Katalog speichern. Aktualisierungen des Katalogpreises werden mit dem Kanal-Manager synchronisiert und dann an [!DNL Walmart Marketplace]  sodass die aufgelisteten Artikel den aktuellen Preis anzeigen. |
| [!UICONTROL Status] | Gibt den aktuellen Bestellstatus im [!DNL Commerce] Bestellworkflow. Der Status wird aktualisiert, wenn Sie erfolgreich Produkte zu [!DNL Channel Manager] und wenn Sie Produkte auf dem Markt finden. Wenn ein Vorgang fehlschlägt, zeigt die Auflistung einen Fehlerstatus an. Nachdem Sie den Fehler behoben haben, [!DNL Channel Manager] wiederholt den Vorgang und aktualisiert den Status. |
| [!UICONTROL Status Detail] | Bietet zusätzliche Informationen zu Produkten mit *Fehler* oder *Übereinstimmung* Status. |

### Über den Listenstand

Im Arbeitsbereich &quot;Listen&quot;zeigt die Bezeichnung Status an, wo sich ein Produkt im [!DNL Channel Manager] -Arbeitsablauf, damit Sie die nächsten Schritte bestimmen und Fehler beheben können. Listen können die folgenden Statusbezeichnungen aufweisen:

* **[!UICONTROL Draft]**- Identifiziert nicht vorhandene Produkte [eingereicht [!DNL Walmart] für Abgleich](publish-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**—Identifiziert Produkte, die zum Abgleich auf der [!DNL Walmart Marketplace]. Produkte verbleiben in *Verarbeitung* bis zum [!DNL Walmart] gibt eine HTTP-Statusmeldung zurück, die angibt, ob die Übereinstimmung erfolgreich war oder ob ein Fehler aufgetreten ist. Es kann bis zu 30 Minuten dauern, bis der Match-Vorgang am [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identifiziert Produkte, die erfolgreich zugewiesen wurden unter [!DNL Walmart].

   Eine Übereinstimmung tritt auf, wenn der Produktattributwert - z. B. der UPC-Code - mit dem UPC-Wert in einem vorhandenen übereinstimmt[!DNL Walmart Marketplace] Auflistung. Wenn ein Produkt übereinstimmt, wird das Commerce-Produktangebot der vorhandenen Walmart-Liste hinzugefügt.

   Überprüfen Sie die [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) Dashboard , um die aktualisierte Produktliste zu überprüfen und Produktdetails, Preise und Lagerbestände zu überprüfen.

* **[!UICONTROL Match - Match in Stage]**—Identifiziert Produkte, die übereinstimmen mit [!DNL Walmart] die erst veröffentlicht werden können, wenn die [!DNL Walmart Marketplace] Store ist live. Produkte mit diesem Status werden automatisch veröffentlicht, wenn die Variable [!DNL Walmart Marketplace] Store wird live geschaltet.

* **[!UICONTROL Error]**—Identifiziert Produkte, die nicht mit einem vorhandenen übereinstimmen [!DNL Walmart Marketplace] Auflistung.

* **[!UICONTROL Error description]**—Bietet detaillierte Informationen zum Listenfehler.

   Nachdem Sie den Fehler behoben haben, senden Sie das Produkt erneut zur Übereinstimmung. Siehe [Fehlerbehebung bei Produktübereinstimmungsfehlern](publish-listings-to-marketplace.md#troubleshoot-product-match-errors).
