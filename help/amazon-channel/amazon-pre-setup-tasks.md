---
title: Aufgaben vor der Einrichtung für [!DNL Amazon sales channel]
description: Überprüfen Sie die erforderlichen Aufgaben, bevor Sie Ihren Adobe Commerce- oder Magento Open Source-Store in Amazon Sales Channel integrieren.
role: Admin, Developer
feature: Sales Channels, Install, Configuration
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---

# Aufgaben vor der Einrichtung für [!DNL Amazon sales channel]

Vorher [Store-Integration](./store-integration.md)müssen Sie sicherstellen, dass Ihre [!DNL Amazon Seller Central] -Konto und [!DNL Commerce] -Konto für die Integration bereit sind. Für eine erfolgreiche Integration sind einige Aufgaben vor der Einrichtung erforderlich.

Wenn Sie Ihren ersten Amazon Store im Amazon-Vertriebskanal einrichten, wird eine Liste mit Einrichtungsaufgaben angezeigt. Es wird empfohlen, diese Aufgaben vor der Durchführung zu überprüfen. [Amazon Store hinzufügen](./store-integration.md). Nachdem Sie Ihren ersten Store hinzugefügt haben, können Sie diese Aufgaben in der Ansicht &quot;Lernen und Vorbereitung&quot;des Amazon-Vertriebskanals ansehen. [Startseite](./amazon-sales-channel-home.md).

## 1. Aktivieren Sie Hintergrundaufgaben in [!DNL Commerce]

Alle zwischen synchronisierten Produkte und Daten [!DNL Commerce] und Amazon von einer [Cron-Auftrag](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html). Wenn Sie Aufgaben wie das Hinzufügen oder Aktualisieren von Auflistungen abschließen und Bestellungen erhalten, sendet ein Cron-Auftrag Daten zwischen Ihren [!DNL Commerce] Backend und Ihre [!DNL Amazon Seller Central] -Konto.

- [Aktivieren [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html).

- Für maximale Leistung: [set [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/system.html) alle fünf Minuten ausgeführt werden.

## 2. Erstellen Sie Ihre [!DNL Amazon Seller Central] account

Bevor Sie mit der Einrichtung Ihres Amazon-Vertriebskanals beginnen, müssen Sie über eine aktive [!DNL Amazon Seller Central] -Konto. Wenn Sie kein bestehendes Amazon-Verkaufskonto im [Nordamerika (USA, CA, MX)](https://sell.amazon.com/){target="_blank"} or [European (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"} -Region können Sie die Einrichtung des Amazon-Kundenkontos abschließen.

Für den Amazon-Vertriebskanal ist ein [!DNL Professional Seller] Konto auf [!DNL Amazon Seller Central]. Amazon berechnet monatliche Abos und Verkaufspreise. Siehe [Amazon: Wählen Sie Ihren Verkaufsplan aus.](https://sell.amazon.com/pricing.html){target="_blank"}.

## 3. Stellen Sie sicher, dass Sie ein zugelassener Amazon-Verkäufer sind.

Zur Integration benötigen Sie eine [!DNL Amazon Seller Central] -Konto. Für Ihr Konto dürfen keine Einschränkungen für Produkte oder Kategorien gelten. Einige Produkte und Kategorien müssen vor der Erstellung von Listen genehmigt werden. Überprüfen Sie die Amazon-Richtlinien für Kategorie- und Produktgenehmigungen, um sicherzustellen, dass Ihre Produkte genehmigt sind. Siehe [Amazon: Kategorien und Produkte, für die eine Genehmigung erforderlich ist](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} (Anmeldung bei Seller Central erforderlich).

Es ist auch wichtig sicherzustellen, dass Sie Folgendes in der [!DNL Amazon Seller Central] Konto:

- Stellen Sie sicher, dass Ihre Rückkehrrichtlinie genauso gut oder besser ist wie die Amazon-Rückgaberichtlinie. Siehe [Amazon: Rückgaberichtlinie](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}.

- Stellen Sie sicher, dass Ihre Steuereinstellungen konfiguriert sind. Siehe [Amazon: Steuerpolitik](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} (Anmeldung bei Seller Central erforderlich).

- Stellen Sie sicher, dass Ihre Versandmethoden korrekt konfiguriert sind. So richten Sie Versandmethoden ein, die [!DNL Commerce] Kunden angeboten werden, Ihre Amazon-Bestellungen zu erfüllen, aktualisieren Sie die [Amazon: Versandeinstellungen](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} in [!DNL Amazon Seller Central] -Konto.

## 4. Stellen Sie sicher, dass Ihre Mehrwertsteuer für Ihre Geschäfte konfiguriert ist.

(Wird hauptsächlich von britischen Verkäufern verwendet.) Amazon empfiehlt, sich für die [Amazon - MwSt-Berechnungsservice](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}. Wenn Sie eine andere Methode wählen, sind Sie für die Einhaltung der Mehrwertsteuer verantwortlich.

>[!NOTE]
>
>Es kann 10-14 Tage dauern, bis Amazon Ihr Konto für den MwSt-Berechnungsdienst überprüft und aktiviert.

## 5. Anzahl der automatischen Katalogübereinstimmungen erhöhen

Beim Onboarding verwendet der Amazon-Verkaufskanal Produktattribute, um Ihre vorhandenen Amazon-Listen (falls zutreffend) mit vorhandenen Produkten in Ihrer [!DNL Commerce] Katalog. Nach dem Onboarding werden diese Produktattribute zum Veröffentlichen Ihrer [!DNL Commerce] Katalogelemente mit einer Amazon-Liste zu verknüpfen und Ihre Produktdaten zwischen [!DNL Commerce] und Amazon.

So erhalten Sie die höchste Anzahl von [!DNL Commerce] Produkte automatisch mit Amazon-Listen übereinstimmen, sollten Sie eine Reihe von Produktattributen für Ihre [!DNL Commerce] Katalog. Bevor Sie Ihren Amazon Sales Channel Store einrichten, sollten Sie [!DNL Commerce] Produktattribute, die diesen Amazon-Attributen entsprechen, beispielsweise: ASIN, EAN, ISBN, UPC oder GCID. Siehe [Erstellen Sie ein Produktattribut in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Konfigurieren Sie Ihre Währung und Konversion (nach Bedarf).

Wenn Ihr Amazon-Store eine andere Währung verwendet, als für Ihre [!DNL Commerce] speichern, [die Währung](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) und legen Sie die [Währungskonversionsrate](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-update.html).

## 7. Erstellen Sie bei Bedarf ein Produktbedingungsattribut.

Wenn Ihre Amazon-Listen mehr als eine Produktbedingung enthalten (z. B. _new_, _used_ oder _like new_), erstellen Sie eine [!DNL Commerce] zuweisen und Bedingungswerte zuweisen. Sie müssen dieses Attribut beim Onboarding dem Amazon Condition-Produktattribut zuordnen. Siehe [Erstellen von Attributen für Amazon](./ob-creating-magento-attributes.md).

## 8. Konfigurieren Sie Ihre [!DNL Amazon Seller Central] Versandmethode

Informationen zum Einrichten von Versandmethoden, die Sie zur Erfüllung Ihrer Amazon-Bestellungen anbieten möchten, finden Sie unter _Einstellungen und Versandeinstellungen_ in [!DNL Amazon Seller Central] -Konto.

## Zusätzliche Konfigurationen

Wenn Ihr Amazon-Konto eingerichtet und aktiv ist, gibt es mehrere [!DNL Commerce] Empfehlungen zur Optimierung des Einstiegsprozesses in den Amazon-Verkaufskanal.

### Überprüfen und notieren Sie alle Produkte, die Sie ausschließen möchten

Möglicherweise möchten Sie nicht, dass einige Produkte in Amazon aufgeführt werden. Der Amazon-Vertriebskanal verfügt über eine Regel-Engine, mit der bestimmt wird, welche Produkte in Amazon veröffentlicht werden dürfen. [Listening-Regeln](./listing-rules.md) Sie können Teilmengen von Produkten auswählen, die in Ihrer [!DNL Amazon Seller Central] -Konto, z. B. durch Kategorieauswahl oder Definition eines oder mehrerer Produktattribute. liken [!DNL Commerce] [Katalog](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) oder [Warenkorb](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) Preisregeln, Produktattribute, die für die Berechtigung zur Amazon-Auflistung verwendet werden, müssen **[!UICONTROL Use for Promo Rule Conditions]** auf `Yes`. Siehe **[!UICONTROL Use for Promo Rule Conditions]** in [Produktattribute](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

### Legen Sie Ihre [!DNL Amazon Seller Central] region to inactive

Um den fehlerfreien Datenübergang während der Integration zu erleichtern, wird empfohlen, für Ihre Amazon-Region den Wert `Inactive` Status unter Einstellungen > Kontoinformationen > Urlaubseinstellungen. Wenn Ihre Einrichtung abgeschlossen ist, ändern Sie den Status zurück zu `Active` in Amazon.

![Nächstes Symbol](assets/btn-next.png) [**Fahren Sie mit Erstellen fort [!DNL Commerce] Attribute**](./ob-creating-magento-attributes.md)
