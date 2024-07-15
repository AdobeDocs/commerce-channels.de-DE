---
title: '[!DNL Channel Manager] Versionshinweise'
description: Die neuesten Versionsinformationen für [!DNL Channel Manager] aus Adobe Commerce.
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# [!DNL Channel Manager] Versionshinweise

Diese Versionshinweise beschreiben die erste Version von [!DNL Channel Manager] und umfassen:

![Neu](../assets/new.svg) Neue Funktionen
![Korrektur des Problems](../assets/fix.svg) Fehlerbehebungen und Verbesserungen
![Bekanntes Problem](../assets/bug.svg) Bekannte Probleme

Unter [Bevorstehende Versionen](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) erfahren Sie mehr über die Veröffentlichungszeitpläne und die Unterstützung.

Unter [Produktverfügbarkeit](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) erfahren Sie, welche Adobe Commerce-Versionen diese Erweiterung unterstützen.

## v2.1.0

*3. Oktober 2023*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg) Der Kanal-Manager ist jetzt mit den Versionen [Adobe Commerce Version 2.4.7 Beta](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html) kompatibel.

## v2.0.0

*20. März 2023*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg)<!--CHAN-5893--> Der Kanal-Manager ist jetzt mit Adobe Commerce-Version 2.4.6 kompatibel.

## v1.1.0

*23. November 2022*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg)<!--CHAN-5204--> **Rückgaben und Rückerstattungen**: Sie können jetzt die Rückgabe- und Rückgabeverfahren von Walmart Marketplace für Bestellungen verarbeiten, die über einen Adobe Commerce- und Magento Open Source Channel Manager-Store versandt werden. Informationen und Updates zu Rückgaben und Erstattungen werden zwischen Walmart und Adobe Commerce synchronisiert, sodass die aktuellen Daten sowohl in der [!DNL Commerce] Storefront als auch in [!DNL Walmart Marketplace] verfügbar sind. Siehe [Rückgabe und Rückerstattung von Bestellungen](return-refund-orders.md).

![Korrektur](../assets/fix.svg)<!--CHAN-5661--> Korrektur des `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` -Fehlers, der auftrat, wenn die Neusynchronisierung von Kanal-Manager die Anzeigereihenfolge von Daten mit dem Befehl `bin/magento saas:resync --feed orders` betraf. Der Fehler wurde behoben, indem die Package-Abhängigkeiten des Channel Manager-Moduls für das Sales Data Exporter-Modul aktualisiert wurden, das von `magento/module-sales-data-exporter` in `magento/module-sales-orders-data-exporter` umbenannt wurde.

## v1.0.0

*14. Januar 2022*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg) Erste Version des Kanal-Managers für die allgemeine Verfügbarkeit

