---
title: Listen verwalten
description: Verwalten von Verkaufskanallisten für eine [!DNL Commerce] mit dem Kanal-Manager für Adobe Commerce und Magento Open Source speichern.
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 30495c4e47f15c821206f7b0252b868b4e27d62d
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Verwalten von Listen

Produktlisten für einen verbundenen Kanal verwalten aus [!UICONTROL Listings] in der Kanalspeicheransicht.

Verwenden Sie die *[!UICONTROL Listings]* Arbeitsbereich zum Verwalten der [!DNL Commerce] Produkte, die auf dem Walmart Marketplace zum Verkauf angeboten werden. Der Status für eine einzelne Auflistung zeigt an, wo sich das Produkt im [!DNL Channel Manager] -Workflow, damit Sie die nächsten Schritte bestimmen und etwaige Fehler beheben können.

![Listenseite für einen verbundenen Vertriebskanal](assets/products-submit-for-matching.png)

## Anzeigen von Listen

1. Navigieren Sie vom Administrator zu [!UICONTROL **Marketing** > Kanäle > **Kanal-Manager**].

1. Wählen Sie in der Liste &quot;Channel Store&quot;das Stiftsymbol in einer Store-Einstiegszeile aus, um die Store-Ansicht zu öffnen.

1. Auswählen [!UICONTROL **Auflistungen**].

## Hinzufügen von Commerce-Produkten zum Kanal-Manager

Führen Sie die folgenden Aufgaben aus, um das Produktsortiment für den Kanal Walmart Marketplace zu erstellen:

* [Hinzufügen von Produkten aus Ihrem Commerce-Produktkatalog zum Channel Manager](add-products-to-connected-channel.md)

* [Produktabgleich konfigurieren](map-product-attributes-for-matching.md#configure-product-attribute-settings)

## Produkte in Walmart veröffentlichen

Sie können Produktangebote im Walmart Marketplace erstellen, indem Sie Produktabgleiche verwenden oder Produktlisten für neue Produkte manuell hochladen. Anweisungen finden Sie unter [Veröffentlichen von Listen in Walmart Marketplace](publish-listings-to-marketplace.md) wie in den folgenden Themen beschrieben:

* **[Produkte bei Walmart abgleichen](publish-listings-to-marketplace.md)**- Veröffentlichen Sie Produktlisten von Ihrem Kanal in [!DNL Walmart Marketplace] durch Aktualisierung bestehender Listen, die dasselbe Produkt verkaufen. Übereinstimmungskriterien werden durch die [Konfiguration der Attributzuordnung](map-product-attributes-for-matching.md) für Ihren Kanal.

* **[Manuelles Hochladen neuer Listen](publish-listings-to-marketplace.md#upload-new-product-listings)-**-Verwenden Sie für Produkte, die nicht mit einer vorhandenen Liste auf dem Walmart Marketplace übereinstimmen, eine Excel-Vorlage der Walmart-Produktkategorie, um Produktlisten stapelweise hochzuladen.

## Listen-Steuerelemente und Feldbeschreibungen

Die folgenden Tabellen beschreiben die Steuerelemente und Felder, die im [!UICONTROL Listings] Seite.

**Steuerelemente für[!UICONTROL Listings]**

| **Attribut** | **Anforderungsstufe** |
|----------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Refresh products] | Aktualisiert die Anzeige mit der aktuellsten Liste und dem aktuellen Status |
| [!UICONTROL Add Products ] | Öffnet die [!UICONTROL  Admin Product Catalog] Seite zum Auswählen der Produkte, die Sie zu Ihrem [!DNL Walmart Marketplace] Sortierung oder Aktualisierung von Produktattributen, um die Anforderungen an die Auflistung von Walmart Marketplace zu erfüllen. |
| [!UICONTROL Match products on Walmart] | Nachdem Sie ein oder mehrere Produkte im Status Entwurf ausgewählt haben, wählen Sie [!UICONTROL Match products on Walmart] , um nach Produktangeboten zu suchen, die einem vorhandenen hinzugefügt werden können [!DNL Walmart Marketplace] Auflistung. |


**Spaltenbeschreibungen**

| **Feld** | **Beschreibung** |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | Name des Produkts aus der [!DNL Commerce] Katalog speichern. |
| [!UICONTROL SKU (Unique ID)] | Das zugeordnete Attribut, das zum Abgleichen von Produkten auf dem Marketplace verwendet wird. Dieser Feldname hängt von der zugeordneten Attributkonfiguration für [!DNL Channel Manager] Auflistungen. In diesem Fall verwendet der Produktabgleichsvorgang die Produkt-SKU aus der [!DNL Commerce] Katalog zum Auffinden einer [!DNL Walmart Marketplace]  Liste mit einem SKU-Wert, der dem SKU-Wert aus den Commerce-Produktattributen entspricht. |
| [!UICONTROL  Quantity] | Umfang des in Adobe Commerce oder Magento Open Source verfügbaren Bestands. |
| [!UICONTROL Price] | Der Produktpreis aus dem [!DNL Commerce] Katalog speichern. Aktualisierungen des Katalogpreises werden mit dem Kanal-Manager synchronisiert und dann an [!DNL Walmart Marketplace]  sodass die aufgelisteten Artikel den aktuellen Preis anzeigen. |
| [!UICONTROL Status] | Gibt den aktuellen Bestellstatus im [!DNL Commerce] Bestellworkflow. Der Status wird aktualisiert, wenn Sie erfolgreich Produkte zu [!DNL Channel Manager] und wenn Sie Produkte auf dem Markt finden. Wenn ein Vorgang fehlschlägt, wird in der Liste der Fehlerstatus angezeigt. Nachdem Sie den Fehler behoben haben, [!DNL Channel Manager] wiederholt den Vorgang und aktualisiert den Status. |


### Über den Listenstand

Im Arbeitsbereich &quot;Listen&quot;zeigt die Bezeichnung Status an, wo sich ein Produkt im [!DNL Channel Manager] -Arbeitsablauf, damit Sie die nächsten Schritte bestimmen und Fehler beheben können. Listen können die folgenden Statusbezeichnungen aufweisen:

* **[!UICONTROL Draft]**- Identifiziert nicht vorhandene Produkte [eingereicht [!DNL Walmart] für Abgleich](publish-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**-Identifiziert Produkte, die zum Abgleich auf der [!DNL Walmart Marketplace]. Produkte verbleiben in *Verarbeitung* bis zum [!DNL Walmart] gibt eine HTTP-Statusmeldung zurück, die angibt, ob die Übereinstimmung erfolgreich war oder ob ein Fehler aufgetreten ist. Es kann bis zu 30 Minuten dauern, bis der Match-Vorgang am [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**- Identifiziert Produkte, die erfolgreich zugewiesen wurden unter [!DNL Walmart].

   Eine Übereinstimmung tritt auf, wenn der Produktattribut value-UPC-Code beispielsweise mit dem UPC-Wert in einem vorhandenen[!DNL Walmart Marketplace] Auflistung. Wenn ein Produkt übereinstimmt, wird das Commerce-Produktangebot der vorhandenen Walmart-Liste hinzugefügt.

   Überprüfen Sie die [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) Dashboard , um die aktualisierte Produktliste zu überprüfen und Produktdetails, Preise und Lagerbestände zu überprüfen.


* **[!UICONTROL Error]**- Identifiziert Produkte, die nicht mit einem vorhandenen übereinstimmen [!DNL Walmart Marketplace] Auflistung. Anzeigen von Fehlerdetails durch Bewegen des Mauszeigers über die *Fehler* Statusbezeichnung.

   Nachdem Sie den Fehler behoben haben, senden Sie das Produkt erneut zur Übereinstimmung. Siehe [Fehlerbehebung bei Produktübereinstimmungsfehlern](https://docs.google.com/document/d/1bEbCyVLXJQQsbZvEwetJvZKWQJOKoiw5Ia1uB4Bs4uo/edit#heading=h.sz6eji8z9vzy).

* **[!UICONTROL Error - Match in Stage]**-Identifiziert Produkte, die übereinstimmen mit [!DNL Walmart] die erst veröffentlicht werden können, wenn die [!DNL Walmart Marketplace] Store ist live. Produkte mit diesem Status werden automatisch veröffentlicht, wenn die Variable [!DNL Walmart Marketplace] Store wird live geschaltet.
