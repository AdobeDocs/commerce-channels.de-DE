---
title: Amazon-Listen manuell veröffentlichen
description: Bei Bedarf können Sie Ihre beendeten Amazon-Auflistungen manuell über Ihren Commerce-Administrator veröffentlichen.
feature: Sales Channels, Products, Merchandising
exl-id: ca3f674e-d93a-44a6-8c06-b417694a0f1e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Amazon-Listen manuell veröffentlichen

Sie können eine oder mehrere Amazon-Listen, die beendet wurden, manuell veröffentlichen.

1. Anzeigen von Listen auf der _[!UICONTROL Ended]_auf der Registerkarte [Produktlisten](./managing-product-listings.md) page (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_oder_[!UICONTROL Ineligible]_ Registerkarte).

1. Klicken Sie in der linken Spalte auf , um die einzelnen Listen zu überprüfen, die Sie erneut veröffentlichen möchten.

1. under _[!UICONTROL Actions]_klicken **[!UICONTROL Publish Product to Amazon]**.

1. Klicks **[!UICONTROL OK]** in der Bestätigungsnachricht angezeigt.

   Es wird eine Meldung angezeigt, die bestätigt, dass die ausgewählten Listen zur Veröffentlichung in Amazon verarbeitet werden.

   Listening-Informationen werden basierend auf Ihren Cron-Einstellungen in Amazon veröffentlicht. Listening-Informationen werden bei der nächsten Datensynchronisierung an Amazon gesendet. Bis Amazon mit der Listenbestätigung antwortet, bleiben die manuell veröffentlichten Listen auf der _Listenbereit_ mit einem `List in Progress` -Status. Wenn die Listenbestätigung von Amazon empfangen wird, werden die Listen in die _Aktiv_ mit einer `Active` -Status.
