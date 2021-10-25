---
title: Amazon-Listen manuell veröffentlichen
description: Bei Bedarf können Sie Ihre beendeten Amazon-Einträge manuell über Ihren Commerce-Administrator veröffentlichen.
exl-id: ca3f674e-d93a-44a6-8c06-b417694a0f1e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Amazon-Listen manuell veröffentlichen

Sie können eine oder mehrere beendete Amazon-Auflistungen manuell veröffentlichen.

1. Ansicht einer oder mehrerer Auflistungen auf der _[!UICONTROL Ended]_auf [Produktauflistungen](./managing-product-listings.md) Seite (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_oder_[!UICONTROL Ineligible]_ Tabulator).

1. Klicken Sie in der linken Spalte, um die einzelnen Einträge zu überprüfen, die Sie erneut veröffentlichen möchten.

1. Unter _[!UICONTROL Actions]_, klicken **[!UICONTROL Publish Product to Amazon]**.

1. Klick **[!UICONTROL OK]** in der Bestätigungsmeldung.

   Es wird eine Meldung angezeigt, mit der bestätigt wird, dass die ausgewählten Auflistungen zur Veröffentlichung auf Amazon verarbeitet werden.

   Listungsinformationen werden auf Basis Ihrer cron-Einstellungen auf Amazon veröffentlicht. Bei der nächsten Datensynchronisierung werden Listendaten an Amazon gesendet. Bis Amazon mit der Bestätigung der Auflistung antwortet, bleiben die manuell veröffentlichten Listen auf der _Bereit für Liste_ Tabulator mit `List in Progress` Status. Wenn die Listungsbestätigung von Amazon erhalten wird, werden die Listen in die _Aktiv_ mit einem Tabulator `Active` Status.
