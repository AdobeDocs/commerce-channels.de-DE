---
title: Protokolle und Berichte für Amazon-Listen speichern
description: Verwenden Sie die Protokolle und speichern Sie Berichte, um zu sehen, was in Ihrem Adobe Commerce- oder Magento Open Source-Store und in Ihren Amazon Marketplace-Listen passiert.
feature: Sales Channels, Logs
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Protokolle und Berichte für Amazon-Listen speichern

Die Amazon Sales Channel-Erweiterung enthält einige wertvolle Protokolle und Store-Berichte, mit denen Sie die Änderungen anzeigen können, die sich auf Ihre Amazon-Listen und -Bestellungen auswirken. Sie können diese Berichte verwenden, um zu sehen, was in Ihrem Store passiert, und um verschiedene Listenstatus zu verstehen.

Für die Protokolle oder Berichte sind keine Aktionen verfügbar, da sie schreibgeschützte Funktionen sind.

Der Zugriff auf die folgenden Protokolle erfolgt über das [Dashboard speichern](./amazon-store-dashboard.md).

- Das [Änderungsprotokoll zur Auflistung](./listing-changes-log.md) zeigt die Änderungen an, die in Ihrem Amazon-Vertriebskonto vorgenommen wurden, und spiegelt die Einstellungen Ihres Amazon-Vertriebskanals wider.

- Das [Kommunikationsfehlerprotokoll](./communication-errors-log.md) zeigt alle gemeldeten Kommunikationsfehler mit Amazon an.

Der Zugriff auf die folgenden speicherspezifischen Berichte erfolgt über das [Dashboard &quot;Speichern&quot;](./amazon-store-dashboard.md).

- Der Bericht zur [Wettbewerbsanalyse](./competitive-price-analysis.md) zeigt, dass Ihr Amazon _den Anlandepreis_ (Listenpreis plus Versandpreis) im Verhältnis zum Preis [Buy Box](./buy-box-competitor-pricing.md) und zum niedrigsten Preis des Konkurrenten](./lowest-competitor-pricing.md) hat.[

- Der Bericht [Listing-Verbesserungen](./listing-improvements.md) enthält alle vorgeschlagenen Listenerverbesserungen, die von Amazon für den ausgewählten Store bereitgestellt werden.

>[!TIP]
>
>Sie können die Protokolldatei auch auf zusätzliche Informationen überprüfen, wenn eine Fehlerbehebung erforderlich ist. Siehe [Admin-Einstellungen des Vertriebskanals](./sales-channel-settings.md). Die Protokollierung der Synchronisierung von Amazon-Verkaufskanälen wird in die Datei `{Commerce Root}/var/log/channel_amazon.log` geschrieben und kann im [Entwicklermodus](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes) angezeigt werden.
