---
title: Bestand- und Preisaktualisierungen
description: '''[!DNL Channel Manager] Synchronisiert Inventar- und Preisaktualisierungen zwischen dem Commerce Store und [!DNL Walmart Marketplace] damit Sie Ihre Vertriebskanalvorgänge von Ihrem Commerce-Administrator aus verwalten können.'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: a1944052f02968c36495275cd5ddfb2ca43ce967
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Bestand- und Preisaktualisierungen

[!DNL Channel Manager] erfasst Inventar und Preise für Produkte im Kanalspeicher. Wenn sich Inventar- oder Preisänderungen ändern, werden Aktualisierungen mit beiden synchronisiert [!DNL Channel Manager] und [!DNL Walmart Marketplace] , um die aktuelle Lagermenge und die Preise in Produktlisten widerzuspiegeln.

## Inventaraktualisierungen

Wenn sich die Lagerbestände ändern, synchronisiert der Channel Manager Aktualisierungen zwischen Commerce und Walmart Marketplace, um sicherzustellen, dass der Channel Manager und der Walmart Marketplace über die richtige Lagermenge verfügen.

Es kann bis zu 10 Minuten dauern, bis Bestandsaktualisierungen über den Kanal-Manager und den Marketplace hinweg synchronisiert werden.

* **Aktualisierungen der Lagermenge im Produktkatalog**-Wenn sich die Commerce-Lagermenge aufgrund von [manuelle Änderungen der Lagermenge](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html), Erstattungen oder Abbrüche synchronisiert der Kanalmanager die Änderung mit verbundenen Kanälen und [!DNL Walmart Marketplace].

* **Reduzieren Sie die Lagermenge entsprechend den Bestellungen von Walmart Marketplace.**-Nachdem eine Walmart Marketplace-Auftragssynchronisierung an den Channel Manager durchgeführt wurde, sendet der Channel Manager die Aktualisierung an das Commerce-Bestellsystem. Der Handel passt die Lagermengen je nach Bestellung an. Anschließend wird die aktualisierte Menge mit dem Walmart Marketplace synchronisiert. Bis die Synchronisierungsvorgänge abgeschlossen sind, kann es zu Mengenunterschieden zwischen dem Kanal-Manager und dem Marketplace kommen.

>[!IMPORTANT]
>
> Nach der Synchronisation eines Walmart Marketplace-Auftrags mit dem Channel Manager werden Lagerbestände und Bestellinformationen nur für Rückerstattungen und Stornierungen aktualisiert, die von Commerce initiiert werden. Wenn eine Bestellung vom Walmart Marketplace rückerstattet oder storniert wird, verarbeiten Sie die Änderung von Commerce, um die Genauigkeit der Commerce-Lagermengen und Bestellinformationen zu gewährleisten.

## Preisaktualisierungen

Wenn sich der Produktpreis in Commerce ändert, synchronisiert der Channel Manager die Aktualisierung aus dem [!DNL Commerce] Produktkatalog [!DNL Walmart Marketplace]. Es kann bis zu fünf Minuten dauern, bis der Marketplace die Preisänderungen anzeigt.

### Preise für ein veröffentlichtes Produkt verwalten

1. Aus dem [!UICONTROL Admin]auswählen **[!UICONTROL Catalog > Products]**.
1. Suchen Sie im Produktraster nach dem zu aktualisierenden Produkt und wählen Sie **[!UICONTROL Edit]**.
1. Überprüfen und aktualisieren Sie den Preis nach Bedarf.
1. **[!UICONTROL Save]** die Änderung.

Weitere Informationen zur Verwaltung der Produktpreiskonfiguration in Commerce finden Sie unter [Preise verwalten](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
