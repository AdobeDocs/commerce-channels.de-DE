---
title: '[!DNL Channel Manager] Versionshinweise'
description: Die neuesten Versionshinweise für [!DNL Channel Manager] aus Adobe Commerce.
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 3%

---

# [!DNL Channel Manager] Versionshinweise

Diese Versionshinweise beschreiben die erste Version von [!DNL Channel Manager] und umfassen:

![Neu](../assets/new.svg) Neue Funktionen
![Problem behoben](../assets/fix.svg) Fehlerbehebungen und Verbesserungen
![Bekanntes Problem](../assets/bug.svg) Bekannte Probleme

Siehe [Bevorstehende Versionen](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) , um mehr über die Veröffentlichungszeitpläne und die Unterstützung zu erfahren.

Siehe [Produktverfügbarkeit](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) , um zu erfahren, welche Adobe Commerce-Versionen diese Erweiterung unterstützen.

## v2.1.0

*3. Oktober 2023*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg) Der Kanal-Manager ist jetzt mit [Beta-Version 2.4.7 von Adobe Commerce](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html) veröffentlicht.

## v2.0.0

*20. März 2023*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg)<!--CHAN-5893--> Der Kanal-Manager ist jetzt mit Adobe Commerce-Version 2.4.6 kompatibel.

## v1.1.0

*23. November 2022*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg)<!--CHAN-5204--> **Rückgaben und Erstattungen**- Sie können jetzt die Rückgabe- und Erstattungsverfahren von Walmart Marketplace für Bestellungen verarbeiten, die über einen Adobe Commerce- und Magento Open Source Channel Manager-Store versandt werden. Informationen und Aktualisierungen über Rückgaben und Erstattungen werden zwischen Walmart und Adobe Commerce synchronisiert, sodass die aktuellen Daten in beiden [!DNL Commerce] Storefront und [!DNL Walmart Marketplace]. Siehe [Rückgabe- und Erstattungsanordnungen](return-refund-orders.md).

![Fest](../assets/fix.svg)<!--CHAN-5661--> Die `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` Fehler, der bei der erneuten Synchronisierung der Kanalmanager auftrat, um Daten mithilfe der `bin/magento saas:resync --feed orders` Befehl. Der Fehler wurde behoben, indem die Package-Abhängigkeiten des Channel Manager für das Sales Data Exporter-Modul aktualisiert wurden, das in `magento/module-sales-data-exporter` nach `magento/module-sales-orders-data-exporter`.

## v1.0.0

*14. Januar 2022*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg) Erste Version von Channel Manager für allgemeine Verfügbarkeit

