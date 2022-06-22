---
title: '"Info [!DNL Channel Manager]'''
description: '"Erfahren Sie, wie Sie installieren und verwenden [!DNL Channel Manager] , um Adobe Commerce- und Magento Open Source-Stores mit Drittanbieter-Marktplätzen zu integrieren und einen Vertriebskanal zu erstellen, über den Sie Marktplatzierungen, -preise, -inventare und -verkäufe nahtlos über Ihren Commerce-Administrator verwalten können."'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 8146be1c94ffb1c8abd0d28e53d3476fd78f2c62
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---


# Info [!DNL Channel Manager]

[!DNL Channel Manager] hilft Händlern, den Umsatz zu steigern, neue Kunden zu erreichen, Vertriebsvorgänge zu optimieren und Zeit zu sparen, indem ein Adobe Commerce- oder Magento Open Source-Produktkatalog in die [!DNL Walmart Marketplace].

![[!DNL Channel Manager] Admin-Ansicht der Erweiterung](assets/channel-manager-home.png)

[!DNL Channel Manager] unterstützt Adobe Commerce- oder Magento Open Source-Händler, die verkaufen möchten [!DNL Walmart Marketplace] durch Erweiterung der [!DNL Commerce] Admin. Mit [!DNL Channel Manager] installierte, gespeicherte Administratoren und Betriebspersonal können [!DNL Walmart Marketplace] Verkaufs-, Bestands- und Produktpreise nahtlos aus der Commerce-Umgebung heraus.

Der erweiterte Admin optimiert Vorgänge, da Händler dieselben Workflows und Prozesse zur Verwaltung von Verkäufen aus beiden verwenden können [!DNL Commerce] Storefronts und der Walmart Marketplace.

Nach der Installation und Konfiguration [!DNL Channel Manager]können Sie die folgenden Funktionen verwenden, um Walmart Marketplace-Verkaufsaufträge zu verwalten:

* **Listenverwaltung**-Einfache Verbindung von Produktlisten durch passende Produkte aus Ihrer [!DNL Commerce] Katalog zu existieren [!DNL Walmart Marketplace] Auflistungen.

* **Inventory management**-Elemente im Marktplatzierungskonto des Händlers werden automatisch synchronisiert und aktualisiert von [!DNL Commerce] zur Gewährleistung genauer Lagerbestände.

* **Preisaktualisierungen**- Erhalten Sie genaue Preise für Marktplatzierungen mit automatischer Preissynchronisierung. Wenn sich ein Preis in Adobe Commerce ändert, werden die Änderungen auf dem Markt übernommen.

* **Auftragsverwaltung**-Wenn neue Bestellungen auf einem Markt erstellt werden, [!DNL Channel Manager] Synchronisiert Bestellungen mit Adobe Commerce und sendet Bestellbestätigungen an den Marketplace. Diese Bestätigung stellt sicher, dass der Bestand für jede Bestellung reserviert ist. Der letzte Schritt besteht darin, die entsprechenden Bestellungen im [!DNL Commerce] Auftragsverwaltungssystem für die Verarbeitung.

* **Versandmanagement**-Wenn Bestellungen als in Adobe Commerce versandt gekennzeichnet sind, wird die Versandaktualisierung an die [!DNL Walmart Marketplace]. Diese Benachrichtigung stellt sicher, dass die Verkäufer ihre SLA-Anforderungen erfüllen und dass Kunden Versandaktualisierungen für ihre aktuellen Bestellungen erhalten.

* **Stornierungen**-Wenn Bestellungen in Adobe Commerce storniert werden, [!DNL Channel Manager] sendet aktualisierte Bestellinformationen an den Marketplace, um die Aktion für die entsprechende Marketplace-Bestellung zu replizieren. Nach Abschluss der Auftragsstornierung wird die [!DNL Commerce] Bestandsmengenaktualisierungen, die die zurückgegebenen Elemente widerspiegeln, und Bestandsaktualisierungen werden automatisch mit synchronisiert. [!DNL Walmart Marketplace].

## Erwartete Latenz für [!DNL Channel Manager] Vorgänge

Die Datensynchronisation zwischen [!DNL Channel Manager] und [!DNL Walmart Marketplace] -Store benötigt etwas Zeit, um abzuschließen. Überprüfen Sie die erwartete Verarbeitungszeit für [!DNL Channel Manager] Operationen, die die Planung des Betriebs von Vertriebskanälen erleichtern.

**Geschätzte Latenz für [!DNL Channel Manager] Vorgänge**

| **Vorgang** | **Beschreibung** | **Erwartete Verzögerung** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| Hinzufügen von Produkten zu [!DNL Channel Manager] | Wählen Sie Produkte aus dem [!DNL Commerce] Produktkatalog und importieren Sie sie in [!DNL Channel Manager]. | **Bis zu fünf Minuten**-Wenn Sie viele Produkte auswählen, z. B. einen gesamten Produktkatalog, dauert der Importvorgang länger. |
| Produkte abgleichen auf [!DNL Walmart Marketplace] | Produktlisten auswählen in [!DNL Channel Manager] und senden Sie an Walmart zur Zuordnung. | **Bis zu 30 Minuten**-Wenn Sie viele Produkte auswählen, dauert der passende Prozess je nach ausgewählter Menge länger. |
| Inventaraktualisierungen | Wenn sich die Lagerbestandsmenge in Commerce ändert, [!DNL Channel Manager] synchronisiert die Aktualisierung mit Walmart. | **Bis zu 10 Minuten** |
| Preisaktualisierungen | Wenn sich ein Produktpreis ändert, [!DNL Channel Manager] synchronisiert die Aktualisierung mit Walmart. | **Bis zu fünf Minuten** |
| Sortierreihenfolge von Walmart an [!DNL Commerce] | Kundenaufträge a [!DNL Commerce] Produkt auf dem Walmart Marketplace. Walmart sendet den Auftrag an [!DNL Channel Manager]. Die Reihenfolge wird im Bestell-Dashboard angezeigt. | **Bis zu 30 Minuten** |
| In der Reihenfolge erstellt [!DNL Commerce] Auftragsverwaltung | [!DNL Channel Manager] erstellt die [!DNL Commerce] Bestellung über die Walmart-Bestellung und aktualisiert das Bestell-Dashboard, um die [!DNL Commerce] Bestellnummer. | **Bis zu fünf Minuten** |
| Aktualisierung des Versandstatus in [!DNL Commerce] Auftragsverwaltung | Wenn eine Bestellung aus dem Handel versandt wird, [!DNL Channel Manager] aktualisiert den Versandstatus im Bestell-Dashboard und sendet das Update an den Walmart Marketplace, damit der Kunde benachrichtigt werden kann. | **Bis zu fünf Minuten** |
| Aktualisierung der Auftragsstornierung in der Commerce Order Management | Wenn eine Bestellung aus dem Handel abgebrochen wird, [!DNL Channel Manager] aktualisiert den Bestellstatus im Bestell-Dashboard und sendet das Update an Walmart Marketplace, damit der Kunde benachrichtigt werden kann. Nach Abschluss der Auftragsstornierung wird die [!DNL Commerce] Bestandsmengenaktualisierungen, um die zurückgegebenen Elemente widerzuspiegeln. Dann [!DNL Channel Manager] synchronisiert die Aktualisierung mit dem [!DNL Walmart Marketplace]. | **Bis zu fünf Minuten** |


