---
title: Protokolle und Berichte speichern
description: Verwenden Sie die Protokolle und speichern Sie Berichte, um zu sehen, was in Ihrem Adobe Commerce- oder Magento Open Source-Store und in Ihren Amazon Marketplace-Listen geschieht.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Protokolle und Berichte speichern

Die Amazon Sales Kanal-Erweiterung beinhaltet einige wertvolle Protokolle und speichert Berichte, mit denen Sie die Änderungen, die Ihre Amazon-Auflistungen und -Bestellungen betreffen, Ansicht haben. Sie können diese Berichte verwenden, um zu sehen, was in Ihrem Geschäft passiert, und um verschiedene Listenstatus zu verstehen.

Für die Protokolle oder speichern Sie Berichte keine Aktionen, da es sich um reine Rezensionsfunktionen handelt.

Auf die folgenden Protokolle kann zugegriffen werden über [Dashboard speichern](./amazon-store-dashboard.md).

- Die [Änderungsprotokoll auflisten](./listing-changes-log.md) zeigt die Änderungen an Ihrem Amazon Seller-Konto an, die sich aus Ihren Amazon Sales Kanal-Einstellungen ergeben haben.

- Die [Kommunikationsprotokoll](./communication-errors-log.md) zeigt alle gemeldeten Kommunikationsfehler mit Amazon an.

Auf die folgenden speicherspezifischen Berichte können Sie über die [Dashboard speichern](./amazon-store-dashboard.md).

- Die [Analyse der Wettbewerbspreise](./competitive-price-analysis.md) Bericht zeigt, dass Ihr Amazon _Anlandepreis_ (Listenpreis plus Versandpreis) in Bezug auf [Buy Box](./buy-box-competitor-pricing.md) Preis und [kleinster Konkurrent](./lowest-competitor-pricing.md) Preis.

- Die [Listungsverbesserungen](./listing-improvements.md) zeigt alle von Amazon für den ausgewählten Store vorgeschlagenen Verbesserungen an.

>[!TIP]
>
>Sie können die Protokolldatei auch auf weitere Informationen prüfen, wenn die Fehlerbehebung erforderlich ist. Siehe [Admin-Einstellungen für Sales-Kanal](./sales-channel-settings.md). Die Protokollierung der Synchronisation von Amazon Sales Kanal wird in `{Commerce Root}/var/log/channel_amazon.log` Datei und kann angezeigt werden in [Entwicklermodus](https://docs.magento.com/user-guide/magento/installation-modes.html){Zielgruppe=&quot;_blank&quot;}.
