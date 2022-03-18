---
title: Workspace-Steuerelemente
description: Amazon Sales Channel bietet Arbeitsbereichssteuerungen, mit denen Sie Auflistungen finden, Informationen anzeigen und Aktionen einfach anwenden können.
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Workspace-Steuerelemente

Der Amazon-Vertriebskanal [Startseite](./amazon-sales-channel-home.md) verfügt über einige gängige Steuerelemente für den Arbeitsbereich, darunter Filter, Standardansicht, Spalten und Export. Nicht alle Seiten haben die gleichen Steuerungsoptionen.

![Beispiele für Steuerelemente in Amazon Sales Channel Workspace](assets/amazon-workspace-controls.png)

## Aktionen

Die _[!UICONTROL Actions]_selector stellt eine Liste von Aktionen bereit, die einem Benutzer für eine Seite zur Verfügung stehen. Wenn diese Option ausgewählt ist, wird die Aktion auf alle ausgewählten Elemente angewendet. Um eine Aktion auf ein bestimmtes Element anzuwenden, aktivieren Sie das Kontrollkästchen in der ersten Spalte jedes Elements und wählen Sie eine Option unter_[!UICONTROL Actions]_.

Wenn beispielsweise der Selektor auf der _[!UICONTROL Attributes]_Seite, enthält sie die_[!UICONTROL Re-import Product Attribute Values]_ Aktion. Wenn Sie diese Aktion auswählen, wird der entsprechende Ping eingefügt [!DNL Amazon Seller Central] -Konto und aktualisiert die [!DNL Commerce] -Daten für jedes der Amazon-Store-Elemente, die in der linken Spalte aktiviert sind.

![Menübeispiel Aktionen](assets/amazon-sales-channel-home-actions-option.png)

## Filter

Die _[!UICONTROL Filters]_-Steuerelement zeigt Optionen zum Eingrenzen der in der Tabelle angezeigten Daten an. Filteroptionen basieren auf den im Spalten-Steuerelement ausgewählten Spalten. Filteroptionen werden nur für Spalten angezeigt, die im Spalten-Steuerelement aktiviert sind.

Filtersteuerelemente können dynamische Kalender enthalten, um Daten für bestimmte Datumsangaben einzuschränken, Dropdownmenüs für Spalten mit vordefinierten Auswahlmöglichkeiten und Freitextfelder, die benutzerdefinierte Daten enthalten können.

Das folgende Beispiel zeigt die Einstellungen zum Filtern der Liste von Bestellungen, sodass nur Bestellungen angezeigt werden, die die folgenden Kriterien erfüllen:

- zwischen dem 1.1.2019 und dem 2.7.2019 aufgegebene Bestellungen und
- Bestellungen mit einem Käufer mit dem Namen `Smith`und
- Bestellungen mit dem Status `Shipped`.

Wenn Sie die Filteroptionen festgelegt haben, klicken Sie auf **[!UICONTROL Apply Filters]** , um die aufgeführten Daten zu filtern. Klicken Sie auf Abbrechen , um das Steuerelement Filter zu verlassen, ohne anzuwenden.

![Beispiel für eine Filtersteuerung](assets/workspace-controls-filters.png)

Nachdem Sie Filter auf Ihre Daten angewendet haben, **[!UICONTROL Active Filters]** angezeigt. Sie können auf die ![Symbol Filter löschen](assets/x-icon-clear-filters.png) Symbol zum Löschen einer bestimmten Filteroption oder klicken Sie auf **[!UICONTROL Clear All]** , um alle angewendeten Filter zu löschen.

![Beispiel für aktive Filter](assets/applied-filters-line.png)

## Ansicht

Das Ansichtssteuerelement basiert auf den Standardspalten für die Seite und erhält daher den Namen &quot;Standardansicht&quot;. Mithilfe des Spalten-Steuerelements können Sie verfügbare Spalten hinzufügen oder entfernen. Wenn Sie Ihre Spalten anpassen, können Sie die Ansicht dann als benutzerdefinierte Ansicht im Ansichtssteuerelement speichern.

Wenn Sie Ihre Spalten von der Seite hinzugefügt oder entfernt haben, wird Folgendes angezeigt:

1. Klicken **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**.

1. Geben Sie einen Namen für die Ansicht ein.

1. Um die benutzerdefinierte Ansicht zu speichern, klicken Sie auf das Pfeilsymbol.

![Steuerbeispiel anzeigen](assets/workspace-controls-view.png)

In diesem Beispiel wird die _Auftrags-ID_ wird im Spalten-Steuerelement hinzugefügt und als benutzerdefinierte Ansicht gespeichert. Beachten Sie, dass sich der Name der Ansicht nach dem Speichern des benutzerdefinierten Ansichtsnamens von _Standardansicht_ zum eingegebenen Namen.

Sie können zwischen den Ansichten umschalten, indem Sie die gewünschte Ansicht im _[!UICONTROL View]_Menü.

Wenn Sie den Namen Ihrer benutzerdefinierten Ansicht löschen oder ändern möchten, klicken Sie auf das Stiftsymbol. Sie können dann einen anderen Namen eingeben oder auf das Papierkorbsymbol klicken, um die benutzerdefinierte Ansicht zu löschen. Die Standardansicht kann nicht gelöscht werden.

## Spalten

Mit dem Spalten-Steuerelement können Sie Spalten von Daten zur Seitenanzeige hinzufügen oder daraus entfernen. Jede Amazon-Vertriebskanalseite verfügt über eine vordefinierte Kombination von Datenspalten, aber die meisten Seiten verfügen über zusätzliche Spalten. Wenn keine weiteren Spalten verfügbar sind, können Sie die Standardspalten aus der Anzeige entfernen.

Das folgende Beispiel zeigt ein Spalten-Steuerelement. Die aktivierten Optionen entsprechen den Spaltenüberschriften, die auf der Seite angezeigt werden.

- Um Ihrer Seite eine Datenspalte hinzuzufügen, aktivieren Sie das Kontrollkästchen .
- Um eine Datenspalte aus Ihrer Seite zu entfernen, aktivieren Sie das Kontrollkästchen nicht.

![Beispiel für Spalten-Steuerung](assets/workspace-controls-columns.png)

Kontrollkästchenänderungen werden sofort angezeigt. Wenn Sie Änderungen vornehmen und die Seite verlassen, kehrt die Seite zur standardmäßigen Spaltenanzeige zurück. Für regelmäßig vorgenommene Änderungen können Sie die Spaltenänderungen als benutzerdefinierte Ansicht im Ansichtssteuerelement speichern. Anschließend können Sie im Ansichtssteuerelement umschalten, ohne Spalten manuell hinzufügen oder entfernen zu müssen.

Sie können auf **[!UICONTROL Reset]** , um die Optionen wieder auf die Standardeinstellungen zurückzusetzen, oder Sie können auf **[!UICONTROL Cancel]** , um ohne Ihre Änderungen zu beenden.

## Export

Mit der Option Exportieren können Sie die Daten in eine Datendatei exportieren, die dann in eine Drittanbieter-Software oder in eine separate Datenbank importiert werden kann. Die exportierten Daten sind auf die angezeigten Daten beschränkt. Stellen Sie bei Bedarf sicher, dass Sie Spalten hinzufügen oder entfernen, bevor Sie das Exportsteuerelement verwenden.

Wenn Sie bereit sind, Ihre Daten zu exportieren, wählen Sie eine Exportformatoption und klicken Sie auf **[!UICONTROL Export]**.

- CSV - eine kommagetrennte Wertdatei mit Textdaten
- Excel XML - ein XML-basiertes Tabellendatenformat (typisch für Excel-Benutzer)

Die generierte Datendatei speichert automatisch zum Herunterladen in Ihrem angegebenen Ordner.

![Exportkontrolle](assets/workspace-controls-export.png)
