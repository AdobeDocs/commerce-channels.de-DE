---
title: Onboard Amazon Sales Channel
description: Erfahren Sie mehr über die Aufgaben vor dem Setup, über die Einstiegsschritte und wie Amazon mit Amazon Sales Channel in Adobe Commerce und Magento Open Source arbeitet.
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Onboard Amazon Sales Kanal

In diesem Abschnitt werden die Aufgaben vor dem Setup, die Schritte zum Einstieg und einige wichtige Konzepte für die Funktionsweise von Amazon mit dem Amazon-Kanal in Adobe Commerce und Magento Open Source beschrieben.

Die [!DNL Amazon Sales Channel] Extension unterstützt mehrere Amazon Stores. Für eine [!DNL Amazon Seller Central] ein Konto, das in der Amazon-Region USA/Kanada/Mexiko tätig ist, drei Amazon-Stores (je einer für den US-amerikanischen Verkauf, den mexikanischen Verkauf und den kanadischen Vertrieb) errichtet. Jeder der drei Läden definiert das Marktland während seiner Gründung. Wenn Sie mehr als eine [!DNL Amazon Seller Central] können Sie bis zu drei Amazon-Stores für jeden Ihrer [!DNL Amazon Seller Central] Konten. Wenn man auch in Großbritannien verkauft, hätte man einen vierten Amazon-Laden.

>[!TIP]
>
>A [Konto für gewerbliche Verkäufer](https://sell.amazon.com/){Zielgruppe=&quot;_blank&quot;} auf [!DNL Amazon Seller Central] in Nordamerika oder in der europäischen Region (UK) erforderlich ist. Amazon berechnet monatlich ein Abonnement und Verkaufsgebühren. Siehe [Amazon: Wählen Sie Ihren Verkaufsplan aus](https://sell.amazon.com/pricing.html){Zielgruppe=&quot;_blank&quot;}.<br><br>
>Einstieg ganz einfach: Erstellen Sie einen Store und verbinden Sie ihn dann mit Ihrem [!DNL Amazon Seller Central] Konto.
>Wenn Ihr Store verbunden ist, versucht der Amazon Kanal, Ihre Amazon-Auflistungen zu importieren und mit Ihrem Katalog abzustimmen, basierend auf Ihrer [Attributzuordnung](./attributes-view.md).<br><br>
>Ihre Amazon Sales Kanal-Einstellungen wirken sich auf Ihre Amazon-Auflistungen aus. Ihre anfänglichen Listen-, Preis- und Produkteinstellungen sind standardmäßig für Sie festgelegt. Sie können Ihre [Speichereinstellungen](./ob-store-review.md) (Auflisten, Preise, Bestellung und Berichte), nachdem Ihr Store mit Ihrem [!DNL Amazon Seller Central] Konto.

| Schritte | Ereignisse |
|--- |--- |
| [Aufgaben vor dem Setup](./amazon-pre-setup-tasks.md) | Bevor Sie an Bord gehen, müssen Sie sicherstellen, dass Sie über einen aktiven und genehmigten [!DNL Amazon Seller Central] Konto. Es gibt auch einige [!DNL Commerce] Anforderungen und Empfehlungen, die vor dem Einsteigen abzuschließen sind. |
| [Überprüfen Sie den Amazon API-Schlüssel](./amazon-verify-api-key.md) | beim Zugriff auf Amazon Sales Kanal, [!DNL Commerce] überprüft und validiert automatisch den Amazon API-Schlüssel, den Sie in Ihrer Store-Konfiguration hinzugefügt haben. Wenn Ihr API-Schlüssel nicht hinzugefügt wurde oder ungültig ist, werden Sie aufgefordert, [Amazon API-Schlüssel hinzufügen oder aktualisieren](./amazon-verify-api-key.md). |
| [Integration speichern](./store-integration.md) | Dieser Schritt umfasst die Erstellung eines Amazon Sales Kanal Store und die anschließende Verbindung zu Ihrem [!DNL Amazon Seller Central] Konto. Sie benötigen die primären Anmeldeberechtigungen für Ihre [!DNL Amazon Seller Central] Konto (die E-Mail oder das Telefon, mit der das Verkäuferkonto erstellt wurde) für diesen Schritt. |
| [Listungsregel erstellen](./ob-create-listing-rule.md) | Nachdem Sie Ihren Amazon Sales Kanal Store verbunden haben, werden Sie aufgefordert, eine Listungsregel zu erstellen. Dieser Schritt wird empfohlen, Sie können ihn aber auch überspringen, um den Prozess für den Import der Liste Beginn. Sie haben auch Zugriff auf [Einstellungen speichern und auflisten](./ob-store-review.md) im Geschäft [Dashboard](./amazon-store-dashboard.md). |
