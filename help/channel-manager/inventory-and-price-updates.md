---
title: Bestand- und Preisaktualisierungen
description: '"[!DNL Channel Manager] Synchronisiert Inventar- und Preisaktualisierungen zwischen dem Commerce Store und [!DNL Walmart Marketplace] damit Sie Ihre Vertriebskanalvorgänge von Ihrem Commerce-Administrator aus verwalten können."'
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Bestand- und Preisaktualisierungen

Der Kanal-Manager verfolgt Inventar und Preise für veröffentlichte Produkte und Synchronisierungsänderungen an den Channel Manager und den Walmart Marketplace, um aktuelle Lagermengen und Preise in Produktlisten widerzuspiegeln.**

## Inventaraktualisierungen

Wenn sich die Lagerbestände ändern, synchronisiert der Channel Manager Aktualisierungen zwischen dem Commerce-Produktkatalog und dem Walmart Marketplace, sodass sowohl der Channel Manager als auch der Walmart Marketplace die aktuelle Lagermenge anzeigen.

Es kann bis zu 5 Minuten dauern, bis Bestandsänderungen im Kanalmanager und Walmart Marketplace angezeigt werden.

* **Aktualisierungen der Lagermenge im Produktkatalog**-Wenn sich die Commerce-Lagermenge für ein Produkt ändert, das auf Walmart verkauft wird, weil [manuelle Bestandsmengenänderung](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html) oder eine Rückerstattung oder Stornierung einer Bestellung, synchronisiert der Channel Manager die Änderung mit dem verbundenen Vertriebskanal und der [!DNL Walmart Marketplace].

* **Reduzieren Sie die Lagermenge entsprechend den Bestellungen von Walmart Marketplace.**-Nachdem eine Walmart Marketplace-Auftragssynchronisierung an den Channel Manager durchgeführt wurde, sendet der Channel Manager die Aktualisierung an das Commerce-Bestellsystem. Der Handel passt die Lagermengen je nach Bestellung an. Anschließend wird die aktualisierte Menge mit dem Walmart Marketplace synchronisiert. kann es zu einigen Unterschieden in der Lagerbestandsmenge kommen, die im Kanalmanager und im Marketplace angezeigt werden, bis die Synchronisierungsvorgänge abgeschlossen sind.

>[!IMPORTANT]
>
> Nach der Synchronisation eines Walmart Marketplace-Auftrags mit dem Channel Manager werden Lagerbestände und andere Bestellinformationen nur für Rückerstattungen und Stornierungen aktualisiert, die von Commerce initiiert werden. Wenn eine Bestellung vom Walmart Marketplace zurückerstattet oder storniert wird, verarbeiten Sie die Änderung von Commerce, um sicherzustellen, dass die Lagerbestandsmengen und Bestellinformationen korrekt sind.

## Preisaktualisierungen

Wenn sich der Produktpreis in Commerce ändert, synchronisiert der Channel Manager die Aktualisierung vom Commerce-Produktkatalog mit dem Walmart Marketplace. Es kann bis zu 5 Minuten dauern, bis Bestandsänderungen angezeigt werden.

### Preise für ein veröffentlichtes Produkt verwalten

1. Aus dem [!UICONTROL Admin]auswählen **[!UICONTROL Catalog > Products]**.
1. Suchen Sie im Produktraster nach dem zu aktualisierenden Produkt und wählen Sie **[!UICONTROL Edit]**.
1. Überprüfen und aktualisieren Sie den Preis nach Bedarf.
1. **[!UICONTROL Save]** die Änderung.

Der Kanal-Manager synchronisiert alle Preisaktualisierungen mit dem Kanalspeicher und [!DNL Walmart Marketplace]. Dieser Vorgang kann bis zu 5 Minuten dauern.

Weitere Informationen zur Verwaltung der Produktpreiskonfiguration in Commerce finden Sie unter [Preise verwalten](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
