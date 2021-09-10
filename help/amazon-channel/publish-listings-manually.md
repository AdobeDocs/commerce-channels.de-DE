---
title: Amazon-Listen manuell veröffentlichen
description: Bei Bedarf können Sie Ihre beendeten Amazon-Auflistungen manuell über Ihren Commerce-Administrator veröffentlichen.
exl-id: ca3f674e-d93a-44a6-8c06-b417694a0f1e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Amazon-Listen manuell veröffentlichen

Sie können eine oder mehrere Amazon-Listen, die beendet wurden, manuell veröffentlichen.

1. Zeigen Sie eine oder mehrere Auflistungen auf der Registerkarte _[!UICONTROL Ended]_auf der Seite [Produktauflistungen](./managing-product-listings.md) an (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_oder_[!UICONTROL Ineligible]_ Registerkarte).

1. Klicken Sie in der linken Spalte auf , um die einzelnen Listen zu überprüfen, die Sie erneut veröffentlichen möchten.

1. Klicken Sie unter _[!UICONTROL Actions]_auf **[!UICONTROL Publish Product to Amazon]**.

1. Klicken Sie in der Bestätigungsnachricht auf **[!UICONTROL OK]**.

   Es wird eine Meldung angezeigt, die bestätigt, dass die ausgewählten Listen zur Veröffentlichung in Amazon verarbeitet werden.

   Listening-Informationen werden basierend auf Ihren Cron-Einstellungen in Amazon veröffentlicht. Listening-Informationen werden bei der nächsten Datensynchronisierung an Amazon gesendet. Bis Amazon mit der Auflistungsbestätigung antwortet, bleiben die manuell veröffentlichten Auflistungen auf der Registerkarte _Bereit zur Liste_ mit dem Status `List in Progress`. Wenn die Listenbestätigung von Amazon empfangen wird, werden die Auflistungen auf den Tab _Aktiv_ mit dem Status `Active` verschoben.
