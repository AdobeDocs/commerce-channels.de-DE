---
title: Best Practices und Einschränkungen für den Amazon-Vertriebskanal
description: Lesen Sie sich die Best Practices und Einschränkungen bei der Verwendung des Amazon-Vertriebskanals für Adobe Commerce und Magento Open Source durch.
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Best Practices und Einschränkungen für den Amazon-Vertriebskanal

Zu den Best Practices gehören:

- Der Amazon-Vertriebskanal kann sich auf Ihre Amazon-Auflistungen auswirken, indem er die Preise erhöht oder senkt, Produktinformationen (einschließlich verfügbarem Lager) synchronisiert sowie Auflistungen hinzufügt, aktualisiert und beendet (löscht). Überprüfen Sie Ihre Auflistungen nach Status während des Setups und passen Sie Ihre Einstellungen an ([Auflistungseinstellungen](./listing-settings.md), [Auflistungsregeln](./listing-rules.md), [Preisregeln](./pricing-products.md), [Überschreibungen](./overrides.md) usw.), bevor Sie die Einrichtung des Stores abschließen. Diese Einstellungen können nach Bedarf auch nach der Einrichtung geändert werden.

- Der Amazon-Vertriebskanal kann Ihre Preisregeln festlegen, um Ihren Listenpreis automatisch anzupassen. Zu den Sicherheitsvorkehrungen für automatisierte Preise gehören die [Grundstückspreise](./floor-price.md) und die [optionale Deckungssumme](./optional-ceiling-price.md) Funktionen von [Intelligente Neupreisregeln](./intelligent-repricing-rules.md). Durch die Verwendung dieser Schutzklauseln können Sie sicherstellen, dass Ihre Börsennotierungspreise nicht unter Ihren Kosten oder über einen festgelegten Preis liegen.

- Die Datensynchronisation zwischen dem Amazon-Vertriebskanal und Amazon wird durch Ihre Einstellungen [[!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;} gesteuert. Die integrierte Drosselung zwischen [!DNL Commerce] und Amazon trägt zur reibungslosen und effizienten Datenübertragung bei. Bei hohen eCommerce-Traffic-Zeiten (wie Black Friday) kann die Aktualisierung der Amazon-Systeme jedoch länger als üblich dauern. Setzen Sie den Cron [!DNL Commerce] so, dass er alle fünf Minuten ausgeführt wird.

- Der Amazon-Vertriebskanal importiert Ihre Amazon-Bestellinformationen. Um Ihre Amazon-Bestellungen im Amazon-Vertriebskanal zu verwalten, müssen Sie sicherstellen, dass Ihre [Bestelleinstellungen](./order-settings.md) für den Import definiert sind und für jede Amazon-Bestellung eine entsprechende [!DNL Commerce]-Bestellung erstellt wird. Wenn sie nicht definiert ist, können Sie nur Ihre Amazon-Bestellinformationen anzeigen. Sämtliche Umsatzsteuern über Amazon werden weiterhin über Ihr [!DNL Amazon Seller Central] -Konto verwaltet und übertragen. In einigen Staaten ist Amazon verpflichtet, Steuern automatisch zu erheben und zu begrenzen. Für andere Staaten haben die Verkäufer die Möglichkeit, Steuern manuell oder automatisch zu berechnen. Siehe [Amazon: Steuerrichtlinien](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target=&quot;_blank&quot;}. Möglicherweise müssen Sie sich bei Ihrem [!DNL Amazon Seller Central]-Konto anmelden, um die Dokumentation zu den Steuerrichtlinien von Amazon anzuzeigen.

- Für Regionen im Vereinigten Königreich empfiehlt es sich, sich im [Amazon VAT Calculation Service](https://sell.amazon.co.uk/learn/vat-resources/){target=&quot;_blank&quot;} vor dem Onboarding des Amazon-Vertriebskanals anzumelden.


   >[!NOTE]
   >
   >Es kann 10-14 Tage dauern, bis Amazon Ihr Konto für den MwSt-Berechnungsdienst überprüft und aktiviert.

Zu den Einschränkungen gehören:

- Bundle, Geschenkkarten und gruppierte Produktarten, die Teil Ihres [!DNL Commerce]-Katalogs sind, werden vom Amazon-Vertriebskanal für die Auflistung in Amazon nicht unterstützt.

- Der Amazon-Vertriebskanal kann keine Liste für ein Produkt erstellen, das keine vorhandene oder vorherige Amazon-Liste hat. Wenn in [!DNL Amazon Seller Central] kein Produkt mit ASIN vorhanden ist, muss es in [!DNL Amazon Seller Central] hinzugefügt werden, damit Amazon dem Produkt ein ASIN zuweisen kann. Nachdem ein Produkt in Amazon hinzugefügt und eine Liste erstellt wurde, kann die Liste mit Ihrem Katalog im Amazon-Vertriebskanal abgeglichen und synchronisiert werden.
