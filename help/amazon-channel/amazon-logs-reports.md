---
title: Protokolle und Store-Berichte
description: Verwenden Sie die Protokolle und speichern Sie Berichte, um zu sehen, was in Ihrem Adobe Commerce- oder Magento Open Source-Store und in Ihren Amazon Marketplace-Listen passiert.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Protokolle und Store-Berichte

Die Amazon Sales Channel-Erweiterung enthält einige wertvolle Protokolle und Store-Berichte, mit denen Sie die Änderungen anzeigen können, die sich auf Ihre Amazon-Listen und -Bestellungen auswirken. Sie können diese Berichte verwenden, um zu sehen, was in Ihrem Store passiert, und um verschiedene Listenstatus zu verstehen.

Für die Protokolle oder Berichte sind keine Aktionen verfügbar, da sie schreibgeschützte Funktionen sind.

Die folgenden Protokolle sind über die [Store-Dashboard](./amazon-store-dashboard.md).

- Die [Protokoll zu Listungsänderungen](./listing-changes-log.md) zeigt die Änderungen an, die in Ihrem Amazon-Vertriebskonto vorgenommen wurden, in Anlehnung an Ihre Amazon-Vertriebskanaleinstellungen.

- Die [Kommunikationsprotokoll](./communication-errors-log.md) zeigt alle gemeldeten Kommunikationsfehler mit Amazon an.

Die folgenden speicherspezifischen Berichte sind über die [Store-Dashboard](./amazon-store-dashboard.md).

- Die [Preisanalyse für Wettbewerber](./competitive-price-analysis.md) zeigt, dass Ihr Amazon _Anlandepreis_ (Börsenkurs plus Versandpreis) im Verhältnis zum [Buy Box](./buy-box-competitor-pricing.md) Preis und [kleinster Konkurrent](./lowest-competitor-pricing.md) Preis.

- Die [Verbesserungen bei Listen](./listing-improvements.md) zeigt alle vorgeschlagenen Verbesserungen an, die von Amazon für den ausgewählten Store bereitgestellt werden.

>[!TIP]
>
>Sie können die Protokolldatei auch auf zusätzliche Informationen überprüfen, wenn eine Fehlerbehebung erforderlich ist. Siehe [Admin-Einstellungen für Vertriebskanäle](./sales-channel-settings.md). Die Protokollierung der Synchronisierung der Amazon-Verkaufskanäle wird in `{Commerce Root}/var/log/channel_amazon.log` Datei und kann in [Entwicklermodus](https://docs.magento.com/user-guide/magento/installation-modes.html){target="_blank"}.
