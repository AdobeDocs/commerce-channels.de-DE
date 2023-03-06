---
title: Onboard Amazon Sales Channel
description: Erfahren Sie mehr über die Aufgaben vor der Einrichtung, Onboarding-Schritte und die Funktionsweise von Amazon mit Amazon Sales Channel in Adobe Commerce und Magento Open Source.
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Onboard Amazon Sales Channel

In diesem Abschnitt werden die Aufgaben vor der Einrichtung, das Onboarding und einige Schlüsselkonzepte für die Funktionsweise von Amazon mit dem Amazon-Vertriebskanal in Adobe Commerce und Magento Open Source beschrieben.

Die [!DNL Amazon Sales Channel] -Erweiterung unterstützt mehrere Amazon-Stores. Für eine [!DNL Amazon Seller Central] -Konto, das in der Amazon-Region USA/Kanada/Mexiko tätig ist, drei Amazon-Stores erstellen (jeweils einen für US-Verkäufe, Mexiko-Verkäufe und Kanada-Verkäufe). Jeder der drei Stores definiert das Land des Marktplatzes während seiner Erstellung. Wenn Sie mehr als eine [!DNL Amazon Seller Central] -Konto können Sie bis zu drei Amazon Stores für jeden Ihrer [!DNL Amazon Seller Central] Konten. Wenn Sie auch im Vereinigten Königreich verkaufen, hätten Sie einen vierten Amazon-Laden.

>[!TIP]
>
>A [Professional Seller-Konto](https://sell.amazon.com/){target="_blank"} on [!DNL Amazon Seller Central] in the North America or European (UK) region is required. Amazon charges a monthly subscription and fees for selling. See [Amazon: Choose your selling plan](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>Das Onboarding ist einfach: Erstellen Sie Ihren Store und verbinden Sie ihn dann mit Ihrem [!DNL Amazon Seller Central] -Konto.
>Wenn Ihr Store verbunden ist, versucht der Amazon-Kanal, Ihre Amazon-Auflistungen zu importieren und basierend auf Ihrem [Attributzuordnung](./attributes-view.md).<br><br>
>Die Einstellungen Ihres Amazon-Vertriebskanals wirken sich auf Ihre Amazon-Auflistungen aus. Ihre Erstauflistung, Preise und Produkteinstellungen sind für Sie standardmäßig festgelegt. Sie können Ihre [Store-Einstellungen](./ob-store-review.md) (Auflistung, Preise, Bestellung und Berichterstellung), nachdem Ihr Geschäft mit Ihrem [!DNL Amazon Seller Central] -Konto.

| Schritte | Was passiert? |
|--- |--- |
| [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md) | Bevor Sie an Bord gehen, müssen Sie sicherstellen, dass Sie über eine aktive und genehmigte [!DNL Amazon Seller Central] -Konto. Es gibt auch einige [!DNL Commerce] Anforderungen und Empfehlungen, die vor dem Onboarding abzuschließen sind. |
| [Überprüfen des Amazon API-Schlüssels](./amazon-verify-api-key.md) | Beim Zugriff auf den Amazon-Vertriebskanal [!DNL Commerce] überprüft und validiert automatisch den Amazon-API-Schlüssel, den Sie in Ihrer Store-Konfiguration hinzugefügt haben. Wenn Ihr API-Schlüssel nicht hinzugefügt wurde oder ungültig ist, werden Sie aufgefordert, [Amazon-API-Schlüssel hinzufügen oder aktualisieren](./amazon-verify-api-key.md). |
| [Store-Integration](./store-integration.md) | Dieser Schritt umfasst das Erstellen eines Amazon-Verkaufskanalspeichers und dessen anschließende Verbindung zu Ihrem [!DNL Amazon Seller Central] -Konto. Sie benötigen die primären Anmeldedaten für Ihre [!DNL Amazon Seller Central] -Konto (die E-Mail oder das Telefon, mit der das Verkäuferkonto erstellt wurde) für diesen Schritt. |
| [Listening-Regel erstellen](./ob-create-listing-rule.md) | Nachdem Sie Ihren Amazon-Verkaufskanalspeicher verbunden haben, werden Sie aufgefordert, eine Listening-Regel zu erstellen. Dieser Schritt wird empfohlen, Sie können ihn jedoch auch überspringen, um den Listenimport-Prozess zu starten. Sie können auch auf Ihre [Einstellungen zum Speichern und Auflisten](./ob-store-review.md) im Geschäft [Dashboard](./amazon-store-dashboard.md). |
