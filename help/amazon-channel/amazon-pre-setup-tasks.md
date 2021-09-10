---
title: Aufgaben vor der Einrichtung
description: Überprüfen Sie die erforderlichen Aufgaben, bevor Sie Ihren Adobe Commerce- oder Magento Open Source-Speicher in Amazon Sales Channel integrieren.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Aufgaben vor der Einrichtung

Vor [Store-Integration](./store-integration.md) müssen Sie sicherstellen, dass Ihr [!DNL Amazon Seller Central]-Konto und Ihr [!DNL Commerce]-Konto für die Integration bereit sind. Für eine erfolgreiche Integration sind einige Aufgaben vor der Einrichtung erforderlich.

Wenn Sie Ihren ersten Amazon Store im Amazon-Vertriebskanal einrichten, wird eine Liste mit Einrichtungsaufgaben angezeigt. Es wird empfohlen, diese Aufgaben zu überprüfen, bevor Sie [einen Amazon Store ](./store-integration.md) hinzufügen. Nachdem Sie Ihren ersten Store hinzugefügt haben, können Sie diese Aufgaben in der Ansicht &quot;Learning and Preparation&quot;des Amazon-Vertriebskanals [Homepage](./amazon-sales-channel-home.md) überprüfen.

## 1. Aktivieren Sie Hintergrundaufgaben in [!DNL Commerce].

Alle zwischen [!DNL Commerce] und Amazon synchronisierten Produkte und Daten werden von einem [cron-Auftrag](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;} verwaltet. Wenn Sie Aufgaben wie das Hinzufügen oder Aktualisieren von Auflistungen und den Empfang von Bestellungen abschließen, sendet und empfängt ein Cron-Auftrag Daten zwischen Ihrem [!DNL Commerce]-Backend und Ihrem [!DNL Amazon Seller Central]-Konto.

- [ [!DNL Commerce] Aktiviert](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}.

- Um die maximale Leistung zu erzielen, wird [set [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target=&quot;_blank&quot;} alle fünf Minuten einmal ausgeführt.

## 2. Erstellen Sie Ihr [!DNL Amazon Seller Central]-Konto.

Bevor Sie mit der Einrichtung Ihres Amazon-Vertriebskanals beginnen, müssen Sie über ein aktives [!DNL Amazon Seller Central]-Konto verfügen. Wenn Sie kein Amazon-Verkaufskonto in der Region [Nordamerika (USA, CA, MX)](https://sell.amazon.com/){target=&quot;_blank&quot;} oder [Europa (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target=&quot;_blank&quot;} haben, können Sie den Einrichtungsprozess für das Kundenkonto von Amazon abschließen.

Für den Amazon-Vertriebskanal ist ein [!DNL Professional Seller] -Konto für [!DNL Amazon Seller Central] erforderlich. Amazon berechnet monatliche Abos und Verkaufspreise. Siehe [Amazon: Wählen Sie Ihren Verkaufsplan](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}.

## 3. Stellen Sie sicher, dass Sie ein zugelassener Amazon-Verkäufer sind.

Zur Integration benötigen Sie ein genehmigtes [!DNL Amazon Seller Central]-Konto. Für Ihr Konto dürfen keine Einschränkungen für Produkte oder Kategorien gelten. Einige Produkte und Kategorien müssen vor der Erstellung von Listen genehmigt werden. Überprüfen Sie die Amazon-Richtlinien für Kategorie- und Produktgenehmigungen, um sicherzustellen, dass Ihre Produkte genehmigt sind. Siehe [Amazon: Kategorien und Produkte, für die eine Genehmigung erforderlich ist](https://sellercentral.amazon.com/gp/help/200333160){target=&quot;_blank&quot;} (Anmeldung von Seller Central erforderlich).

Außerdem müssen Sie sicherstellen, dass Sie Folgendes in Ihrem [!DNL Amazon Seller Central]-Konto konfiguriert haben:

- Stellen Sie sicher, dass Ihre Rückkehrrichtlinie genauso gut oder besser ist wie die Amazon-Rückgaberichtlinie. Siehe [Amazon: Rückgaberichtlinie](https://www.amazon.com/gp/help/customer/display.html){target=&quot;_blank&quot;}.

- Stellen Sie sicher, dass Ihre Steuereinstellungen konfiguriert sind. Siehe [Amazon: Steuerrichtlinien](https://sellercentral.amazon.com/gp/help/external/help.html){target=&quot;_blank&quot;} (Anmeldung von Seller Central erforderlich).

- Stellen Sie sicher, dass Ihre Versandmethoden korrekt konfiguriert sind. Um die Versandmethoden einzurichten, die den Kunden [!DNL Commerce] zur Erfüllung Ihrer Amazon-Bestellungen angeboten werden, aktualisieren Sie [Amazon: Versandeinstellungen](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target=&quot;_blank&quot;} in Ihrem [!DNL Amazon Seller Central]-Konto.

## 4. Stellen Sie sicher, dass Ihre Mehrwertsteuer für Ihre Geschäfte konfiguriert ist.

(Wird hauptsächlich von britischen Verkäufern verwendet.) Amazon empfiehlt, sich für den [Amazon-Mehrwertsteuerberechnungsdienst](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target=&quot;_blank&quot;} anzumelden. Wenn Sie eine andere Methode wählen, sind Sie für die Einhaltung der Mehrwertsteuer verantwortlich.

>[!NOTE]
>
>Es kann 10-14 Tage dauern, bis Amazon Ihr Konto für den MwSt-Berechnungsdienst überprüft und aktiviert.

## 5. Anzahl der automatischen Katalogübereinstimmungen erhöhen

Beim Onboarding verwendet der Amazon-Verkaufskanal Produktattribute, um Ihre bestehenden Amazon-Auflistungen (falls zutreffend) mit vorhandenen Produkten in Ihrem [!DNL Commerce]-Katalog abzugleichen. Nach dem Onboarding werden diese Produktattribute verwendet, um Ihre [!DNL Commerce] -Katalogelemente in einer Amazon-Liste zu veröffentlichen und Ihre Produktdaten zwischen [!DNL Commerce] und Amazon zu synchronisieren.

Damit die höchste Anzahl von [!DNL Commerce]-Produkten automatisch mit Amazon-Auflistungen übereinstimmt, sollten Sie eine Reihe von Produktattributen für Ihren [!DNL Commerce]-Katalog erstellen. Bevor Sie Ihren Amazon-Verkaufskanalspeicher einrichten, sollten Sie [!DNL Commerce] -Produktattribute hinzufügen, die diesen Amazon-Attributen entsprechen, z. B.: ASIN, EAN, ISBN, UPC oder GCID. Siehe [Erstellen eines Produktattributs in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Konfigurieren Sie Ihre Währung und Konversion (nach Bedarf).

Wenn Ihr Amazon-Store eine andere Währung verwendet als für Ihren [!DNL Commerce]-Store konfiguriert ist, aktivieren Sie [die Währung](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;} und legen Sie die [Währungsumrechnungsrate](https://docs.magento.com/user-guide/stores/currency-update.html){target=&quot;_blank&quot;} fest.

## 7. Erstellen Sie nach Bedarf ein Attribut für die Produktbedingung .

Wenn Ihre Amazon-Listen mehr als eine Produktbedingung enthalten (z. B. _new_, _used_ oder _like new_), erstellen Sie ein [!DNL Commerce] -Attribut und weisen Sie Bedingungswerte zu. Sie müssen dieses Attribut beim Onboarding dem Amazon Condition-Produktattribut zuordnen. Siehe [Erstellen von Attributen für Amazon](./ob-creating-magento-attributes.md).

## 8. Konfigurieren Sie Ihre Versandmethode [!DNL Amazon Seller Central] .

Informationen zum Einrichten von Versandmethoden, die Sie zur Erfüllung Ihrer Amazon-Bestellungen anbieten möchten, finden Sie unter [Einstellungen und Versandeinstellungen][10] in Ihrem [!DNL Amazon Seller Central]-Konto.

## Zusätzliche Konfigurationen

Wenn Ihr Amazon-Konto eingerichtet und aktiv ist, gibt es mehrere [!DNL Commerce] Empfehlungen, die den Onboarding-Prozess für den Amazon-Verkaufskanal optimieren.

### Überprüfen und notieren Sie alle Produkte, die Sie ausschließen möchten

Möglicherweise möchten Sie nicht, dass einige Produkte in Amazon aufgeführt werden. Der Amazon-Vertriebskanal verfügt über eine Regel-Engine, mit der bestimmt wird, welche Produkte in Amazon veröffentlicht werden dürfen. [Mit ](./listing-rules.md) Listening-Regeln können Sie Teilmengen von Produkten auswählen, die in Ihrem  [!DNL Amazon Seller Central] Konto veröffentlicht werden sollen (oder nicht veröffentlicht werden), z. B. durch Kategorieauswahl oder Definition eines oder mehrerer Produktattribute. Wie [!DNL Commerce] [catalog](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;} oder [Warenkorb](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;} Preisregeln, müssen für Produktattribute, die für die Amazon-Listenberechtigung verwendet werden, **[!UICONTROL Use for Promo Rule Conditions]** auf `Yes` gesetzt sein. Siehe **[!UICONTROL Use for Promo Rule Conditions]** in [Produktattribute](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}.

### Legen Sie die Region [!DNL Amazon Seller Central] auf &quot;Inaktiv&quot;fest

Um den fehlerfreien Datenübergang während der Integration zu erleichtern, wird empfohlen, den Amazon-Bereich unter Einstellungen > Kontoinformationen > Urlaubseinstellungen auf den Status `Inactive` zu setzen. Siehe [Amazon: Listening-Status für Urlaub][11]. Wenn Ihre Einrichtung abgeschlossen ist, ändern Sie den Status in Amazon wieder in `Active`.

![Nächstes ](assets/btn-next.png) [**SymbolFahren Sie mit dem Erstellen von  [!DNL Commerce] Attributen fort.**](./ob-creating-magento-attributes.md)
