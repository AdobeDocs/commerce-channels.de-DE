---
title: Vertriebskanaleinstellungen
description: Um die Protokollierung, Cron-Quelle und Synchronisation für Amazon-Vertriebskanalfunktionen zu verwalten, aktualisieren Sie die Commerce-Konfiguration.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
role: Admin, Developer
feature: Sales Channels, Configuration, Logs
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Vertriebskanaleinstellungen

Wenn die Erweiterung [!DNL Amazon Sales Channel] installiert ist, werden im Vertriebskanal &quot;Admin für Amazon&quot;Standardwerte festgelegt. Diese Einstellungen können in Ihren Konfigurationseinstellungen für Ihren Amazon Store geändert werden. Zu diesen Einstellungen gehören:

- Zeiträume für das Löschen des Aktivitätsprotokollverlaufs
- Cron-Quellauswahl
- Optionen zur Protokollsynchronisierung

## Einstellungen der Commerce-Kanäle ändern

1. Wechseln Sie in der Seitenleiste _Admin_ zu **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. Erweitern Sie im linken Bereich den Wert **[!UICONTROL Sales Channels]** und wählen Sie **[!UICONTROL Global Settings]** aus.

1. Wählen Sie für **[!UICONTROL Clear Log History]** eine Option:

   - `Once Daily` - Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal täglich zu löschen.

   - `Once Weekly` - Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal wöchentlich zu löschen.

   - `Once Monthly` - (Standard) Wählen Sie aus, den Verlauf Ihrer Store-Aktivität einmal monatlich zu löschen.

1. Wählen Sie für **[!UICONTROL Background Tasks (CRON) Source]** `Magento CRON` aus.

   Mit dieser Option kann der Amazon-Verkaufskanal Ihre [!DNL Commerce] [Cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) -Einstellungen verwenden, um Kommunikations- und Datensynchronisierungsintervalle mit [!DNL Amazon Seller Central] zu bestimmen.

1. Wählen Sie für **[!UICONTROL Enable Debug Logging]** `Enabled` aus, um zusätzliche Synchronisierungsdaten zu erfassen, wenn eine Fehlerbehebung erforderlich ist.

   Die Protokollierung von Amazon-Verkaufskanälen wird in die Datei `{Commerce Root}/var/log/channel_amazon.log` geschrieben und kann im [Entwicklermodus](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes) angezeigt werden. Die Protokollierung sollte während der Fehlerbehebung nur `Enabled` betragen und nach Abschluss der Fehlerbehebung `Disabled` betragen.

1. Wählen Sie für &quot;**[!UICONTROL Read-Only Mode]**&quot;die Option &quot;`Enabled`&quot;, um alle ausgehenden, sich vom Status ändernden API-Anfragen zu blockieren.

   Mit dieser Einstellung werden potenzielle Änderungen gespeichert, aber erst gesendet, wenn [!UICONTROL Read-Only Mode] deaktiviert ist. Der Konfigurationscache muss für den schreibgeschützten Modus gelöscht werden, um aktiviert zu werden. Um die Datenübertragungen erneut zu starten, wählen Sie `Disabled` aus.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] ist für Kopien der Produktionsinstanz wie Staging oder Qualitätssicherung konzipiert und sollte nicht in der Produktionsinstanz verwendet werden.
   >
   >Wenn eine Datenbank auf eine neue Kopie der Instanz migriert wird (erkannt, wenn sich die URL eines Stores in der Konfiguration ändert), wird [!UICONTROL Read-Only Mode] automatisch aktiviert.

1. Klicken Sie auf **[!UICONTROL Save Config]**.

![Sales Channel-Konfigurationseinstellungen](assets/config-sales-channel-global-settings.png){width="600" zoomable="yes"}
