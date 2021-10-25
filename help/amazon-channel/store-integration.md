---
title: Integration speichern
description: Vor dem Beginn des Einstiegsprozesses müssen Sie einen Amazon-Sales Channel-Store erstellen (hinzufügen) und mit Ihrem Amazon-Händlerkonto verbinden.
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Integration speichern

Um mit Amazon Sales Kanal zu beginnen, müssen Sie einen Amazon Sales Kanal Store erstellen (hinzufügen) und mit Ihrem Amazon Seller-Konto verbinden. Diese beiden Schritte integrieren Ihre [!DNL Commerce] und Amazon-Konten, um Daten freizugeben, Produkte zu synchronisieren und mehr.

_Sie benötigen die primären Anmeldeberechtigungen für Ihre [!DNL Amazon Seller Central] Konto (die E-Mail oder Telefon, die zur Erstellung des Verkäuferkontos verwendet wurde), um Ihren Store zu verbinden._

>[!NOTE]
>
>Nach der Integration in den ersten Store werden Sie jährlich aufgefordert, Ihre Amazon Sales Kanal-Verbindung nach Amazon zu erneuern, indem Sie den Zugriff erneut gewähren. Sie können diese Autorisierung verlängern oder widerrufen im _Aktuelle Autorisierungen_ in der _Amazon MWS-Entwicklerberechtigungen_ Abschnitt **Einstellungen** > **Benutzerberechtigungen** Seite Ihres Seller Central-Kontos.

## Amazon-Store Hinzufügen

1. Auf _Admin_ Sidebar, Gehe zu **Marketing** > _Kanal_ > **Amazon Sales Channel**.

   Wenn Sie Ihren ersten Amazon Sales Kanal Store hinzufügen, _Aufgaben vor dem Setup_ Modal angezeigt. Nachdem Ihr erster Store hinzugefügt wurde, können Sie auf die Aufgaben vor dem Setup zugreifen auf [Amazon Sales Kanal Home](./amazon-sales-channel-home.md) Seite unter _Lernen und Vorbereitung_ im Menü links.

1. Klick **[!UICONTROL Add Amazon Store]**.

   Die _[!UICONTROL Add Amazon sales channel]_Seite wird geöffnet.

   ![hinzufügen Amazon Sales Kanal Store](assets/amazon-store-integration.png)

1. für **[!UICONTROL Magento Website to use for Amazon Listing]**, wählen Sie aus, welches Ihrer [!DNL Commerce] Websites, die für diesen Amazon Sales Kanal Store verbunden werden.

   Diese Einstellung definiert auch die Standardeinstellung [!DNL Commerce] speichern für [Amazon-Bestellungen importieren](./order-settings.md).

1. für **[!UICONTROL Email Address]**, geben Sie Ihre bevorzugte Kontakt-E-Mail-Adresse ein.

1. für **[!UICONTROL New Store Name]**, geben Sie einen beschreibenden Namen für Ihren neuen Amazon Sales Kanal Store ein.

   >[!NOTE]
   >
   >Dieser Name wird als [!DNL Commerce] nur Verweis und Identifizierung des Speichers auf [Amazon Sales Kanal Home](./amazon-sales-channel-home.md) Seite. Sie wollen etwas machen, das Ihr Team leicht erkennen kann. So könnte z. B. Ihr Amazon-Store, der in den Vereinigten Staaten verkauft wird, `Amazon Store USA`.

1. für **[!UICONTROL Amazon Marketplace Country]**, wählen Sie die Region/das Land aus, in der dieser Amazon Sales Kanal Store Produkte verkauft. Optionen:

   - Vereinigte Staaten
   - Kanada
   - Mexiko
   - Vereinigtes Königreich

1. In _[!UICONTROL Map your Magento attributes to Amazon]_führen Sie die folgenden Schritte aus:

   - für **[!UICONTROL Product ID on the Amazon market]**, wählen Sie das Amazon-Attribut aus, das dem [!DNL Commerce] Attribut unten ausgewählt.

      Diese ID hilft Ihnen, die entsprechenden Produkte in Ihrem [!DNL Commerce] Katalog.

   - für **[!UICONTROL Map a Magento attribute]**, wählen Sie [!DNL Commerce] Produktattribut, das dem oben ausgewählten Amazon-Attribut zugeordnet werden soll.

      [Zuordnungsattribute](./ob-creating-magento-attributes.md) hilft sicherzustellen, dass Ihre Amazon-Auflistung dem entsprechenden Produkt in Ihrer [!DNL Commerce] Katalog.

1. Klick **[!UICONTROL Connect]**.

   Das Dialogfeld wird geschlossen und der neue Store wird auf der [Amazon Sales Kanal Home](./amazon-sales-channel-home.md) Seite mit einer Bestätigungsmeldung.

## Laden verbinden mit [!DNL Amazon Seller Central]

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Connect store]** auf der zu startenden Speicherkarte [!DNL Amazon Seller Central] in einer neuen Registerkarte.

1. Geben Sie Ihren [!DNL Amazon Seller Central] Kontoanmeldedaten und klicken Sie auf **[!UICONTROL Sign in]**.

   Zum Abschluss dieser Verbindung müssen Sie sich bei Ihrem [!DNL Amazon Seller Central] Konto mit den Anmeldedaten des primären Benutzers (E-Mail oder Telefon, mit dem das Verkäuferkonto erstellt wurde).

1. Wenn Sie dazu aufgefordert werden, füllen Sie die Amazon-Zweifaktorengenehmigung (2FA) aus, indem Sie den Code eingeben, den Sie von Amazon erhalten, und klicken Sie auf **[!UICONTROL Sign in]**.

1. Auf _[!UICONTROL Amazon Marketplace Web Service]_Bestätigungsseite, wählen Sie die[!UICONTROL I understand...]&quot; Kontrollkästchen und klicken Sie auf **[!UICONTROL Next]**.

1. Auf _[!UICONTROL You are almost done]_Nachricht, klicken Sie **[!UICONTROL Continue]**.

   Sie haben Amazon Sales Kanal die Berechtigung zum Zugriff auf Ihre Daten und zum Teilen mit ihnen erteilt [!DNL Amazon Seller Central] Konto. Die Amazon-Seite wird geschlossen und es wird eine Bestätigungsmeldung angezeigt.

   Die [Amazon Sales Kanal Home](./amazon-sales-channel-home.md) -Seite wird geöffnet und zeigt Ihre Amazon Store-Karten an.

   Klicken Sie zur Ansicht des Store-Dashboards auf **[!UICONTROL View Store]** auf der Ladenkarte.

![Amazon Sales Kanal Home mit neuer Ladenkarte](assets/asc-dashboard-after-2fa.png)

Ihr neuer Amazon Sales Kanal Store ist jetzt mit Ihrem [!DNL Amazon Seller Central] Konto.

![Nächstes Symbol](assets/btn-next.png) [**Erstellen einer Listing-Regel fortsetzen**](./ob-create-listing-rule.md)
