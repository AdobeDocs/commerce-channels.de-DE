---
title: Überschreibungen erstellen und bearbeiten
description: Verwenden Sie Amazon Sales Channel-Überschreibungen, um Ihre Änderungen auf eine einzelne Amazon-Auflistung oder auf mehrere Auflistungen anzuwenden.
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Überschreibungen erstellen und bearbeiten

Sie können eine Auflistung erstellen und überschreiben oder eine auf eine Auflistung angewendete Außerkraftsetzung bearbeiten oder entfernen. Überschreibt die Einstellung eines bestimmten Werts für eine bestimmte Auflistung.

## Überschreibung für eine einzelne Auflistung erstellen

Die _[!UICONTROL Create Override]_Aktion ist verfügbar, wenn Auflistungen auf der_[!UICONTROL Inactive]_, _[!UICONTROL Active]_und_[!UICONTROL Ineligible]_ Tabulatoren.

1. Ansicht einer Auflistung auf einer _[!UICONTROL Products Listings]_Seite (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_und_[!UICONTROL Ineligible]_ Tabulator).

1. In _[!UICONTROL Action]_Spalte, klicken **[!UICONTROL Select]**>**[!UICONTROL Create Override]**um die Seite mit den Produktlistungen zu öffnen.

   ![Überschreiben der Amazon-Auflistung erstellen](assets/amazon-select-create-override.png)

1. Überprüfen Sie die _[!UICONTROL Listing Details]_.

1. Bestimmen Sie den Typ der Außerkraftsetzung, die Sie erstellen.

   Sie können einen einzelnen Überschreibungstyp oder eine beliebige Kombination von Typen für die Auflistung definieren (Preis, Bearbeitungszeit, Bedingung, Verkaufsmitteilungen).

   - **Preis** - Klicken **[!UICONTROL Change Listing Price]** und geben Sie Ihren festgelegten Preiswert ein für **[!UICONTROL Price Override]**.
   - **Bearbeitungszeit** - Klicken **[!UICONTROL Change Handling Time]** und geben Sie den definierten Zeitwert (in Tagen) ein für **[!UICONTROL Handling Time Override]**.
   - **Bedingung** - Klicken **[!UICONTROL Change Condition]** und wählen Sie die richtige Option für die **[!UICONTROL Condition Override]**.
   - **Hinweise für Verkäufer** - Klicken **[!UICONTROL Change Seller Notes]** und geben Sie den Hinweistext ein für **[!UICONTROL Seller Notes Override]**.

1. Klick **[!UICONTROL Save Listing Override]**.

   Die _[!UICONTROL Product Listing Overrides]_Seite wird geschlossen. Der Status der Auflistung ändert sich in `Relist in Progress`. Die Änderung wird mit der nächsten Datensynchronisierung auf Amazon veröffentlicht (wie in Ihren cron-Einstellungen konfiguriert). Die Auflistung wird ebenfalls dem_[!UICONTROL Overrides]_ Tabulator.

Das folgende Beispiel zeigt eine Außerkraftsetzung, die einen neuen Preis von `$55`, eine neue Bearbeitungszeit von `1 day`, eine neue Bedingung von `Used; Like New`und neuer Text für den Verkäufer-Hinweis.

![Beispiel-Amazon-Listenseite](assets/amazon-overrides-edit.png)

## Überschreiben für eine einzelne Auflistung bearbeiten oder entfernen {#edit-override-single-listing}

Die _[!UICONTROL Edit Overrides]_Aktion ist verfügbar, wenn Auflistungen auf der_[!UICONTROL Overrides]_ Tabulator.

1. Ansicht einer Auflistung auf _[!UICONTROL Product Listings]_Seite (_[!UICONTROL Overrides]_ Tabulator).

1. In _[!UICONTROL Action]_Spalte, klicken **[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   Die _[!UICONTROL Product Listing Overrides]_Seite wird geöffnet.

   ![Überschreiben der Amazon-Auflistung auswählen](assets/amazon-select-edit-overrides.png)

1. Überprüfen Sie die _[!UICONTROL Listing Details]_.

1. So bearbeiten Sie Ihre _[!UICONTROL Override]_-Einstellungen, legen Sie die Abschnitte für den Typ fest, den Sie ändern möchten (Preis, Bearbeitungszeit, Bedingung, Verkaufsmitteilungen).

   Um einen Überschreibungstyp unverändert zu lassen, wählen Sie `No Change To <override type>` (Standard). Mit dieser Einstellung bleibt der zuvor definierte Wert für die Außerkraftsetzung unverändert.

   - **Preis** - Klicken **[!UICONTROL Change Listing Price]** und geben Sie Ihren festgelegten Preiswert ein für **[!UICONTROL Price Override]**.
   - **Bearbeitungszeit** - Klicken **[!UICONTROL Change Handling Time]** und geben Sie den definierten Zeitwert (in Tagen) ein für **[!UICONTROL Handling Time Override]**.
   - **Bedingung** - Klicken **[!UICONTROL Change Condition]** und wählen Sie die richtige Option für **[!UICONTROL Condition Override]**.
   - **Hinweise für Verkäufer** - Klicken **[!UICONTROL Change Seller Notes]** und geben Sie den Hinweistext ein für **[!UICONTROL Seller Notes Override]**.

1. Um einen Überschreibungstyp zu entfernen, klicken Sie auf **Entfernen** für jeden Typ, den Sie entfernen möchten. Wenn der zuvor definierte Wert nicht entfernt wurde, verbleibt er in der Überschreibung.

1. Klick **[!UICONTROL Save Listing Override]**.

   Die _[!UICONTROL Product Listing Overrides]_Seite wird geschlossen. Der Status der Auflistung ändert sich in `Relist in Progress`. Die Änderung wird mit der nächsten Datensynchronisierung auf Amazon veröffentlicht (wie in Ihren cron-Einstellungen konfiguriert). Wenn diese Liste nicht bereits aufgeführt ist, werden die Auflistungen ebenfalls zu_[!UICONTROL Overrides]_ Tabulator.

Schweine auf _Überschreiben erstellen_ Beispiel. Das folgende Beispiel zeigt eine Bearbeitung der zuvor erstellten Überschreibung, die einen neuen Preis von `$50`, entfernt die Überschreibungsdauer für die Handling-Zeit und behält die vorherigen Überschreibungen für Bedingungs- und Verkäuferhinweise bei.

![Bearbeiten oder Entfernen einer Überschreibung](assets/amazon-overrides-edit-2.png)
__

## Überschreibung für mehrere Auflistungen bearbeiten oder entfernen {#edit-override-multiple-listings}

Die _[!UICONTROL Edit Listing Overrides]_Diese Aktion ist auf folgender Website verfügbar:_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ und _[!UICONTROL Ineligible]_Tabulatoren.

>[!NOTE]
>
>Da Sie Überschreibungen für mehrere Auflistungen ändern, _[!UICONTROL Listing Details]_-Abschnitt wird nicht wie bei der Änderung einer einzelnen Auflistung angezeigt.

1. Ansicht der Auflistung auf einer _[!UICONTROL Products Listings]_Seite (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ und _[!UICONTROL Ineligible]_Tabulator).

1. Aktivieren Sie das Kontrollkästchen in der linken Spalte für jede Liste, die Sie ändern möchten.

1. Unter _[!UICONTROL Actions]_, klicken **[!UICONTROL Edit Listing Overrides]**.

   Die _[!UICONTROL Product Listing Overrides]_Seite wird geöffnet.

   ![Überschreiben der Amazon-Auflistung auswählen](assets/amazon-actions-edit-listing-overrides.png)

1. So bearbeiten Sie Ihre _[!UICONTROL Override]_-Einstellungen, legen Sie die Abschnitte für den Typ fest, den Sie ändern möchten (Preis, Bearbeitungszeit, Bedingung, Verkaufsmitteilungen).

   Um das gleiche zu überschreiben, wählen Sie `No Change To <override type>` (Standard). Mit dieser Einstellung bleibt der zuvor definierte Wert für die Außerkraftsetzung unverändert.

   - **Preis** - Klicken **[!UICONTROL Change Listing Price]** und geben Sie Ihren festgelegten Preiswert ein für **[!UICONTROL Price Override]**.
   - **Bearbeitungszeit** - Klicken **[!UICONTROL Change Handling Time]** und geben Sie den definierten Zeitwert (in Tagen) ein für **[!UICONTROL Handling Time Override]**.
   - **Bedingung** - Klicken **[!UICONTROL Change Condition]** und wählen Sie die richtige Option für **[!UICONTROL Condition Override]**.
   - **Hinweise für Verkäufer** - Klicken **[!UICONTROL Change Seller Notes]** und geben Sie den Hinweistext ein für **[!UICONTROL Seller Notes Override]**.

1. Um einen Überschreibungstyp zu entfernen, klicken Sie auf **[!UICONTROL Remove]** für jeden Typ, den Sie entfernen möchten. Wenn der zuvor definierte Wert nicht entfernt wurde, verbleibt er in der Überschreibung.

1. Klick **[!UICONTROL Save Listing Override]**.

   Die _[!UICONTROL Product Listing Overrides]_Seite wird geschlossen. Der Status der Auflistungen ändert sich in `Relist in Progress`. Die Änderung wird mit der nächsten Datensynchronisierung auf Amazon veröffentlicht (wie in Ihren cron-Einstellungen konfiguriert). Wenn diese Liste nicht bereits aufgeführt ist, werden die Auflistungen ebenfalls zu_[!UICONTROL Overrides]_ Tabulator.

### Typen überschreiben

| Überschreiben | Beschreibung |
|--- |--- |
| [!UICONTROL Price Override] | Ein Preisüberschuss definiert den Preis für die Auflistungen. Diese Außerkraftsetzung hat Vorrang vor allen automatisierten Einstellungen, bis die Außerkraftsetzung entfernt wurde.<br><br>Um den Preis Ihres Produkts zu überschreiben, wählen Sie **[!UICONTROL Change Listing Price]** und geben Sie den neuen Preis ein für **[!UICONTROL Price Override]**. |
| [!UICONTROL Handling Time Override] | Eine Umschlagzeit definiert die Zeit (in Tagen) für die Verarbeitung und das Versenden von Produkten. Eine Zeitüberschreibung für die Verarbeitung hat Vorrang vor allen automatisierten und standardmäßigen Einstellungen für die Bearbeitungszeit, bis die Außerkraftsetzung entfernt wurde.<br><br>Der Wert, der im _[!UICONTROL Handling Time Override]_ist entweder Ihre standardmäßige Bearbeitungszeit, die in [Listeneinstellungen](./listing-settings.md) oder die festgelegte Überschreibungsdauer. Wenn Sie eine Verarbeitungszeit-Überschreibung entfernen, wird in der Liste standardmäßig die in Ihren Listeneinstellungen definierte Bearbeitungszeit verwendet.<br><br>Wählen Sie zum Definieren einer Überschreibungszeit **[!UICONTROL Change Handling Time]**und geben Sie die neue Bearbeitungszeit (in Tagen) ein für **[!UICONTROL Handling Time Override]**. |
| [!UICONTROL Condition Override] | Um die Listingbedingung zu überschreiben, wählen Sie **[!UICONTROL Change Condition]** und wählen Sie die neue Bedingung aus **Bedingungsüberschreiben**. |
| [!UICONTROL Seller Notes Override] | Für Produkte in Ihrem Katalog, die mit einer anderen Bedingung als `New`, kann eine Verkaufsnote hinzugefügt werden, um Ihr Produkt und seinen Zustand potenziellen Käufern näher zu erläutern. Sie können eine Außerkraftsetzung für eine Verkäuferinformation eingeben für `New` -Bedingungsprodukt, aber Amazon zeigt die Notiz nicht an.<br><br>Um die Verkäufernotizen zu überschreiben, wählen Sie **[!UICONTROL Change Seller Notes]** und geben Sie die neue Notiz ein für **[!UICONTROL Seller Notes Override]**. |
