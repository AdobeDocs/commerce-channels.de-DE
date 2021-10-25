---
title: Aufgaben vor dem Setup
description: Überprüfen Sie die erforderlichen Aufgaben, bevor Sie Ihren Adobe Commerce- oder Magento Open Source-Store in Amazon Sales Channel integrieren.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Aufgaben vor dem Setup

Vor [Integration speichern](./store-integration.md), müssen Sie sicherstellen, dass [!DNL Amazon Seller Central] und Ihrem Konto [!DNL Commerce] Konto ist für die Integration bereit. Für eine erfolgreiche Integration gibt es einige erforderliche Aufgaben vor dem Setup.

Wenn Sie Ihren ersten Amazon Store in Amazon Sales Kanal einrichten, wird eine Liste von Setup-Aufgaben angezeigt. Es wird empfohlen, diese Aufgaben vor Ihnen zu lesen [Amazon Store hinzufügen](./store-integration.md). Nach dem Hinzufügen Ihres ersten Ladens können Sie diese Aufgaben in der Ansicht Lernen und Vorbereitung des Amazon Kanals lesen. [Startseite](./amazon-sales-channel-home.md).

## 1. Hintergrundinformationen aktivieren in [!DNL Commerce]

Alle Produkte und Daten synchronisiert zwischen [!DNL Commerce] und Amazon wird von einem [cron job](https://docs.magento.com/user-guide/system/cron.html){Zielgruppe=&quot;_blank&quot;}. Wenn Sie Aufgaben wie das Hinzufügen oder Aktualisieren von Auflistungen abgeschlossen haben und Bestellungen erhalten, sendet ein Cron-Auftrag Daten zwischen Ihren [!DNL Commerce] Backend und Ihre [!DNL Amazon Seller Central] Konto.

- [Aktivieren [!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){Zielgruppe=&quot;_blank&quot;}.

- Für maximale Leistung [set [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){Zielgruppe=&quot;_blank&quot;} zum einmaligen Ausführen alle fünf Minuten.

## 2. Erstellen Sie [!DNL Amazon Seller Central] Konto

Bevor Sie mit der Einrichtung Ihres Amazon Sales Kanals beginnen, müssen Sie einen aktiven [!DNL Amazon Seller Central] Konto. Wenn Sie kein bestehendes Amazon Seller-Konto im [Nordamerika (USA, CA, MX)](https://sell.amazon.com/){Zielgruppe=&quot;_blank&quot;} oder [europäisch (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){Zielgruppe=&quot;_blank&quot;} Region, können Sie den Vorgang zur Einrichtung des Amazon-Händlerkontos abschließen.

Amazon Sales Kanal erfordert [!DNL Professional Seller] Konto auf [!DNL Amazon Seller Central]. Amazon berechnet monatlich ein Abonnement und Verkaufsgebühren. Siehe [Amazon: Wählen Sie Ihren Verkaufsplan aus](https://sell.amazon.com/pricing.html){Zielgruppe=&quot;_blank&quot;}.

## 3. Vergewissern Sie sich, dass Sie ein zugelassener Amazon-Verkäufer sind

Für die Integration benötigen Sie eine Genehmigung von [!DNL Amazon Seller Central] Konto. Ihr Konto darf keine Beschränkungen für Produkte oder Kategorien enthalten. Einige Produkte und Kategorien müssen vor dem Erstellen von Auflistungen genehmigt werden. Überprüfen Sie die Amazon-Richtlinien für Kategorie und Produktgenehmigung, um sicherzustellen, dass Ihre Produkte genehmigt werden. Siehe [Amazon: Genehmigungspflichtige Kategorien und Erzeugnisse](https://sellercentral.amazon.com/gp/help/200333160){Zielgruppe=&quot;_blank&quot;} (Anmeldung bei Verkäuferzentrale erforderlich).

Es ist außerdem wichtig sicherzustellen, dass Sie Folgendes konfiguriert haben: [!DNL Amazon Seller Central] Konto:

- Vergewissern Sie sich, dass Ihre Rückgaberichtlinie so gut wie oder besser ist als die Rückgaberichtlinie der Amazon. Siehe [Amazon: Rückgaberichtlinie](https://www.amazon.com/gp/help/customer/display.html){Zielgruppe=&quot;_blank&quot;}.

- Stellen Sie sicher, dass Ihre Steuereinstellungen konfiguriert sind. Siehe [Amazon: Steuerpolitik](https://sellercentral.amazon.com/gp/help/external/help.html){Zielgruppe=&quot;_blank&quot;} (Anmeldung bei Verkäuferzentrale erforderlich).

- Stellen Sie sicher, dass Ihre Versandmethoden korrekt konfiguriert sind. So legen Sie die Versandmethoden fest, die [!DNL Commerce] den Kunden angeboten werden, Ihre Amazon-Bestellungen zu erfüllen, aktualisieren Sie die [Amazon: Versandeinstellungen](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){Zielgruppe=&quot;_blank&quot;} in Ihrer [!DNL Amazon Seller Central] Konto.

## 4. Vergewissern Sie sich, dass Ihre Mehrwertsteuer für Ihre Geschäfte konfiguriert ist.

(hauptsächlich von britischen Verkäufern verwendet) Amazon empfiehlt, sich für die [MwSt-Berechnungsservice Amazon](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){Zielgruppe=&quot;_blank&quot;}. Wenn Sie eine andere Methode wählen, sind Sie für die Einhaltung der Mehrwertsteuer verantwortlich.

>[!NOTE]
>
>Es kann 10-14 Tage dauern, bis Amazon Ihr MwSt.-Berechnungsservice-Konto überprüft und aktiviert.

## 5. Anzahl der automatischen Katalogpassungen erhöhen

Amazon Sales Kanal verwendet beim Einstieg Produktattribute, um Ihre bestehenden Amazon-Listen (falls zutreffend) mit den vorhandenen Produkten in Ihren [!DNL Commerce] Katalog. Nach dem Einstieg werden diese Produktattribute verwendet, um Ihre [!DNL Commerce] Katalogelemente in einer Amazon-Liste zu speichern und Ihre Produktdaten zu synchronisieren zwischen [!DNL Commerce] und Amazon.

Um die höchste Anzahl von [!DNL Commerce] Produkte, die automatisch mit Amazon-Auflistungen übereinstimmen, sollten Sie eine Reihe von Produktattributen für Ihre [!DNL Commerce] Katalog. Bevor Sie Ihren Amazon Sales Kanal Store einrichten, sollten Sie [!DNL Commerce] Produktattribute, die diesen Amazon-Attributen entsprechen, z. B.: ASIN, EAN, ISBN, UPC oder GCID. Siehe [Produkt-Attribut erstellen in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Währung und Konversion konfigurieren (falls erforderlich)

Wenn Ihr Amazon Store eine andere Währung verwendet, als für Ihre [!DNL Commerce] speichern, [die Währung aktivieren](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){Zielgruppe=&quot;_blank&quot;} und legen Sie die [Währung Konversionsrat](https://docs.magento.com/user-guide/stores/currency-update.html){Zielgruppe=&quot;_blank&quot;}.

## 7. Produkt-Bedingungsattribut erstellen (nach Bedarf)

Wenn Ihre Amazon-Auflistungen mehr als eine Produktbedingung enthalten (z. B. _neu_, _verwendet_ oder _wie neu_), erstellen Sie eine [!DNL Commerce] Attribut und Zuweisen von Bedingungswerten. Sie müssen dieses Attribut beim Einstieg dem Amazon Condition-Produktattribut zuordnen. Siehe [Erstellen von Attributen für Amazon](./ob-creating-magento-attributes.md).

## 8. Konfigurieren Sie Ihre [!DNL Amazon Seller Central] Versandmethode

Informationen zum Einrichten von Versandmethoden, die Sie zur Erfüllung Ihrer Amazon-Aufträge Angebot haben möchten, finden Sie unter [Einstellungen für Versandverfahren][10] in [!DNL Amazon Seller Central] Konto.

## Zusätzliche Konfigurationen

Wenn Ihr Amazon-Konto eingerichtet und aktiv ist, gibt es mehrere [!DNL Commerce] Empfehlungen zur Optimierung des Amazon Sales Kanal-Onboarding-Prozesses.

### Alle Produkte, die Sie ausschließen möchten, prüfen und notieren

Möglicherweise möchten Sie nicht, dass einige Produkte auf Amazon aufgelistet werden. Amazon Sales Kanal verfügt über eine Listing Rule Engine, die verwendet wird, um zu bestimmen, welche Produkte für die Veröffentlichung in Amazon infrage kommen. [Listungsregeln](./listing-rules.md) Sie können Teilmengen von Produkten auswählen, die in Ihren [!DNL Amazon Seller Central] , z. B. durch Auswahl der Kategorie oder durch Definition eines oder mehrerer Produktattribute. Gefällt mir [!DNL Commerce] [Katalog](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){Zielgruppe=&quot;_blank&quot;} oder [Warenkorb](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){Zielgruppe=&quot;_blank&quot;} Preisregeln, Produktattribute, die für die Amazon-Notierungsfähigkeit verwendet werden, müssen über **[!UICONTROL Use for Promo Rule Conditions]** einstellen auf `Yes`. Siehe **[!UICONTROL Use for Promo Rule Conditions]** in [Produktattribute](https://docs.magento.com/user-guide/stores/attributes-product.html){Zielgruppe=&quot;_blank&quot;}.

### Legen Sie Ihre [!DNL Amazon Seller Central] Region zu inaktiv

Um die fehlerfreie Transition von Daten während der Integration zu erleichtern, sollten Sie Ihren Amazon-Bereich auf `Inactive` Status unter Einstellungen > Kontoinformationen > Urlaubseinstellungen. Siehe [Amazon: Listungsstatus für Urlaube][11]. Wenn die Einrichtung abgeschlossen ist, ändern Sie den Status in `Active` in Amazon.

![Nächstes Symbol](assets/btn-next.png) [**Erstellen fortsetzen [!DNL Commerce] Attribute**](./ob-creating-magento-attributes.md)
