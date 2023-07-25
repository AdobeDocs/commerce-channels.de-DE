---
title: Vertriebskanaleinstellungen
description: Aktualisieren Sie die Commerce-Konfiguration, um die Protokollierung, Cron-Quelle und Synchronisation für Amazon-Vertriebskanalfunktionen zu verwalten.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
role: Admin, Developer
feature: Sales Channels, Configuration, Logs
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Vertriebskanaleinstellungen

Wenn die [!DNL Amazon Sales Channel] installiert ist, werden im Vertriebskanal Admin für Amazon Standardwerte festgelegt. Diese Einstellungen können in Ihren Konfigurationseinstellungen für Ihren Amazon Store geändert werden. Zu diesen Einstellungen gehören:

- Zeiträume für das Löschen des Aktivitätsprotokollverlaufs
- Cron-Quellauswahl
- Optionen zur Protokollsynchronisierung

## Ändern der Einstellungen für Commerce-Kanäle

1. Im _Admin_ Seitenleiste, navigieren Sie zu **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Erweitern Sie im linken Bereich **[!UICONTROL Sales Channels]** und wählen Sie **[!UICONTROL Global Settings]**.

1. Für **[!UICONTROL Clear Log History]**, wählen Sie eine Option aus:

   - `Once Daily` - Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal täglich zu löschen.

   - `Once Weekly` - Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal wöchentlich zu löschen.

   - `Once Monthly` - (Standard) Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal monatlich zu löschen.

1. Für **[!UICONTROL Background Tasks (CRON) Source]** auswählen `Magento CRON`.

   Mit dieser Option kann der Amazon-Vertriebskanal Ihre [!DNL Commerce] [Cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) Einstellungen zum Ermitteln von Kommunikations- und Datensynchronisierungsintervallen mit [!DNL Amazon Seller Central].

1. Für **[!UICONTROL Enable Debug Logging]** auswählen `Enabled` , um bei der Fehlerbehebung zusätzliche Synchronisierungsdaten zu erfassen.

   Die Protokollierung des Amazon-Vertriebskanals wird in `{Commerce Root}/var/log/channel_amazon.log` Datei und kann in [Entwicklermodus](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes). Die Protokollierung sollte nur `Enabled` während der Fehlerbehebung und sollten `Disabled` wenn die Fehlerbehebung abgeschlossen ist.

1. Für **[!UICONTROL Read-Only Mode]** auswählen `Enabled` , um alle ausgehenden, sich ändernden API-Anfragen zu blockieren.

   Mit dieser Einstellung werden potenzielle Änderungen gespeichert, aber nicht gesendet, bis [!UICONTROL Read-Only Mode] deaktiviert ist. Der Konfigurationscache muss für den schreibgeschützten Modus gelöscht werden, um aktiviert zu werden. Um die Datenübertragung erneut zu starten, wählen Sie `Disabled`.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] ist für Kopien der Produktionsinstanz wie Staging oder Qualitätssicherung konzipiert und sollte nicht in der Produktionsinstanz verwendet werden.
   >
   >Wenn eine Datenbank auf eine neue Kopie der Instanz migriert wird (erkannt, wenn sich die URL eines Stores in der Konfiguration ändert), [!UICONTROL Read-Only Mode] automatisch aktiviert ist.

1. Klicken **[!UICONTROL Save Config]**.

![Sales Channel-Konfigurationseinstellungen](assets/config-sales-channel-global-settings.png){width="600" zoomable="yes"}
