---
title: Erstellen und Bearbeiten von Außerkraftsetzungen des Amazon-Vertriebskanals
description: Verwenden Sie Amazon-Sales Channel-Überschreibungen, um Ihre Änderungen auf eine einzelne Amazon-Liste oder auf mehrere Auflistungen anzuwenden.
feature: Sales Channels, Products, Configuration
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Erstellen und Bearbeiten von Überschreibungen

Sie können eine Liste erstellen und überschreiben oder eine auf eine Liste angewendete Überschreibung bearbeiten oder entfernen. Überschreibt einen definierten Wert für eine bestimmte Auflistung.

## Erstellen einer Überschreibung für eine einzelne Liste

Die Aktion _[!UICONTROL Create Override]_ist verfügbar, wenn Sie Listen auf den Registerkarten_[!UICONTROL Inactive]_, _[!UICONTROL Active]_und_[!UICONTROL Ineligible]_ anzeigen.

1. Zeigen Sie eine Liste auf einer _[!UICONTROL Products Listings]_-Seite an ( Registerkarte_[!UICONTROL Inactive]_, _[!UICONTROL Active]_und_[!UICONTROL Ineligible]_).

1. Klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**>**[!UICONTROL Create Override]**, um die Seite &quot;Produktlistenüberschreibungen&quot;zu öffnen.

   ![Amazon-Listenüberschreibungen erstellen](assets/amazon-select-create-override.png){width="220"}

1. Um sicherzustellen, dass Sie die richtige Liste anzeigen, überprüfen Sie die _[!UICONTROL Listing Details]_.

1. Bestimmen Sie den Typ der Überschreibung, die Sie erstellen.

   Sie können einen einzelnen Überschreibungstyp oder eine beliebige Kombination von Typen für die Auflistung definieren (Preis, Bearbeitungszeit, Bedingung, Verkaufshinweise).

   - **Preis** - Klicken Sie auf **[!UICONTROL Change Listing Price]** und geben Sie Ihren definierten Preiswert für **[!UICONTROL Price Override]** ein.
   - **Handling Time** - Klicken Sie auf **[!UICONTROL Change Handling Time]** und geben Sie den definierten Zeitwert (in Tagen) für **[!UICONTROL Handling Time Override]** ein.
   - **Bedingung** - Klicken Sie auf **[!UICONTROL Change Condition]** und wählen Sie die richtige Option für den **[!UICONTROL Condition Override]** aus.
   - **Verkaufshinweise** - Klicken Sie auf **[!UICONTROL Change Seller Notes]** und geben Sie Ihren Notiztext für **[!UICONTROL Seller Notes Override]** ein.

1. Klicken Sie auf **[!UICONTROL Save Listing Override]**.

   Die Seite _[!UICONTROL Product Listing Overrides]_wird geschlossen. Der Status der Auflistung ändert sich in `Relist in Progress`. Die Änderung wird mit der nächsten Datensynchronisation in Amazon veröffentlicht (wie in Ihren Cron-Einstellungen konfiguriert). Die Auflistung wird auch der Registerkarte_[!UICONTROL Overrides]_ hinzugefügt.

Das folgende Beispiel zeigt eine Außerkraftsetzung, die einen neuen Preis von `$55`, eine neue Bearbeitungszeit von `1 day`, eine neue Bedingung von `Used; Like New` und einen neuen Text für die Verkaufsnotiz definiert.

![Beispiel für Amazon-Listenüberschreibungen](assets/amazon-overrides-edit.png){width="600" zoomable="yes"}

## Bearbeiten oder Entfernen einer Überschreibung für eine einzelne Auflistung {#edit-override-single-listing}

Die Aktion _[!UICONTROL Edit Overrides]_ist verfügbar, wenn Sie Listen auf der Registerkarte_[!UICONTROL Overrides]_ anzeigen.

1. Zeigen Sie eine Liste auf der Seite _[!UICONTROL Product Listings]_an ( Registerkarte_[!UICONTROL Overrides]_ ).

1. Klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   Die Seite _[!UICONTROL Product Listing Overrides]_wird geöffnet.

   ![Wählen Sie eine Amazon-Listenüberschreibungen aus](assets/amazon-select-edit-overrides.png){width="125"}

1. Um sicherzustellen, dass Sie die richtige Liste überschreiben, überprüfen Sie die _[!UICONTROL Listing Details]_.

1. Um Ihre _[!UICONTROL Override]_-Einstellungen zu bearbeiten, definieren Sie die Abschnitte für den Typ, den Sie ändern möchten (Preis, Bearbeitungszeit, Bedingung, Verkaufshinweise).

   Um den gleichen Überschreibungstyp beizubehalten, wählen Sie &quot;`No Change To <override type>`&quot;(Standardeinstellung). Bei dieser Einstellung bleibt der zuvor definierte Wert zum Außerkraftsetzen unverändert.

   - **Preis** - Klicken Sie auf **[!UICONTROL Change Listing Price]** und geben Sie Ihren definierten Preiswert für **[!UICONTROL Price Override]** ein.
   - **Handling Time** - Klicken Sie auf **[!UICONTROL Change Handling Time]** und geben Sie den definierten Zeitwert (in Tagen) für **[!UICONTROL Handling Time Override]** ein.
   - **Bedingung** - Klicken Sie auf **[!UICONTROL Change Condition]** und wählen Sie die richtige Option für **[!UICONTROL Condition Override]** aus.
   - **Verkaufshinweise** - Klicken Sie auf **[!UICONTROL Change Seller Notes]** und geben Sie Ihren Notiztext für **[!UICONTROL Seller Notes Override]** ein.

1. Um einen Überschreibungstyp zu entfernen, klicken Sie für jeden zu entfernenden Typ auf **Entfernen** . Wenn der zuvor definierte Wert nicht entfernt wird, bleibt er in der Überschreibung.

1. Klicken Sie auf **[!UICONTROL Save Listing Override]**.

   Die Seite _[!UICONTROL Product Listing Overrides]_wird geschlossen. Der Status der Auflistung ändert sich in `Relist in Progress`. Die Änderung wird mit der nächsten Datensynchronisation in Amazon veröffentlicht (wie in Ihren Cron-Einstellungen konfiguriert). Wenn diese nicht bereits aufgeführt sind, werden die Listen auch der Registerkarte_[!UICONTROL Overrides]_ hinzugefügt.

Piggyback für das Beispiel _Erstellen einer Überschreibung_. Das folgende Beispiel zeigt eine Bearbeitung der zuvor erstellten Überschreibung, die einen neuen Preis von `$50` definiert, die Außerkraftsetzung der Handling-Zeit entfernt und die vorherigen Bedingungen und Verkaufshinweise außer Kraft setzt.

![Bearbeiten oder Entfernen einer Überschreibung](assets/amazon-overrides-edit-2.png){width="600" zoomable="yes"}
__

## Bearbeiten oder Entfernen einer Überschreibung für mehrere Listen {#edit-override-multiple-listings}

Die Aktion _[!UICONTROL Edit Listing Overrides]_ist auf den Registerkarten_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ und _[!UICONTROL Ineligible]_verfügbar.

>[!NOTE]
>
>Da Sie Überschreibungen für mehrere Auflistungen ändern, wird der Abschnitt &quot;_[!UICONTROL Listing Details]_&quot;nicht so angezeigt wie beim Ändern einer einzelnen Liste.

1. Zeigen Sie die Liste auf einer _[!UICONTROL Products Listings]_-Seite an ( Registerkarte_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ und _[!UICONTROL Ineligible]_).

1. Aktivieren Sie das Kontrollkästchen in der linken Spalte für jede Liste, die Sie ändern möchten.

1. Klicken Sie unter _[!UICONTROL Actions]_auf **[!UICONTROL Edit Listing Overrides]**.

   Die Seite _[!UICONTROL Product Listing Overrides]_wird geöffnet.

   ![Wählen Sie eine Amazon-Listenüberschreibungen aus](assets/amazon-actions-edit-listing-overrides.png){width="200"}

1. Um Ihre _[!UICONTROL Override]_-Einstellungen zu bearbeiten, definieren Sie die Abschnitte für den Typ, den Sie ändern möchten (Preis, Bearbeitungszeit, Bedingung, Verkaufshinweise).

   Um dasselbe zu überschreiben, wählen Sie `No Change To <override type>` (Standard) aus. Bei dieser Einstellung bleibt der zuvor definierte Wert zum Außerkraftsetzen unverändert.

   - **Preis** - Klicken Sie auf **[!UICONTROL Change Listing Price]** und geben Sie Ihren definierten Preiswert für **[!UICONTROL Price Override]** ein.
   - **Handling Time** - Klicken Sie auf **[!UICONTROL Change Handling Time]** und geben Sie den definierten Zeitwert (in Tagen) für **[!UICONTROL Handling Time Override]** ein.
   - **Bedingung** - Klicken Sie auf **[!UICONTROL Change Condition]** und wählen Sie die richtige Option für **[!UICONTROL Condition Override]** aus.
   - **Verkaufshinweise** - Klicken Sie auf **[!UICONTROL Change Seller Notes]** und geben Sie Ihren Notiztext für **[!UICONTROL Seller Notes Override]** ein.

1. Um einen Überschreibungstyp zu entfernen, klicken Sie für jeden zu entfernenden Typ auf **[!UICONTROL Remove]** . Wenn der zuvor definierte Wert nicht entfernt wird, bleibt er in der Überschreibung.

1. Klicken Sie auf **[!UICONTROL Save Listing Override]**.

   Die Seite _[!UICONTROL Product Listing Overrides]_wird geschlossen. Der Status der Auflistungen ändert sich in `Relist in Progress`. Die Änderung wird mit der nächsten Datensynchronisation in Amazon veröffentlicht (wie in Ihren Cron-Einstellungen konfiguriert). Wenn diese nicht bereits aufgeführt sind, werden die Listen auch der Registerkarte_[!UICONTROL Overrides]_ hinzugefügt.

### Typen überschreiben

| Überschreibung | Beschreibung |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Override] | Ein Preisüberschreiben definiert den Preis für die Auflistungen. Diese Überschreibung hat Vorrang vor allen automatisierten Einstellungen, bis die Überschreibung entfernt wird.<br><br>Um den Preis Ihres Produkts zu überschreiben, wählen Sie **[!UICONTROL Change Listing Price]** und geben Sie den neuen Preis für **[!UICONTROL Price Override]** ein. |
| [!UICONTROL Handling Time Override] | Eine Umschlagszeit-Überschreibung definiert die Zeit (in Tagen), die für die Verarbeitung und das Versenden von Produkten benötigt wird. Eine Überschreibungszeit hat Vorrang vor allen automatisierten und standardmäßigen Verarbeitungszeiteinstellungen, bis die Überschreibung entfernt wird.<br><br>Der Wert, der im Feld _[!UICONTROL Handling Time Override]_vorhanden ist, ist entweder die standardmäßige Bearbeitungszeit, die Sie in Ihren [Listeneinstellungen](./listing-settings.md) festgelegt haben, oder die von Ihnen definierte Verarbeitungszeit für die Außerkraftsetzung. Wenn Sie eine Zeitüberschreitung bei der Verarbeitung entfernen, wird standardmäßig die in Ihren Listeneinstellungen definierte Bearbeitungszeit verwendet.<br><br>Wählen Sie **[!UICONTROL Change Handling Time]**aus und geben Sie die neue Bearbeitungszeit (in Tagen) für **[!UICONTROL Handling Time Override]**ein, um eine Überschreibungszeit für die Bearbeitungszeit festzulegen. |
| [!UICONTROL Condition Override] | Um die Auflistungsbedingung zu überschreiben, wählen Sie &quot;**[!UICONTROL Change Condition]**&quot;und wählen Sie die neue Bedingung unter &quot;**Bedingungsüberschreibungen**&quot;aus. |
| [!UICONTROL Seller Notes Override] | Für Produkte in Ihrem Katalog, die mit einer anderen Bedingung als `New` definiert sind, kann eine Verkaufsnote hinzugefügt werden, in der Ihr Produkt und seine Bedingung für potenzielle Käufer detailliert beschrieben werden. Sie können eine Außerkraftsetzung der Verkaufsnotiz für ein &quot;`New`&quot;-Bedingungsprodukt eingeben, Amazon zeigt die Notiz jedoch nicht an.<br><br>Um die Verkaufshinweise zu überschreiben, wählen Sie **[!UICONTROL Change Seller Notes]** und geben Sie die neue Notiz für **[!UICONTROL Seller Notes Override]** ein. |
