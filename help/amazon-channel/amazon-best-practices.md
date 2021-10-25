---
title: Best Practices und Einschränkungen für Amazon Sales Kanal
description: Überprüfen Sie die Best Practices und Einschränkungen bei der Verwendung des Amazon Sales Kanals für Adobe Commerce und Magento Open Source.
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Best Practices und Beschränkungen für Amazon Sales Kanal

Zu den bewährten Verfahren gehören:

- Amazon Sales Kanal kann Ihre Amazon-Auflistungen beeinflussen, indem er die Preise erhöht oder senkt, Produktinformationen (einschließlich verfügbarer Bestände) synchronisiert und Listen hinzufügt, aktualisiert und beendet (löscht). Überprüfen Sie Ihre Einträge während der Einrichtung anhand des Status und passen Sie Ihre Einstellungen an ([Listeneinstellungen](./listing-settings.md), [Listungsregeln](./listing-rules.md), [Preisregeln](./pricing-products.md), [Überschreibungen](./overrides.md)usw.) vor Abschluss der Store-Einrichtung. Diese Einstellungen können auch nach der Installation nach Bedarf geändert werden.

- Amazon Sales Kanal kann Ihre Preisregeln so festlegen, dass Sie Ihren Listenpreis automatisch anpassen können. Zu den automatischen Preisgarantien gehören [Tiefstpreis](./floor-price.md) und [fakultativer Höchstpreis](./optional-ceiling-price.md) Funktionen von [Intelligente Preisanpassungsregeln](./intelligent-repricing-rules.md). Die Verwendung dieser Sicherheitsmaßnahmen trägt dazu bei, dass Ihre Börsennotierungspreise nicht unter Ihren Kosten oder über einen bestimmten Preis liegen.

- Die Datensynchronisierung zwischen Amazon Sales Kanal und Amazon wird von Ihrem [[!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html)Einstellungen für {Zielgruppe=&quot;_blank&quot;}. Integrierte Drosselung zwischen [!DNL Commerce] und Amazon trägt dazu bei, eine reibungslose und effiziente Datenübertragung zu gewährleisten, aber während hoher eCommerce-Traffic-Zeiten (z. B. Black Freitag) könnte die Aktualisierung der Amazon-Systeme länger als sonst dauern. Legen Sie Ihre [!DNL Commerce] Cron, der einmal alle fünf Minuten ausgeführt wird.

- Amazon Sales Kanal importiert Ihre Amazon Bestellinformationen. Um Ihre Amazon-Bestellungen im Amazon Sales Kanal zu verwalten, müssen Sie sicherstellen, dass [Auftragseinstellungen](./order-settings.md) für den Import und die Erstellung entsprechender [!DNL Commerce] für jede Amazon Bestellung. Wenn sie nicht definiert ist, können Sie nur Ihre Amazon-Bestellinformationen Ansicht haben. Alle Steuern für Verkäufe über Amazon werden weiterhin über Ihre [!DNL Amazon Seller Central] Konto. In einigen Staaten ist Amazon verpflichtet, Steuern automatisch zu erheben und zu erlassen. Für andere Staaten haben die Verkäufer die Möglichkeit, Steuern manuell oder automatisch zu berechnen. Siehe [Amazon: Steuerpolitik](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){Zielgruppe=&quot;_blank&quot;}. Möglicherweise müssen Sie sich bei Ihrem [!DNL Amazon Seller Central] -Konto in die Steuerdokumentation der Ansicht Amazon.

- Für Regionen des Vereinigten Königreichs ist es empfehlenswert, sich bei der [MwSt-Berechnungsservice Amazon](https://sell.amazon.co.uk/learn/vat-resources/){Zielgruppe=&quot;_blank&quot;} vor dem Einstieg in den Amazon-Kanal.


   >[!NOTE]
   >
   >Es kann 10-14 Tage dauern, bis Amazon Ihr MwSt.-Berechnungsservice-Konto überprüft und aktiviert.

Zu den Beschränkungen gehören:

- Bundle, Geschenkkarten und gruppierte Produkttypen, die Teil Ihrer [!DNL Commerce] Der Katalog wird vom Amazon Sales Kanal für die Auflistung in Amazon nicht unterstützt.

- Amazon Sales Kanal kann keine Liste für ein Produkt erstellen, das keine bestehende oder frühere Amazon-Liste enthält. Wenn ein Produkt nicht vorhanden ist in [!DNL Amazon Seller Central] mit einem ASIN, muss es hinzugefügt werden in [!DNL Amazon Seller Central] damit Amazon dem Produkt ein ASIN zuweisen kann. Nachdem ein Produkt in Amazon hinzugefügt und eine Auflistung erstellt wurde, kann die Auflistung mit Ihrem Katalog im Amazon Sales Kanal abgeglichen und synchronisiert werden.
