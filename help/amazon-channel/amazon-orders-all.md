---
title: Anzeigen von Amazon-Bestellungen
description: Zeigen Sie Ihre Amazon Marketplace-Bestellungen in der Adobe Commerce- oder Magento Open Source-Administration an.
feature: Sales Channels, Orders
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Anzeigen von Amazon-Bestellungen

Es gibt zwei Möglichkeiten, Ihre Amazon-Bestellungen anzuzeigen: _[!UICONTROL Recent Orders]_und_[!UICONTROL All Orders]_.

Beide Optionen zeigen Ihnen grundlegende Bestellinformationen, die von Amazon empfangen werden, darunter:

- Kaufdatum
- Bestellnummer
- Status
- Name des Käufers
- Gesamtsumme
- Bestellhinweise

Die Ansicht &quot;_[!UICONTROL All Orders]_&quot; fügt Filteroptionen für Auftragssuchvorgänge hinzu.

>[!NOTE]
>
>Mit Ausnahme der Spalte _[!UICONTROL Order Notes]_wird die Tabelle_[!UICONTROL Amazon orders]_ mit Bestellinformationen aus Amazon gefüllt. Die Spalte _Bestellnotizen_ wird von [!DNL Commerce] aktualisiert, wenn die Bestellung verarbeitet wird.

## Letzte Bestellungen

Sie können Ihre neuesten Bestellungen im Abschnitt _[!UICONTROL Recent Orders]_des [Dashboard speichern](./amazon-store-dashboard.md) anzeigen.

![Letzte Bestellungen](assets/amazon-recent-orders-imported.png){width="600" zoomable="yes"}

### Aktuelle Amazon-Bestellungen anzeigen

1. Klicken Sie auf einer Store-Karte auf **[!UICONTROL View Store]**.

1. Zeigen Sie Ihre Bestellungen im Abschnitt _[!UICONTROL Recent Orders]_an.

1. Um Bestelldetails anzuzeigen, klicken Sie in der Spalte _[!UICONTROL Order Number]_auf die Amazon-Bestellnummer.

   Die Seite _[!UICONTROL Amazon Order Details]_für die Bestellung wird geöffnet.

## Alle Bestellungen anzeigen

Sie können alle Ihre Amazon-Bestellungen auf der Seite _[!UICONTROL Amazon orders]_anzeigen (auch als_[!UICONTROL All Orders]_-Ansicht bezeichnet). Die Amazon-Bestelltabelle ähnelt dem Abschnitt _[!UICONTROL Recent Orders]_im Store-Dashboard. Sie können jedoch alle Ihre Amazon-Bestellungen anzeigen und Ihre Bestellliste mit den folgenden Filteroptionen eingrenzen:

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon-Bestellungen](assets/amazon-orders-list-all.png){width="600" zoomable="yes"}

### Alle Amazon-Bestellungen anzeigen

1. Klicken Sie auf einer Store-Karte auf **[!UICONTROL View Store]**.

1. Klicken Sie im Abschnitt _[!UICONTROL Recent Orders]_auf **[!UICONTROL All Orders]**.

1. Um die Liste einzuschränken oder nach einer bestimmten Bestellnummer zu suchen, füllen Sie die Parameter **[!UICONTROL Filter by]** aus und klicken Sie auf **[!UICONTROL Apply filters]**.

1. Um Bestelldetails anzuzeigen, klicken Sie in der Spalte _[!UICONTROL Order Number]_auf die Amazon-Bestellnummer.

   Die Seite _[!UICONTROL Amazon Order Details]_für die Bestellung wird geöffnet.

## Filter verwenden

Sie können Filter auf Ihre Bestellliste im Abschnitt _[!UICONTROL Filter by]_anwenden. Nehmen Sie Ihre Auswahl vor und klicken Sie auf **[!UICONTROL Apply filters]**. Die angewendeten Filter werden über dem Raster der Bestellungen angezeigt.

![Filter zum Anzeigen von Amazon-Bestellungen](assets/amazon-orders-filter-view.png){width="600" zoomable="yes"}

### Ändern angewendeter Filter

- Sie können Ihre Filter im Abschnitt _[!UICONTROL Filter by]_hinzufügen oder ändern. Klicken Sie auf **[!UICONTROL Apply filters]**, um die Liste der Bestellungen und die Filteroptionen zu aktualisieren, die über dem Bestellungsraster angezeigt werden.

- Sie können Filter entweder einzeln entfernen, indem Sie für den Filter auf &quot;`x`&quot;klicken oder alle gleichzeitig auf &quot;**[!UICONTROL Clear all filters]**&quot;. Wenn Sie einen Filter entfernen, werden die Liste der Bestellungen und die Filteroptionen, die über dem Bestellungsraster angezeigt werden, aktualisiert.

- Wenn Ihre Bestellliste lang ist, können Sie die Paginierungssteuerelemente unterhalb des Rasters verwenden, um weitere Bestellungen anzuzeigen.

>[!TIP]
>
>Einige Tipps zur Ansicht der Bestellungen:
>
>- Wenn Sie über mehrere Amazon Store-Integrationen verfügen, kann eine Aktualisierung Ihrer Seitenansicht beim Wechsel zwischen Store-Ansichten erforderlich sein, um sowohl die Bestellliste als auch die Paginierungsansichten für den aktuellen Store zu aktualisieren.
>- Bei der Sortierung nach Spalte gilt die Sortierung nur für die aktuelle Listenansicht. Es empfiehlt sich, die Liste zu filtern und anschließend die Seite zu sortieren, die Sie anzeigen.
>- Abhängig von der Breite des Ansichtsfensters können Sie in den Spalten überlappenden Text sehen. Um die Spalten für den Text zu erweitern, erweitern Sie die Fensteransicht.
>- Filtern Sie beim Filtern nach _[!UICONTROL Total]_nach Ganzzahlen. Die Eingabe eines Dezimalbetrags kann zu Fehlern in den Ergebnissen führen.

### Standardspalten

| Spalte | Beschreibung |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Filter by] | Nur in der Ansicht _[!UICONTROL All Orders]_verfügbar.<br>Schränken Sie die Liste der Bestellungen auf Grundlage von:<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | Das Datum des Kaufs, wie es von Amazon empfangen wurde. |
| [!UICONTROL Order Number] | Die von Amazon generierte und von ihm empfangene Bestellnummer. Um den Bildschirm &quot;Amazon-Bestelldetails&quot;anzuzeigen, klicken Sie auf den Link. |
| [!UICONTROL Status] | Der Status der Bestellung, wie er von Amazon empfangen wurde. Optionen: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | Der Name der Person, die die Bestellung aufgegeben hat, wie er von Amazon empfangen wurde. |
| [!UICONTROL Grand Total] | Der Gesamtwährungswert der Bestellung, wie er von Amazon empfangen wurde. |
| [!UICONTROL Order Notes] | Die letzte Aktion, die für die Reihenfolge aufgezeichnet wurde, während sie in [!DNL Commerce] verarbeitet wird. Die Informationen umfassen u. a. Bestellimportfehler und Bestellaktualisierungen.<br>**Hinweis**: Dieses Feld wird von [!DNL Commerce] aktualisiert, wenn die Bestellung verarbeitet wird. |
