---
title: Best Practices und Einschränkungen für [!DNL Amazon sales channel]
description: Lesen Sie die Best Practices und Einschränkungen bei der Verwendung des Amazon-Vertriebskanals für Adobe Commerce und Magento Open Source.
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Best Practices und Einschränkungen für [!DNL Amazon sales channel]

Zu den Best Practices gehören:

- Der Amazon-Vertriebskanal kann sich auf Ihre Amazon-Auflistungen auswirken, indem er die Preise erhöht oder senkt, Produktinformationen (einschließlich verfügbarem Lager) synchronisiert sowie Auflistungen hinzufügt, aktualisiert und beendet (löscht). Überprüfen Sie Ihre Auflistungen nach Status während der Einrichtung und passen Sie Ihre Einstellungen an ([Auflistungseinstellungen](./listing-settings.md), [Auflistungsregeln](./listing-rules.md), [Preisregeln](./pricing-products.md), [Außerkraftsetzungen](./overrides.md)usw.), bevor Sie Ihre Store-Einrichtung abschließen. Diese Einstellungen können nach Bedarf auch nach der Einrichtung geändert werden.

- Der Amazon-Vertriebskanal kann Ihre Preisregeln festlegen, um Ihren Listenpreis automatisch anzupassen. Zu den Sicherheitsvorkehrungen für automatisierte Preisfeststellungen gehören [Grundpreis](./floor-price.md) und [fakultativer Höchstpreis](./optional-ceiling-price.md) Funktionen von [Intelligente Neupreisregeln](./intelligent-repricing-rules.md). Durch die Verwendung dieser Schutzklauseln können Sie sicherstellen, dass Ihre Börsennotierungspreise nicht unter Ihren Kosten oder über einen festgelegten Preis liegen.

- Die Datensynchronisation zwischen Amazon Sales Channel und Amazon wird von Ihrem [[!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) -Einstellungen. Integrierte Drosselung zwischen [!DNL Commerce] und Amazon helfen bei der Sicherstellung einer reibungslosen und effizienten Datenübertragung. Bei hohen eCommerce-Traffic-Zeiten (z. B. Black Friday) kann die Aktualisierung der Amazon-Systeme jedoch länger als üblich dauern. Legen Sie Ihre [!DNL Commerce] Cron alle fünf Minuten laufen.

- Der Amazon-Vertriebskanal importiert Ihre Amazon-Bestellinformationen. Um Ihre Amazon-Bestellungen im Amazon-Vertriebskanal zu verwalten, müssen Sie sicherstellen, dass Ihre [Bestelleinstellungen](./order-settings.md) werden definiert, um die entsprechenden [!DNL Commerce] für jede Amazon-Bestellung. Wenn sie nicht definiert ist, können Sie nur Ihre Amazon-Bestellinformationen anzeigen. Sämtliche Umsatzsteuern über Amazon werden weiterhin über Ihre [!DNL Amazon Seller Central] -Konto. In einigen Staaten ist Amazon verpflichtet, Steuern automatisch zu erheben und zu begrenzen. Für andere Staaten haben die Verkäufer die Möglichkeit, Steuern manuell oder automatisch zu berechnen. Siehe [Amazon: Steuerpolitik](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target="_blank"}. Möglicherweise müssen Sie sich bei der [!DNL Amazon Seller Central] -Konto, um die Dokumentation zu den Steuerrichtlinien von Amazon anzuzeigen.

- Für Regionen des Vereinigten Königreichs empfiehlt es sich, sich bei der [Amazon - MwSt-Berechnungsservice](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"} vor dem Onboarding des Amazon-Vertriebskanals.


   >[!NOTE]
   >
   >Es kann 10-14 Tage dauern, bis Amazon Ihr Konto für den MwSt-Berechnungsdienst überprüft und aktiviert.

Zu den Einschränkungen gehören:

- Pakete, Geschenkkarten und gruppierte Produktarten, die Teil Ihrer [!DNL Commerce] -Kataloge werden vom Amazon-Vertriebskanal für die Auflistung in Amazon nicht unterstützt.

- Der Amazon-Vertriebskanal kann keine Liste für ein Produkt erstellen, das keine vorhandene oder vorherige Amazon-Liste hat. Wenn ein Produkt nicht in [!DNL Amazon Seller Central] mit einem ASIN, muss es in [!DNL Amazon Seller Central] damit Amazon dem Produkt ein ASIN zuweisen kann. Nachdem ein Produkt in Amazon hinzugefügt und eine Liste erstellt wurde, kann die Liste mit Ihrem Katalog im Amazon-Vertriebskanal abgeglichen und synchronisiert werden.
