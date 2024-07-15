---
title: Amazon-Vertriebskanal - Workspace-Steuerelemente
description: Amazon Sales Channel bietet Arbeitsbereichssteuerungen, mit denen Sie Auflistungen finden, Informationen anzeigen und Aktionen einfach anwenden können.
feature: Sales Channels
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Workspace-Steuerelemente

Der Amazon-Vertriebskanal [Homepage](./amazon-sales-channel-home.md) verfügt über einige gängige Arbeitsbereichssteuerelemente wie Filter, Standardansicht, Spalten und Export. Nicht alle Seiten haben die gleichen Steuerungsoptionen.

![Beispiele für Amazon Sales Channel Workspace-Steuerelemente](assets/amazon-workspace-controls.png){width="600" zoomable="yes"}

## Aktionen

Der &quot;_[!UICONTROL Actions]_&quot;-Selektor bietet eine Liste von Aktionen, die einem Benutzer für eine Seite zur Verfügung stehen. Wenn diese Option ausgewählt ist, wird die Aktion auf alle ausgewählten Elemente angewendet. Um eine Aktion auf ein bestimmtes Element anzuwenden, aktivieren Sie das Kontrollkästchen in der ersten Spalte jedes Elements und wählen Sie eine Option unter_[!UICONTROL Actions]_ aus.

Wenn der Selektor beispielsweise auf der Seite _[!UICONTROL Attributes]_angezeigt wird, enthält er die Aktion_[!UICONTROL Re-import Product Attribute Values]_. Wenn Sie diese Aktion auswählen, wird das entsprechende [!DNL Amazon Seller Central] -Konto gepingt und die [!DNL Commerce]-Daten für jedes der in der linken Spalte aktivierten Amazon-Store-Elemente aktualisiert.

Beispiel für das Menü ![Aktionen](assets/amazon-sales-channel-home-actions-option.png){width="500"}

## Filter

Das Steuerelement _[!UICONTROL Filters]_zeigt Optionen zum Eingrenzen der in der Tabelle angezeigten Daten an. Filteroptionen basieren auf den im Spalten-Steuerelement ausgewählten Spalten. Filteroptionen werden nur für Spalten angezeigt, die im Spalten-Steuerelement aktiviert sind.

Filtersteuerelemente können dynamische Kalender enthalten, um Daten für bestimmte Datumsangaben einzuschränken, Dropdownmenüs für Spalten mit vordefinierten Auswahlmöglichkeiten und Freitextfelder, die benutzerdefinierte Daten enthalten können.

Das folgende Beispiel zeigt die Einstellungen zum Filtern der Liste von Bestellungen, sodass nur Bestellungen angezeigt werden, die die folgenden Kriterien erfüllen:

- zwischen dem 1.1.2019 und dem 2.7.2019 aufgegebene Bestellungen und
- Bestellungen mit einem Käufer mit dem Namen &quot;`Smith`&quot; und
- Bestellungen mit dem Status `Shipped`.

Wenn Sie die Filteroptionen festgelegt haben, klicken Sie auf **[!UICONTROL Apply Filters]** , um die angezeigten Daten zu filtern. Klicken Sie auf Abbrechen , um das Steuerelement Filter zu verlassen, ohne anzuwenden.

![Beispiel für das Steuerelement &quot;Filter&quot;](assets/workspace-controls-filters.png){width="600" zoomable="yes"}

Nachdem Sie Filter auf Ihre Daten angewendet haben, werden **[!UICONTROL Active Filters]** -Informationen angezeigt. Sie können auf das Symbol ![Filter löschen](assets/x-icon-clear-filters.png) klicken, um eine bestimmte Filteroption zu löschen, oder auf **[!UICONTROL Clear All]** klicken, um alle angewendeten Filter zu löschen.

![Beispiel für aktive Filter](assets/applied-filters-line.png){width="700"}

## Ansicht

Das Ansichtssteuerelement basiert auf den Standardspalten für die Seite und erhält daher den Namen Standardansicht. Mithilfe des Spalten-Steuerelements können Sie verfügbare Spalten hinzufügen oder entfernen. Wenn Sie Ihre Spalten anpassen, können Sie die Ansicht dann als benutzerdefinierte Ansicht im Ansichtssteuerelement speichern.

Wenn Sie Ihre Spalten von der Seite hinzugefügt oder entfernt haben, wird Folgendes angezeigt:

1. Klicken Sie auf **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**.

1. Geben Sie einen Namen für die Ansicht ein.

1. Um die benutzerdefinierte Ansicht zu speichern, klicken Sie auf das Pfeilsymbol.

![Steuerelementbeispiel anzeigen](assets/workspace-controls-view.png)

In diesem Beispiel wird die Spalte _Bestell-ID_ im Spalten-Steuerelement hinzugefügt und als benutzerdefinierte Ansicht gespeichert. Beachten Sie, dass sich der Name der Ansicht nach dem Speichern des benutzerdefinierten Ansichtsnamens von _Standardansicht_ in den eingegebenen Namen änderte.

Sie können zwischen den Ansichten umschalten, indem Sie die gewünschte Ansicht im Menü _[!UICONTROL View]_auswählen.

Wenn Sie den Namen Ihrer benutzerdefinierten Ansicht löschen oder ändern möchten, klicken Sie auf das Stiftsymbol. Sie können dann einen anderen Namen eingeben oder auf das Papierkorbsymbol klicken, um die benutzerdefinierte Ansicht zu löschen. Die Standardansicht kann nicht gelöscht werden.

## Spalten

Mit dem Spalten-Steuerelement können Sie Spalten von Daten zur Seitenanzeige hinzufügen oder daraus entfernen. Jede Amazon-Vertriebskanalseite verfügt über eine vordefinierte Kombination von Datenspalten, aber die meisten Seiten verfügen über zusätzliche Spalten. Wenn keine weiteren Spalten verfügbar sind, können Sie die Standardspalten aus der Anzeige entfernen.

Das folgende Beispiel zeigt ein Spalten-Steuerelement. Die aktivierten Optionen entsprechen den Spaltenüberschriften, die auf der Seite angezeigt werden.

- Um Ihrer Seite eine Datenspalte hinzuzufügen, aktivieren Sie das Kontrollkästchen .
- Um eine Datenspalte aus Ihrer Seite zu entfernen, aktivieren Sie das Kontrollkästchen nicht.

Beispiel für das Steuerelement ![Spalten](assets/workspace-controls-columns.png){width="400"}

Kontrollkästchenänderungen werden sofort angezeigt. Wenn Sie Änderungen vornehmen und die Seite verlassen, kehrt die Seite zur standardmäßigen Spaltenanzeige zurück. Für regelmäßig vorgenommene Änderungen können Sie die Spaltenänderungen als benutzerdefinierte Ansicht im Ansichtssteuerelement speichern. Anschließend können Sie im Ansichtssteuerelement umschalten, ohne Spalten manuell hinzufügen oder entfernen zu müssen.

Sie können auf **[!UICONTROL Reset]** klicken, um die Optionen wieder auf die Standardeinstellungen zurückzusetzen, oder Sie können auf **[!UICONTROL Cancel]** klicken, um ohne Ihre Änderungen zu beenden.

## Export

Mit der Option Exportieren können Sie die Daten in eine Datendatei exportieren, die dann in eine Drittanbieter-Software oder in eine separate Datenbank importiert werden kann. Die exportierten Daten sind auf die angezeigten Daten beschränkt. Stellen Sie bei Bedarf sicher, dass Sie Spalten hinzufügen oder entfernen, bevor Sie das Exportsteuerelement verwenden.

Wenn Sie bereit sind, Ihre Daten zu exportieren, wählen Sie eine Exportformatoption und klicken Sie auf **[!UICONTROL Export]**.

- CSV - eine kommagetrennte Wertdatei mit Textdaten
- Excel XML - ein XML-basiertes Tabellendatenformat (typisch für Excel-Benutzer)

Die generierte Datendatei speichert automatisch zum Herunterladen in Ihrem angegebenen Ordner.

![Steuerelement exportieren](assets/workspace-controls-export.png){width="250"}
