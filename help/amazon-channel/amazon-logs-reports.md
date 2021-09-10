---
title: Protokolle und Store-Berichte
description: Verwenden Sie die Protokolle und speichern Sie Berichte, um zu sehen, was in Ihrem Adobe Commerce- oder Magento Open Source-Store und in Ihren Amazon Marketplace-Listen passiert.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Protokolle und Berichte speichern

Die Amazon Sales Channel-Erweiterung enthält einige wertvolle Protokolle und Store-Berichte, mit denen Sie die Änderungen anzeigen können, die sich auf Ihre Amazon-Listen und -Bestellungen auswirken. Sie können diese Berichte verwenden, um zu sehen, was in Ihrem Store passiert, und um verschiedene Listenstatus zu verstehen.

Für die Protokolle oder Berichte sind keine Aktionen verfügbar, da sie schreibgeschützte Funktionen sind.

Die folgenden Protokolle können über das [Store-Dashboard](./amazon-store-dashboard.md) aufgerufen werden.

- Das [Protokoll zu Listing-Änderungen](./listing-changes-log.md) zeigt die Änderungen an, die in Ihrem Amazon-Vertriebskonto vorgenommen wurden, und spiegelt die Einstellungen Ihres Amazon-Vertriebskanals wider.

- Das [Kommunikationsfehlerprotokoll](./communication-errors-log.md) zeigt alle gemeldeten Kommunikationsfehler mit Amazon an.

Die folgenden speicherspezifischen Berichte können über das [Store-Dashboard](./amazon-store-dashboard.md) aufgerufen werden.

- Der Bericht [Konkurrenzpreisanalyse](./competitive-price-analysis.md) zeigt, dass Ihr Amazon _Landepreis_ (Listenpreis plus Versandpreis) im Verhältnis zum Preis [Buy Box](./buy-box-competitor-pricing.md) und zum niedrigsten Preis von Konkurrenten](./lowest-competitor-pricing.md) steht.[

- Der Bericht [Listening-Verbesserungen](./listing-improvements.md) enthält alle vorgeschlagenen Listenerweiterungen, die von Amazon für den ausgewählten Store bereitgestellt werden.

>[!TIP]
>
>Sie können die Protokolldatei auch auf zusätzliche Informationen überprüfen, wenn eine Fehlerbehebung erforderlich ist. Siehe [Vertriebskanal-Admin-Einstellungen](./sales-channel-settings.md). Die Protokollierung der Synchronisation von Amazon-Verkaufskanälen wird in die Datei `{Commerce Root}/var/log/channel_amazon.log` geschrieben und kann im [Entwicklermodus](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;} angezeigt werden.
