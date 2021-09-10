---
title: Store-Integration
description: Bevor Sie mit dem Onboarding-Prozess beginnen, müssen Sie einen Amazon-Sales Channel-Store erstellen (hinzufügen) und ihn mit Ihrem Amazon-Verkaufskonto verbinden.
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Speicherintegration

Um mit dem Amazon-Vertriebskanal zu beginnen, müssen Sie einen Amazon-Verkaufskanalspeicher erstellen (hinzufügen) und ihn mit Ihrem Amazon-Vertriebskonto verbinden. Diese beiden Schritte integrieren Ihre [!DNL Commerce]- und Amazon-Konten, um Daten freizugeben, Produkte zu synchronisieren und mehr.

_Sie benötigen die primären Anmeldedaten für Ihr  [!DNL Amazon Seller Central] Konto (die E-Mail-Adresse oder das Telefon, mit der das Verkäuferkonto erstellt wurde), um Ihren Store zu verbinden._

>[!NOTE]
>
>Nach der ersten Store-Integration werden Sie jedes Jahr aufgefordert, Ihre Amazon-Vertriebskanalverbindung zu Amazon zu erneuern, indem Sie erneut Zugriff gewähren. Sie können diese Autorisierung in der Tabelle _Aktuelle Berechtigungen_ im Abschnitt _Amazon MWS-Entwicklerberechtigungen_ der Seite **Einstellungen** > **Benutzerberechtigungen** Ihres Seller Central-Kontos verlängern oder widerrufen.

## Hinzufügen eines Amazon-Stores

1. Navigieren Sie in der Seitenleiste _Admin_ zu **Marketing** > _Kanäle_ > **Amazon-Sales Channel**.

   Wenn Sie Ihren ersten Amazon-Verkaufskanalspeicher hinzufügen, wird das Modal _Aufgaben vor der Einrichtung_ angezeigt. Nach dem Hinzufügen Ihres ersten Stores können Sie auf die Einrichtungsaufgaben auf der Seite [Amazon Sales Channel home](./amazon-sales-channel-home.md) unter _Lernen und Vorbereitung_ im Menü links zugreifen.

1. Klicken Sie auf **[!UICONTROL Add Amazon Store]**.

   Die Seite _[!UICONTROL Add Amazon sales channel]_wird geöffnet.

   ![Amazon Sales Channel Store hinzufügen](assets/amazon-store-integration.png)

1. Wählen Sie für **[!UICONTROL Magento Website to use for Amazon Listing]** aus, welche Ihrer [!DNL Commerce] Websites für diesen Amazon-Verkaufskanalspeicher verbunden werden sollen.

   Diese Einstellung definiert auch den standardmäßigen [!DNL Commerce]-Store für [den Import von Amazon-Bestellungen](./order-settings.md).

1. Geben Sie für **[!UICONTROL Email Address]** Ihre bevorzugte Kontakt-E-Mail-Adresse ein.

1. Geben Sie für **[!UICONTROL New Store Name]** einen beschreibenden Namen für den neuen Amazon-Verkaufskanalspeicher ein.

   >[!NOTE]
   >
   >Dieser Name wird nur als [!DNL Commerce]-Referenz verwendet und gibt den Store auf der Seite [Amazon Sales Channel home](./amazon-sales-channel-home.md) an. Sie möchten es so gestalten, dass Ihr Team es leicht erkennen kann. Beispielsweise könnte Ihr Amazon-Store, der in der Region USA verkauft wird, `Amazon Store USA` heißen.

1. Wählen Sie für **[!UICONTROL Amazon Marketplace Country]** die Region/das Land aus, in der dieser Amazon-Verkaufskanalspeicher Produkte verkauft. Optionen:

   - Vereinigte Staaten
   - Kanada
   - Mexiko
   - Vereinigtes Königreich

1. Gehen Sie im Abschnitt _[!UICONTROL Map your Magento attributes to Amazon]_wie folgt vor:

   - Wählen Sie für **[!UICONTROL Product ID on the Amazon market]** das Amazon-Attribut aus, das dem unten ausgewählten [!DNL Commerce]-Attribut zugeordnet werden soll.

      Diese ID hilft dabei, die entsprechenden Produkte in Ihrem [!DNL Commerce] -Katalog richtig abzugleichen.

   - Wählen Sie für **[!UICONTROL Map a Magento attribute]** das Produktattribut [!DNL Commerce] aus, das dem oben ausgewählten Amazon-Attribut zugeordnet werden soll.

      [Die Zuordnung von ](./ob-creating-magento-attributes.md) Attributen hilft sicherzustellen, dass Ihre Amazon-Liste korrekt mit dem entsprechenden Produkt in Ihrem  [!DNL Commerce] Katalog übereinstimmt.

1. Klicken Sie auf **[!UICONTROL Connect]**.

   Das Dialogfeld wird geschlossen und der neue Store wird auf der Seite [Amazon Sales Channel home](./amazon-sales-channel-home.md) mit einer Bestätigungsmeldung angezeigt.

## Verbinden eines Stores mit [!DNL Amazon Seller Central]

1. Klicken Sie im Store-Dashboard auf der Store-Karte auf **[!UICONTROL Connect store]** , um [!DNL Amazon Seller Central] in einer neuen Registerkarte zu starten.

1. Geben Sie Ihre [!DNL Amazon Seller Central]-Kontoanmeldeinformationen ein und klicken Sie auf **[!UICONTROL Sign in]**.

   Um diese Verbindung abzuschließen, müssen Sie sich bei Ihrem [!DNL Amazon Seller Central]-Konto mit den Anmeldedaten für den primären Benutzer anmelden (die E-Mail-Adresse oder das Telefon, mit der das Verkäuferkonto erstellt wurde).

1. Wenn Sie dazu aufgefordert werden, schließen Sie die Amazon-Autorisierung mit zwei Faktoren (2FA) ab, indem Sie den Code eingeben, den Sie von Amazon erhalten, und klicken Sie auf **[!UICONTROL Sign in]**.

1. Aktivieren Sie auf der Bestätigungsseite _[!UICONTROL Amazon Marketplace Web Service]_das Kontrollkästchen &quot;[!UICONTROL I understand...]&quot;und klicken Sie auf **[!UICONTROL Next]**.

1. Klicken Sie in der Meldung _[!UICONTROL You are almost done]_auf **[!UICONTROL Continue]**.

   Sie haben Amazon Sales Channel-Berechtigung für den Zugriff auf und die Freigabe von Daten für Ihr [!DNL Amazon Seller Central]-Konto erteilt. Die Amazon-Seite wird geschlossen und eine Bestätigungsmeldung wird angezeigt.

   Die Seite [Amazon Sales Channel home](./amazon-sales-channel-home.md) mit Ihren Amazon Store-Karten wird geöffnet.

   Um das Store-Dashboard anzuzeigen, klicken Sie auf der Store-Karte auf **[!UICONTROL View Store]** .

![Amazon-Vertriebskanal-Homepage mit neuer Speicherkarte](assets/asc-dashboard-after-2fa.png)

Ihr neuer Amazon-Verkaufskanalspeicher ist jetzt mit Ihrem [!DNL Amazon Seller Central]-Konto verbunden.

![Nächstes ](assets/btn-next.png) [**SymbolFahren Sie mit dem Erstellen einer Listing-Regel fort**](./ob-create-listing-rule.md)
