---
title: '[!DNLChannel Manager] - Versionshinweise'
description: "Die neuesten Versionsinformationen für [!DNL Channel Manager] von Adobe Commerce."
source-git-commit: 501a76a126f090805f95e64078ec2c73de003aa4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 2%

---

# [!DNL Channel Manager] Versionshinweise

Diese Versionshinweise beschreiben die erste Version von [!DNL Channel Manager] und umfassen:

![Neu](../assets/new.svg) Neue Funktionen
![Problem behoben](../assets/fix.svg) Fehlerbehebungen und Verbesserungen
![Bekanntes Problem](../assets/bug.svg) Bekannte Probleme


## v1.1.0

![Neu](../assets/new.svg)<!--CHAN-5204--> **Rückgaben und Erstattungen**- Sie können jetzt die Rückgabe- und Erstattungsverfahren von Walmart Marketplace für Bestellungen verarbeiten, die über einen Adobe Commerce- und Magento Open Source Channel Manager-Store versandt werden. Informationen und Aktualisierungen über Rückgaben und Erstattungen werden zwischen Walmart und Adobe Commerce synchronisiert, sodass die aktuellen Daten in beiden [!DNL Commerce] Storefront und [!DNL Walmart Marketplace]. Siehe [Rückgabe- und Erstattungsanordnungen](return-refund-orders.md).

![Fest](../assets/fix.svg)<!--CHAN-5661--> Die `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` Fehler, der bei der erneuten Synchronisierung der Kanalmanager auftrat, um Daten mithilfe der `bin/magento saas:resync --feed orders` Befehl. Der Fehler wurde behoben, indem die Package-Abhängigkeiten des Channel Manager für das Sales Data Exporter-Modul aktualisiert wurden, das in `magento/module-sales-data-exporter` nach `magento/module-sales-orders-data-exporter`.

## v1.0.0

Erste Version, kompatibel mit den folgenden Commerce-Versionen:

* Open Source (CE): 2.4.x
* Adobe Commerce (EE): 2.4.x
* Adobe Commerce for Cloud (ECE): 2.4.x
* Stabilität: Stabil
