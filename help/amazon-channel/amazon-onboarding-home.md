---
title: "Onboard [!DNL Amazon Sales Channel]"
description: Erfahren Sie mehr über die Aufgaben vor der Einrichtung, Onboarding-Schritte und die Funktionsweise von Amazon mit Amazon Sales Channel in Adobe Commerce und Magento Open Source.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 6321f17c0e6f9e86bb3f5755dc7710fa68d68b0d
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Onboard [!DNL Amazon Sales Channel]

In diesem Abschnitt werden die Aufgaben vor der Einrichtung, das Onboarding und einige Schlüsselkonzepte für die Funktionsweise von Amazon mit dem Amazon-Vertriebskanal in Adobe Commerce und Magento Open Source beschrieben.

Die Erweiterung [!DNL Amazon Sales Channel] unterstützt mehrere Amazon Stores. Erstellen Sie für ein einzelnes [!DNL Amazon Seller Central] -Konto, das in der Region Amazon USA/Kanada/Mexiko tätig ist, drei Amazon-Stores (jeweils einen für den US-amerikanischen Vertrieb, den Mexiko-Verkauf und den Kanada-Verkauf). Jeder der drei Stores definiert das Land des Marktplatzes während seiner Erstellung. Wenn Sie mehr als ein [!DNL Amazon Seller Central] -Konto haben, können Sie für jedes Ihrer [!DNL Amazon Seller Central] -Konten über bis zu drei Amazon-Stores verfügen. Wenn Sie auch im Vereinigten Königreich verkaufen, hätten Sie einen vierten Amazon-Laden.

>[!TIP]
>
>Ein [Professional Seller-Konto](https://sell.amazon.com/){target="_blank"} auf [!DNL Amazon Seller Central] in Nordamerika oder der europäischen (UK) Region ist erforderlich. Amazon berechnet monatliche Abos und Verkaufspreise. Siehe [Amazon: Wählen Sie Ihren Verkaufsplan](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>Das Onboarding ist einfach. Erstellen Sie Ihren Store und verbinden Sie ihn dann mit Ihrem [!DNL Amazon Seller Central]-Konto.
>Wenn Ihr Store verbunden ist, versucht der Amazon-Kanal, Ihre Amazon-Listen zu importieren und basierend auf Ihrer [Attributzuordnung](./attributes-view.md) mit Ihrem Katalog abzugleichen.<br><br>
>Die Einstellungen Ihres Amazon-Vertriebskanals wirken sich auf Ihre Amazon-Auflistungen aus. Ihre Erstauflistung, Preise und Produkteinstellungen sind für Sie standardmäßig festgelegt. Sie können Ihre [Store-Einstellungen](./ob-store-review.md) (Liste, Preise, Bestellung und Berichterstellung) ändern, nachdem Ihr Store mit Ihrem [!DNL Amazon Seller Central]-Konto verbunden ist.

| Schritte | Was passiert? |
|---------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md) | Bevor Sie an Bord gehen, müssen Sie sicherstellen, dass Sie über ein aktives und genehmigtes [!DNL Amazon Seller Central] -Konto verfügen. Es gibt auch einige [!DNL Commerce] Anforderungen und Empfehlungen, die vor dem Onboarding ausgeführt werden müssen. |
| [Überprüfen des Amazon-API-Schlüssels](./amazon-verify-api-key.md) | Beim Zugriff auf den Amazon-Vertriebskanal überprüft und validiert [!DNL Commerce] automatisch den Amazon-API-Schlüssel, den Sie in Ihrer Store-Konfiguration hinzugefügt haben. Wenn Ihr API-Schlüssel nicht hinzugefügt wurde oder ungültig ist, werden Sie aufgefordert, Ihren Amazon-API-Schlüssel [hinzuzufügen oder zu aktualisieren](./amazon-verify-api-key.md). |
| [Store-Integration](./store-integration.md) | Dieser Schritt umfasst das Erstellen eines Amazon-Verkaufskanalspeichers und das anschließende Verbinden mit Ihrem [!DNL Amazon Seller Central]-Konto. Für diesen Schritt benötigen Sie die primären Anmeldedaten für Ihr [!DNL Amazon Seller Central] -Konto (die E-Mail oder das Telefon, mit der bzw. dem das Verkäuferkonto erstellt wurde). |
| [Listening-Regel erstellen](./ob-create-listing-rule.md) | Nachdem Sie Ihren Amazon-Verkaufskanalspeicher verbunden haben, werden Sie aufgefordert, eine Listening-Regel zu erstellen. Dieser Schritt wird empfohlen, Sie können ihn jedoch auch überspringen, um den Listenimport-Prozess zu starten. Sie können auch auf Ihre [Store- und Listeneinstellungen](./ob-store-review.md) im Store [Dashboard](./amazon-store-dashboard.md) zugreifen. |
