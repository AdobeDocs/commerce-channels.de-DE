---
title: Bestand- und Preisaktualisierungen
description: '[!DNL Channel Manager] Synchronisiert Inventar- und Preisaktualisierungen zwischen [!DNL Commerce] speichern und [!DNL Walmart Marketplace] damit Sie Ihre Vertriebskanalvorgänge über die [!DNL Commerce] Admin'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Inventar und Preise aktualisieren

[!DNL Channel Manager] erfasst Inventar und Preise für Produkte in [!DNL Commerce] Produktkatalog und synchronisiert Aktualisierungen mit dem verbundenen Vertriebskanal und [!DNL Walmart Marketplace]. Der Synchronisierungsvorgang stellt sicher, dass die Produktlisten die aktuelle Lagermenge und -preisstruktur widerspiegeln.


>[!IMPORTANT]
>
>Nachher [!DNL Channel Manager] installiert und konfiguriert ist, werden alle Inventar-, Preis- und Bestellaktualisierungen automatisch synchronisiert. Wenn Sie bereits auf Walmart Marketplace verkaufen, deaktivieren Sie alle anderen Integrationen, die das Produkt und die Bestelldaten aktualisieren. Überprüfen Sie dann, ob Lagerbestände und -preise in der Variablen [!DNL Commerce] storefront sind genau und stimmen mit den Daten in [!DNL Walmart Marketplace] bevor Sie eine Verbindung herstellen [!DNL Channel Manager] in den Live-Marketplace-Store.


## Inventaraktualisierungen

Wenn sich die Produktinventarisierung ändert [!DNL Commerce], [!DNL Channel Manager] synchronisiert Aktualisierungen für [!DNL Walmart Marketplace]. Es kann bis zu 10 Minuten dauern, bis Bestandsaktualisierungen über den Vertriebskanal hinweg mit dem [!DNL Walmart marketplace].

* **Aktualisierungen der Lagermenge im Produktkatalog**—When [!DNL Commerce] Änderungen der Lagermenge aufgrund von [manuelle Änderungen der Lagermenge](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html), Erstattungen oder Annullierungen, [!DNL Channel Manager] Synchronisiert die Änderung mit verbundenen Kanälen und [!DNL Walmart Marketplace].

* **Die Lagermenge entsprechend reduzieren [!DNL Walmart Marketplace] Bestellungen**—Nach einem [!DNL Walmart Marketplace] Synchronisierungsaufträge an [!DNL Channel Manager], [!DNL Channel Manager] sendet das Update an die [!DNL Commerce] Bestellsystem. [!DNL Commerce] passt die Lagermengen auf der Basis der Bestellung an. Anschließend wird die aktualisierte Menge mit [!DNL Walmart Marketplace]. Bis die Synchronisierungsvorgänge abgeschlossen sind, werden in den Vertriebskanallisten möglicherweise unterschiedliche Mengen angezeigt und [!DNL Walmart].

>[!IMPORTANT]
>
>Nach [!DNL Walmart Marketplace] Synchronisierungsaufträge an [!DNL Channel Manager], die Lagermengen und die Bestellinformationen werden nur für Erstattungen und Annullierungen aktualisiert, die von [!DNL Commerce]. Wenn eine Bestellung rückerstattet oder von der [!DNL Walmart marketplace], verarbeiten Sie die Änderung von [!DNL Commerce] die Richtigkeit der [!DNL Commerce] Lagermengen und Bestellinformationen.

## Preisaktualisierungen

Wenn sich der Produktpreis in [!DNL Commerce], [!DNL Channel Manager] synchronisiert die Aktualisierung mit dem [!DNL Walmart Marketplace]. Es kann bis zu fünf Minuten dauern, bis die Preisänderung im [!DNL Walmart Marketplace] Auflistung.

### Preise für verbundene Produkte verwalten

1. Aus dem [!UICONTROL Admin]auswählen **[!UICONTROL Catalog > Products]**.
1. Suchen Sie im Produktraster nach dem zu aktualisierenden Produkt und wählen Sie **[!UICONTROL Edit]**.
1. Überprüfen und aktualisieren Sie den Preis nach Bedarf.
1. **[!UICONTROL Save]** die Änderung.

Hilfe zur Verwaltung der Produktpreiskonfiguration finden Sie unter [!DNL Commerce], siehe [Preise verwalten](https://docs.magento.com/user-guide/catalog/pricing.html){target="_blank"}.
