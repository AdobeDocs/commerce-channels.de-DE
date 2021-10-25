---
title: Ansicht Amazon Bestellungen
description: Ansicht Ihrer Amazon Marketplace-Bestellungen im Adobe Commerce oder Magento Open Source Admin.
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Ansicht Amazon-Aufträge

Es gibt zwei Möglichkeiten, Ihre Amazon-Bestellungen Ansicht: _[!UICONTROL Recent Orders]_und_[!UICONTROL All Orders]_.

Beide Optionen zeigen Ihnen grundlegende Bestellinformationen, wie sie von Amazon erhalten wurden, darunter:

- Kaufdatum
- Auftragsnummer
- Status
- Name des Käufers
- Gesamt
- Auftragsnotizen

_[!UICONTROL All Orders]_Ansicht fügt Filteroptionen für Auftragssuchvorgänge hinzu.

>[!NOTE]
>
>Ausgenommen sind _[!UICONTROL Order Notes]_-Spalte_[!UICONTROL Amazon orders]_ -Tabelle mit Bestellinformationen aus Amazon ausgefüllt. Die _Auftragsnotizen_ Spalte wird aktualisiert von [!DNL Commerce] als Auftragsabwicklung.

## Letzte Bestellungen

Sie können Ihre neuesten Bestellungen in der Ansicht _[!UICONTROL Recent Orders]_Abschnitt [Dashboard speichern](./amazon-store-dashboard.md).

![Letzte Bestellungen](assets/amazon-recent-orders-imported.png)

### Ansicht jüngster Amazon-Aufträge

1. Klick **[!UICONTROL View Store]** auf einer Ladenkarte.

1. Ansicht Ihrer Bestellungen im _[!UICONTROL Recent Orders]_Abschnitt.

1. Klicken Sie zur Ansicht der Auftragsdetails auf die Amazon-Bestellnummer im _[!UICONTROL Order Number]_Spalte.

   Die _[!UICONTROL Amazon Order Details]_-Seite für die Auftragsöffnung.

## Ansicht aller Bestellungen

Sie können alle Ihre Amazon-Bestellungen auf der Ansicht _[!UICONTROL Amazon orders]_Seite (auch als_[!UICONTROL All Orders]_ Ansicht). Die Amazon-Bestelltabelle ist ähnlich wie die _[!UICONTROL Recent Orders]_im Store-Dashboard, ermöglicht Ihnen jedoch die Ansicht aller Ihrer Amazon-Bestellungen und die Eingrenzung Ihrer Bestellungen-Liste mit den folgenden Filteroptionen:

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon-Aufträge](assets/amazon-orders-list-all.png)

### Ansicht aller Amazon-Bestellungen

1. Klick **[!UICONTROL View Store]** auf einer Ladenkarte.

1. Klick **[!UICONTROL All Orders]** in _[!UICONTROL Recent Orders]_Abschnitt.

1. Um die Liste einzuschränken oder nach einer bestimmten Bestellnummer zu suchen, füllen Sie **[!UICONTROL Filter by]** Parameter und klicken **[!UICONTROL Apply filters]**.

1. Klicken Sie zur Ansicht der Auftragsdetails auf die Amazon-Bestellnummer im _[!UICONTROL Order Number]_Spalte.

   Die _[!UICONTROL Amazon Order Details]_-Seite für die Auftragsöffnung.

## Filter verwenden

Sie können Filter auf Ihre Bestellungs-Liste anwenden in _[!UICONTROL Filter by]_Abschnitt. Wählen Sie aus und klicken Sie auf **[!UICONTROL Apply filters]**. Die angewendeten Filter werden über dem Auftragsraster angezeigt.

![Filter zum Anzeigen von Amazon-Bestellungen](assets/amazon-orders-filter-view.png)

### Angewendete Filter ändern

- Sie können Filter hinzufügen oder ändern in _[!UICONTROL Filter by]_Abschnitt. Klick **[!UICONTROL Apply filters]**um die Liste der Bestellung und die Filteroptionen zu aktualisieren, die über dem Auftragsraster angezeigt werden.

- Sie können Filter nacheinander entfernen, indem Sie auf `x` für den Filter oder alle gleichzeitig durch Klicken auf **[!UICONTROL Clear all filters]**. Durch das Entfernen eines Filters werden die Liste der Reihenfolge und die Filteroptionen aktualisiert, die über dem Auftragsraster angezeigt werden.

- Wenn die Liste Ihrer Bestellung lang ist, können Sie die Seitenumbruch-Steuerelemente unterhalb des Gitters verwenden, um weitere Bestellungen Ansicht.

>[!TIP]
>
>Einige Tipps zur Ansicht der Bestellungen:
>
>- Wenn Sie mehrere Amazon Store-Integrationen haben, kann ein Aktualisieren der Ansicht Ihrer Seite beim Wechsel zwischen Store-Ansichten erforderlich sein, um sowohl die Liste der Bestellungen als auch die Ansichten für die Seitenumbrüche des aktuellen Store zu aktualisieren.
>- Bei der Sortierung nach Spalte gilt die Sortierung nur für die Ansicht der aktuellen Liste. Es empfiehlt sich, die Liste zu filtern und dann die angezeigte Seite zu sortieren.
>- Abhängig von der Breite des Fensters Ihrer Ansicht können sich überschneidende Textfelder in den Spalten anzeigen. Um die Spalten für den Zeilenumbruch zu erweitern, erweitern Sie die Ansicht des Fensters.
>- Beim Filtern nach _[!UICONTROL Total]_, nach ganzen Zahlen filtern. Die Eingabe eines Dezimalbetrags kann zu Fehlern in den Ergebnissen führen.


### Standardspalten

| Spalte | Beschreibung |
|---|---|
| [!UICONTROL Filter by] | Nur verfügbar im _[!UICONTROL All Orders]_Ansicht.<br>Schränken Sie die Liste von Aufträgen auf folgender Grundlage ein:<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | Datum des Kaufs, wie von Amazon empfangen. |
| [!UICONTROL Order Number] | Die von und von Amazon generierte Bestellnummer. Klicken Sie auf den Link, um den Bildschirm &quot;Amazon-Auftragsdetails&quot;Ansicht. |
| [!UICONTROL Status] | Status der bei Amazon eingegangenen Bestellung. Optionen: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | Der Name der Person, die die Bestellung aufgegeben hat, wie er von Amazon erhalten wurde. |
| [!UICONTROL Grand Total] | Der Gesamtwährungswert der Bestellung, wie er von Amazon erhalten wurde. |
| [!UICONTROL Order Notes] | Zuletzt aufgezeichnete Aktion für die Bestellung, während sie verarbeitet in [!DNL Commerce]. Die Informationen umfassen u. a., sind aber nicht beschränkt auf Bestellfehler und Bestellverarbeitungs-Updates.<br>**Hinweis**: Dieses Feld wird aktualisiert von [!DNL Commerce] als Auftragsabwicklung. |
