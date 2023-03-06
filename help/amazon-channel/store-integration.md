---
title: Store-Integration
description: Bevor Sie mit dem Onboarding-Prozess beginnen, müssen Sie einen Amazon-Sales Channel-Store erstellen (hinzufügen) und ihn mit Ihrem Amazon-Verkaufskonto verbinden.
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Store-Integration

Um mit dem Amazon-Vertriebskanal zu beginnen, müssen Sie einen Amazon-Verkaufskanalspeicher erstellen (hinzufügen) und ihn mit Ihrem Amazon-Vertriebskonto verbinden. Diese beiden Schritte integrieren Ihre [!DNL Commerce] und Amazon-Konten verwenden, um Daten freizugeben, Produkte zu synchronisieren und mehr.

_Sie benötigen die primären Anmeldedaten für Ihre [!DNL Amazon Seller Central] -Konto (die E-Mail oder das Telefon, mit der das Verkäuferkonto erstellt wurde), um Ihr Geschäft zu verbinden._

>[!NOTE]
>
>Nach der ersten Store-Integration werden Sie jedes Jahr aufgefordert, Ihre Amazon-Vertriebskanalverbindung zu Amazon zu erneuern, indem Sie erneut Zugriff gewähren. Sie können diese Autorisierung im _Aktuelle Berechtigungen_ in der _Amazon MWS-Entwicklerberechtigungen_ Abschnitt **Einstellungen** > **Benutzerberechtigungen** Seite Ihres Seller Central-Kontos.

## Hinzufügen eines Amazon-Stores

1. Im _Admin_ Seitenleiste, navigieren Sie zu **Marketing** > _Kanäle_ > **Amazon Sales Channel**.

   Wenn Sie Ihren ersten Amazon-Verkaufskanalspeicher hinzufügen, wird die _Aufgaben vor der Einrichtung_ modal angezeigt. Nachdem Ihr erster Store hinzugefügt wurde, können Sie auf Aufgaben vor der Einrichtung über die [Amazon-Vertriebskanal - Startseite](./amazon-sales-channel-home.md) Seite unter _Lernen und Vorbereitung_ im Menü links.

1. Klicken **[!UICONTROL Add Amazon Store]**.

   Die _[!UICONTROL Add Amazon sales channel]_Seite geöffnet.

   ![Amazon Sales Channel Store hinzufügen](assets/amazon-store-integration.png)

1. Für **[!UICONTROL Magento Website to use for Amazon Listing]**, wählen Sie aus, welche Ihrer [!DNL Commerce] Websites zur Verbindung für diesen Amazon-Verkaufskanalspeicher.

   Diese Einstellung definiert auch die Standardeinstellung [!DNL Commerce] Store für [Importieren von Amazon-Bestellungen](./order-settings.md).

1. Für **[!UICONTROL Email Address]** Geben Sie Ihre bevorzugte Kontakt-E-Mail-Adresse ein.

1. Für **[!UICONTROL New Store Name]** Geben Sie einen beschreibenden Namen für Ihren neuen Amazon-Verkaufskanalspeicher ein.

   >[!NOTE]
   >
   >Dieser Name wird als [!DNL Commerce] nur auf und identifiziert den Store auf der [Amazon-Vertriebskanal - Startseite](./amazon-sales-channel-home.md) Seite. Sie möchten es so gestalten, dass Ihr Team es leicht erkennen kann. Ihr Amazon-Store, der in der Region USA verkauft wird, könnte beispielsweise `Amazon Store USA`.

1. Für **[!UICONTROL Amazon Marketplace Country]** wählen Sie die Region/das Land aus, in der dieser Amazon-Verkaufskanalspeicher Produkte verkauft. Optionen:

   - Vereinigte Staaten
   - Kanada
   - Mexiko
   - Vereinigtes Königreich

1. Im _[!UICONTROL Map your Magento attributes to Amazon]_führen Sie folgende Schritte aus:

   - Für **[!UICONTROL Product ID on the Amazon market]**, wählen Sie das Amazon-Attribut aus, das der [!DNL Commerce] Attribut unten ausgewählt ist.

      Diese ID hilft bei der korrekten Übereinstimmung der entsprechenden Produkte in Ihrer [!DNL Commerce] Katalog.

   - Für **[!UICONTROL Map a Magento attribute]**, wählen Sie die [!DNL Commerce] Produktattribut, das dem oben ausgewählten Amazon-Attribut zugeordnet werden soll.

      [Zuordnen von Attributen](./ob-creating-magento-attributes.md) hilft sicherzustellen, dass Ihre Amazon-Liste korrekt mit dem entsprechenden Produkt in Ihrer [!DNL Commerce] Katalog.

1. Klicken **[!UICONTROL Connect]**.

   Das Dialogfeld wird geschlossen und der neue Store wird auf der [Amazon-Vertriebskanal - Startseite](./amazon-sales-channel-home.md) Seite mit einer Bestätigungsmeldung.

## Schließen Sie einen Store an [!DNL Amazon Seller Central]

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Connect store]** auf der Store-Karte, die gestartet werden soll [!DNL Amazon Seller Central] in einer neuen Registerkarte.

1. Geben Sie Ihre [!DNL Amazon Seller Central] Kontoanmeldeinformationen und klicken Sie auf **[!UICONTROL Sign in]**.

   Um diese Verbindung abzuschließen, müssen Sie sich bei Ihrer [!DNL Amazon Seller Central] Konto mit den Anmeldedaten für den primären Benutzer (die E-Mail oder das Telefon, die bzw. das zum Erstellen des Verkäuferkontos verwendet wurde).

1. Wenn Sie dazu aufgefordert werden, schließen Sie die Amazon-Autorisierung mit zwei Faktoren (2FA) ab, indem Sie den Code eingeben, den Sie von Amazon erhalten, und klicken Sie auf **[!UICONTROL Sign in]**.

1. Im _[!UICONTROL Amazon Marketplace Web Service]_Bestätigungsseite wählen Sie die[!UICONTROL I understand...]&quot;und klicken Sie auf **[!UICONTROL Next]**.

1. Im _[!UICONTROL You are almost done]_Meldung, klicken Sie auf **[!UICONTROL Continue]**.

   Sie haben Amazon Sales Channel-Berechtigung für den Zugriff auf und die Freigabe von Daten für Ihre [!DNL Amazon Seller Central] -Konto. Die Amazon-Seite wird geschlossen und eine Bestätigungsmeldung wird angezeigt.

   Die [Amazon-Vertriebskanal - Startseite](./amazon-sales-channel-home.md) wird angezeigt, auf der Ihre Amazon Store-Karten angezeigt werden.

   Um das Store-Dashboard anzuzeigen, klicken Sie auf **[!UICONTROL View Store]** auf der Speicherkarte.

![Amazon-Vertriebskanal-Homepage mit neuer Speicherkarte](assets/asc-dashboard-after-2fa.png)

Ihr neuer Amazon-Verkaufskanalspeicher ist jetzt mit Ihrem [!DNL Amazon Seller Central] -Konto.

![Nächstes Symbol](assets/btn-next.png) [**Fahren Sie mit dem Erstellen einer Listing-Regel fort.**](./ob-create-listing-rule.md)
