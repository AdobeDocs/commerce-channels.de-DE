---
title: Sales Channel-Einstellungen
description: Aktualisieren Sie die Commerce-Konfiguration, um Protokollierung, Cron-Quelle und Synchronisation für Amazon Sales Kanal-Funktionen zu verwalten.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Sales Channel-Einstellungen

Wann [!DNL Amazon Sales Channel] -Erweiterung installiert ist, werden die Standardwerte im Admin for Amazon Sales Kanal festgelegt. Diese Einstellungen können in Ihren Konfigurationseinstellungen für Ihren Amazon Store geändert werden. Diese Einstellungen umfassen:

- Zeiträume für das Löschen des Protokollverlaufs der Aktivität
- Cron-Quellauswahl
- Protokollsynchronisierungsoptionen

## Geschäftliche Kanal-Einstellungen ändern

1. Auf _Admin_ Sidebar, Gehe zu **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Erweitern Sie im linken Bereich **[!UICONTROL Sales Channels]** und wählen **[!UICONTROL Global Settings]**.

1. für **[!UICONTROL Clear Log History]**, wählen Sie eine Option aus:

   - `Once Daily` - Wählen Sie aus, ob Sie den Verlauf Ihrer Aktivität einmal täglich löschen möchten.

   - `Once Weekly` - Wählen Sie aus, ob der Verlauf Ihrer Aktivität einmal wöchentlich gelöscht werden soll.

   - `Once Monthly` - (Standard) Wählen Sie aus, ob der Verlauf Ihrer Store-Aktivität einmal monatlich gelöscht werden soll.

1. für **[!UICONTROL Background Tasks (CRON) Source]**, wählen `Magento CRON`.

   Mit dieser Option kann Amazon Sales Kanal Ihre [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html) Einstellungen zur Bestimmung der Kommunikations- und Datensynchronisierungsintervalle mit [!DNL Amazon Seller Central].

1. für **[!UICONTROL Enable Debug Logging]**, wählen `Enabled` um zusätzliche Synchronisierungsdaten zu erfassen, wenn die Fehlerbehebung erforderlich ist.

   Die Protokollierung des Amazon Sales Kanal wird in `{Commerce Root}/var/log/channel_amazon.log` Datei und kann angezeigt werden in [Entwicklermodus](https://docs.magento.com/user-guide/magento/installation-modes.html){Zielgruppe=&quot;_blank&quot;}. Protokollierung darf nur `Enabled` während der Fehlerbehebung und sollte `Disabled` wenn die Fehlerbehebung abgeschlossen ist.

1. Klick **[!UICONTROL Save Config]**.

![Konfigurationseinstellungen für Sales Channel](assets/config-sales-channel-global-settings.png)
