---
title: Aufgaben vor der Einrichtung für  [!DNL Amazon sales channel]
description: Überprüfen Sie die erforderlichen Aufgaben, bevor Sie Ihren Adobe Commerce- oder Magento Open Source-Store in Amazon Sales Channel integrieren.
role: Admin, Developer
feature: Sales Channels, Install, Configuration
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Aufgaben vor der Einrichtung für [!DNL Amazon sales channel]

Vor der [Store-Integration](./store-integration.md) müssen Sie sicherstellen, dass Ihr [!DNL Amazon Seller Central]-Konto und Ihr [!DNL Commerce]-Konto für die Integration bereit sind. Für eine erfolgreiche Integration sind einige Aufgaben vor der Einrichtung erforderlich.

Wenn Sie Ihren ersten Amazon Store im Amazon-Vertriebskanal einrichten, wird eine Liste mit Einrichtungsaufgaben angezeigt. Es wird empfohlen, diese Aufgaben zu überprüfen, bevor Sie [einen Amazon-Store hinzufügen](./store-integration.md). Nachdem Sie Ihren ersten Store hinzugefügt haben, können Sie diese Aufgaben in der Ansicht &quot;Lernen und Vorbereitung&quot;des Amazon-Vertriebskanals [Homepage](./amazon-sales-channel-home.md) ansehen.

## 1. Hintergrundaufgaben in [!DNL Commerce] aktivieren

Alle zwischen [!DNL Commerce] und Amazon synchronisierten Produkte und Daten werden von einem [Cron-Auftrag](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) verwaltet. Wenn Sie Aufgaben wie das Hinzufügen oder Aktualisieren von Auflistungen und den Empfang von Bestellungen abschließen, sendet und empfängt ein Cron-Auftrag Daten zwischen Ihrem [!DNL Commerce] -Backend und Ihrem [!DNL Amazon Seller Central] -Konto.

- [Aktivieren Sie [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html).

- Um die maximale Leistung zu erzielen, setzen Sie [cron](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/system.html) auf einmal alle fünf Minuten. [!DNL Commerce] 

## 2. Erstellen Sie Ihr [!DNL Amazon Seller Central]-Konto

Bevor Sie mit der Einrichtung Ihres Amazon-Verkaufskanals beginnen, müssen Sie über ein aktives [!DNL Amazon Seller Central] -Konto verfügen. Wenn Sie kein Amazon-Verkaufskonto in der Region [Nordamerika (USA, CA, MX)](https://sell.amazon.com/){target="_blank"} oder [europäisch (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"} haben, können Sie den Einrichtungsprozess für das Kundenkonto von Amazon abschließen.

Für den Amazon-Verkaufskanal ist ein [!DNL Professional Seller] -Konto für [!DNL Amazon Seller Central] erforderlich. Amazon berechnet monatliche Abos und Verkaufspreise. Siehe [Amazon: Wählen Sie Ihren Verkaufsplan](https://sell.amazon.com/pricing.html){target="_blank"}.

## 3. Stellen Sie sicher, dass Sie ein zugelassener Amazon-Verkäufer sind.

Zur Integration benötigen Sie ein genehmigtes [!DNL Amazon Seller Central] -Konto. Für Ihr Konto dürfen keine Einschränkungen für Produkte oder Kategorien gelten. Einige Produkte und Kategorien müssen vor der Erstellung von Listen genehmigt werden. Überprüfen Sie die Amazon-Richtlinien für Kategorie- und Produktgenehmigungen, um sicherzustellen, dass Ihre Produkte genehmigt sind. Siehe [Amazon: Kategorien und Produkte, für die eine Genehmigung erforderlich ist](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} (Anmeldung bei der Verkäuferzentrale erforderlich).

Außerdem müssen Sie sicherstellen, dass Sie Folgendes in Ihrem [!DNL Amazon Seller Central] -Konto konfiguriert haben:

- Stellen Sie sicher, dass Ihre Rückkehrrichtlinie genauso gut oder besser ist wie die Amazon-Rückgaberichtlinie. Siehe [Amazon: Rückgaberichtlinie](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}.

- Stellen Sie sicher, dass Ihre Steuereinstellungen konfiguriert sind. Siehe [Amazon: Tax Policies](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} (Anmeldung bei der Verkäuferzentrale erforderlich).

- Stellen Sie sicher, dass Ihre Versandmethoden korrekt konfiguriert sind. Um die Versandmethoden einzurichten, die den Kunden [!DNL Commerce] zur Erfüllung Ihrer Amazon-Bestellungen angeboten werden, aktualisieren Sie die [Amazon: Versandeinstellungen](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} in Ihrem [!DNL Amazon Seller Central] -Konto.

## 4. Stellen Sie sicher, dass Ihre Mehrwertsteuer für Ihre Geschäfte konfiguriert ist.

(Wird hauptsächlich von britischen Verkäufern verwendet.) Amazon empfiehlt, sich für den [Amazon-Mehrwertsteuerberechnungsdienst](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"} anzumelden. Wenn Sie eine andere Methode wählen, sind Sie für die Einhaltung der Mehrwertsteuer verantwortlich.

>[!NOTE]
>
>Es kann 10-14 Tage dauern, bis Amazon Ihr Konto für den MwSt-Berechnungsdienst überprüft und aktiviert.

## 5. Anzahl der automatischen Katalogübereinstimmungen erhöhen

Beim Onboarding verwendet der Amazon-Verkaufskanal Produktattribute, um Ihre vorhandenen Amazon-Auflistungen (falls zutreffend) mit vorhandenen Produkten in Ihrem [!DNL Commerce]-Katalog abzugleichen. Nach dem Onboarding werden diese Produktattribute verwendet, um Ihre [!DNL Commerce] -Katalogelemente in einer Amazon-Liste zu veröffentlichen und Ihre Produktdaten zwischen [!DNL Commerce] und Amazon zu synchronisieren.

Damit die höchste Anzahl von [!DNL Commerce] -Produkten automatisch mit Amazon-Auflistungen übereinstimmt, sollten Sie eine Reihe von Produktattributen für Ihren [!DNL Commerce] -Katalog erstellen. Bevor Sie Ihren Amazon-Verkaufskanalspeicher einrichten, sollten Sie [!DNL Commerce] -Produktattribute hinzufügen, die diesen Amazon-Attributen entsprechen, z. B.: ASIN, EAN, ISBN, UPC oder GCID. Siehe [Erstellen eines Produktattributs in  [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Konfigurieren Sie Ihre Währung und Konversion (nach Bedarf).

Wenn Ihr Amazon-Store eine andere Währung verwendet, als für Ihren [!DNL Commerce]-Store konfiguriert ist, aktivieren Sie die Währung](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) und legen Sie den [Währungsumrechnungskurs](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-update.html) fest.[

## 7. Erstellen Sie bei Bedarf ein Produktbedingungsattribut.

Wenn Ihre Amazon-Listen mehr als eine Produktbedingung enthalten (z. B. _new_, _used_ oder _like new_), erstellen Sie ein [!DNL Commerce] -Attribut und weisen Sie Bedingungswerte zu. Sie müssen dieses Attribut beim Onboarding dem Amazon Condition-Produktattribut zuordnen. Siehe [Erstellen von Attributen für Amazon](./ob-creating-magento-attributes.md).

## 8. Konfigurieren Sie Ihre [!DNL Amazon Seller Central] Versandmethode

Informationen zum Einrichten von Versandmethoden, die Sie für die Erfüllung Ihrer Amazon-Bestellungen anbieten möchten, finden Sie unter _Einstellungen und Versandeinstellungen_ in Ihrem [!DNL Amazon Seller Central] -Konto.

## Zusätzliche Konfigurationen

Wenn Ihr Amazon-Konto eingerichtet und aktiv ist, gibt es mehrere [!DNL Commerce] Empfehlungen, die den Onboarding-Prozess für den Amazon-Verkaufskanal optimieren.

### Überprüfen und notieren Sie alle Produkte, die Sie ausschließen möchten

Möglicherweise möchten Sie nicht, dass einige Produkte in Amazon aufgeführt werden. Der Amazon-Vertriebskanal verfügt über eine Regel-Engine, mit der bestimmt wird, welche Produkte in Amazon veröffentlicht werden dürfen. Mit den [Listening-Regeln](./listing-rules.md) können Sie Teilmengen von Produkten auswählen, die in Ihrem [!DNL Amazon Seller Central] -Konto veröffentlicht (oder nicht veröffentlicht) werden sollen, z. B. nach Kategorieauswahl oder durch Definition eines oder mehrerer Produktattribute. Wie bei den Preisregeln [!DNL Commerce] [catalog](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) oder [Warenkorb](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) müssen für die Berechtigung zur Amazon-Auflistung verwendete Produktattribute den Wert **[!UICONTROL Use for Promo Rule Conditions]** auf `Yes` setzen. Siehe **[!UICONTROL Use for Promo Rule Conditions]** in [Produktattributen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

### Setzen Sie Ihren [!DNL Amazon Seller Central] -Bereich auf &quot;Inaktiv&quot;

Um den fehlerfreien Datenübergang während der Integration zu erleichtern, wird empfohlen, den Amazon-Bereich unter Einstellungen > Kontoinformationen > Urlaubseinstellungen auf `Inactive` zu setzen. Wenn das Setup abgeschlossen ist, ändern Sie den Status in Amazon wieder auf &quot;`Active`&quot;.

![Nächstes Symbol](assets/btn-next.png) [**Fahren Sie mit dem Erstellen von [!DNL Commerce] Attributen**](./ob-creating-magento-attributes.md) fort.
