---
title: Sales Channel-Einstellungen
description: Aktualisieren Sie die Commerce-Konfiguration, um die Protokollierung, Cron-Quelle und Synchronisation für Amazon-Vertriebskanalfunktionen zu verwalten.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Sales Channel-Einstellungen

Wenn die [!DNL Amazon Sales Channel]-Erweiterung installiert ist, werden im Vertriebskanal &quot;Admin für Amazon&quot;Standardwerte festgelegt. Diese Einstellungen können in Ihren Konfigurationseinstellungen für Ihren Amazon Store geändert werden. Zu diesen Einstellungen gehören:

- Zeiträume für das Löschen des Aktivitätsprotokollverlaufs
- Cron-Quellauswahl
- Optionen zur Protokollsynchronisierung

## Ändern der Einstellungen für Commerce-Kanäle

1. Gehen Sie in der Seitenleiste _Admin_ zu **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Erweitern Sie im linken Bereich **[!UICONTROL Sales Channels]** und wählen Sie **[!UICONTROL Global Settings]** aus.

1. Wählen Sie für **[!UICONTROL Clear Log History]** eine Option:

   - `Once Daily` - Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal täglich zu löschen.

   - `Once Weekly` - Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal wöchentlich zu löschen.

   - `Once Monthly` - (Standard) Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal monatlich zu löschen.

1. Wählen Sie für **[!UICONTROL Background Tasks (CRON) Source]** `Magento CRON` aus.

   Mit dieser Option kann der Amazon-Vertriebskanal Ihre [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html)-Einstellungen verwenden, um Kommunikations- und Datensynchronisierungsintervalle mit [!DNL Amazon Seller Central] zu bestimmen.

1. Wählen Sie für **[!UICONTROL Enable Debug Logging]** `Enabled` aus, um bei der Fehlerbehebung zusätzliche Synchronisierungsdaten zu erfassen.

   Die Protokollierung von Amazon-Verkaufskanälen wird in die Datei `{Commerce Root}/var/log/channel_amazon.log` geschrieben und kann im [Entwicklermodus](https://docs.magento.com/user-guide/magento/installation-modes.html){:target=&quot;_blank&quot;} angezeigt werden. Die Protokollierung sollte während der Fehlerbehebung nur `Enabled` sein und `Disabled` sein, wenn die Fehlerbehebung abgeschlossen ist.

1. Klicken Sie auf **[!UICONTROL Save Config]**.

![Sales Channel-Konfigurationseinstellungen](assets/config-sales-channel-global-settings.png)
