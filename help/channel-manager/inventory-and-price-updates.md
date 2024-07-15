---
title: Bestand- und Preisaktualisierungen
description: '"[!DNL Channel Manager]" synchronisiert Bestandsaktualisierungen und Preisaktualisierungen zwischen dem [!DNL Commerce] Speicher und  [!DNL Walmart Marketplace] , sodass Sie Ihre Vertriebskanalvorgänge über den  [!DNL Commerce] Admin verwalten können.'
feature: Sales Channels, Merchandising, Inventory, Tools and External Services
role: Leader, Admin, User
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Inventar und Preise aktualisieren

[!DNL Channel Manager] verfolgt Inventar und Preise für Produkte im Produktkatalog von [!DNL Commerce] und synchronisiert Aktualisierungen mit dem verbundenen Absatzkanal und [!DNL Walmart Marketplace]. Der Synchronisierungsvorgang stellt sicher, dass die Produktlisten die aktuelle Lagermenge und -preisstruktur widerspiegeln.


>[!IMPORTANT]
>
>Nachdem [!DNL Channel Manager] installiert und konfiguriert wurde, werden alle Bestands-, Preis- und Bestellaktualisierungen automatisch synchronisiert. Wenn Sie bereits auf Walmart Marketplace verkaufen, deaktivieren Sie alle anderen Integrationen, die das Produkt und die Bestelldaten aktualisieren. Überprüfen Sie dann, ob die Lagerbestände und -preise in der [!DNL Commerce] -Storefront korrekt sind und mit den Daten in [!DNL Walmart Marketplace] übereinstimmen, bevor Sie [!DNL Channel Manager] mit dem Live-Marketplace-Store verbinden.


## Inventaraktualisierungen

Wenn sich die Bestandsebenen des Produkts in [!DNL Commerce] ändern, synchronisiert [!DNL Channel Manager] Aktualisierungen in die [!DNL Walmart Marketplace]. Es kann bis zu 10 Minuten dauern, bis Bestandsaktualisierungen über den Vertriebskanal hinweg mit dem [!DNL Walmart marketplace] synchronisiert werden.

* **Aktualisierungen der Lagermenge im Produktkatalog**—Wenn sich [!DNL Commerce] die Lagermenge aufgrund von [manuellen Bestandsmengenänderungen](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html), Erstattungen oder Stornierungen ändert, synchronisiert [!DNL Channel Manager] die Änderung mit den verbundenen Kanälen und [!DNL Walmart Marketplace].

* **Reduzieren Sie die Lagermenge entsprechend [!DNL Walmart Marketplace] Bestellungen**—Nachdem eine [!DNL Walmart Marketplace] Bestellung mit [!DNL Channel Manager] synchronisiert wurde, sendet [!DNL Channel Manager] die Aktualisierung an das [!DNL Commerce] Bestellsystem. [!DNL Commerce] passt die Lagermengen auf Grundlage der Bestellung an. Anschließend wird die aktualisierte Menge mit [!DNL Walmart Marketplace] synchronisiert. Bis die Synchronisierungsvorgänge abgeschlossen sind, werden in den Vertriebskanallisten möglicherweise unterschiedliche Mengen und [!DNL Walmart] angezeigt.

>[!IMPORTANT]
>
>Nach einer [!DNL Walmart Marketplace]-Auftragssynchronisation mit [!DNL Channel Manager] werden Lagermengen und Bestellinformationen nur für Erstattungen und Stornierungen aktualisiert, die von [!DNL Commerce] eingeleitet wurden. Wenn eine Bestellung vom [!DNL Walmart marketplace] zurückerstattet oder storniert wird, verarbeiten Sie die Änderung von [!DNL Commerce], um die Genauigkeit von [!DNL Commerce] Lagerbestandsmengen und Bestellinformationen sicherzustellen.

## Preisaktualisierungen

Wenn sich der Produktpreis in [!DNL Commerce] ändert, synchronisiert [!DNL Channel Manager] die Aktualisierung mit [!DNL Walmart Marketplace]. Es kann bis zu fünf Minuten dauern, bis die Preisänderung in der Liste [!DNL Walmart Marketplace] angezeigt wird.

### Preise für verbundene Produkte verwalten

1. Wählen Sie [!UICONTROL Admin] aus.**[!UICONTROL Catalog > Products]**
1. Suchen Sie im Produktraster nach dem zu aktualisierenden Produkt und wählen Sie **[!UICONTROL Edit]** aus.
1. Überprüfen und aktualisieren Sie den Preis nach Bedarf.
1. **[!UICONTROL Save]** die Änderung.

Hilfe zur Verwaltung der Produktpreiskonfiguration in [!DNL Commerce] finden Sie unter [Preise verwalten](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html).
