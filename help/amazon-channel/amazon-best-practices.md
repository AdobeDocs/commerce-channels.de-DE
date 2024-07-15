---
title: Best Practices und Einschränkungen für [!DNL Amazon sales channel]
description: Lesen Sie die Best Practices und Einschränkungen bei der Verwendung des Amazon-Vertriebskanals für Adobe Commerce und Magento Open Source.
role: Leader, Admin, User
feature: Sales Channels, Best Practices
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Best Practices und Einschränkungen für [!DNL Amazon sales channel]

Zu den Best Practices gehören:

- Der Amazon-Vertriebskanal kann sich auf Ihre Amazon-Auflistungen auswirken, indem er die Preise erhöht oder senkt, Produktinformationen (einschließlich verfügbarem Lager) synchronisiert sowie Auflistungen hinzufügt, aktualisiert und beendet (löscht). Überprüfen Sie Ihre Auflistungen nach Status während des Setups und passen Sie Ihre Einstellungen an ([Auflistungseinstellungen](./listing-settings.md), [Auflistungsregeln](./listing-rules.md), [Preisregeln](./pricing-products.md), [Überschreibung](./overrides.md) usw.), bevor Sie das Store-Setup abschließen. Diese Einstellungen können nach Bedarf auch nach der Einrichtung geändert werden.

- Der Amazon-Vertriebskanal kann Ihre Preisregeln festlegen, um Ihren Listenpreis automatisch anzupassen. Zu den Sicherheitsmaßnahmen für die automatische Preisgestaltung gehören die Funktionen [Grundpreis](./floor-price.md) und [optionaler Höchstpreis](./optional-ceiling-price.md) der [Intelligenten Neupreisregeln](./intelligent-repricing-rules.md). Durch die Verwendung dieser Schutzklauseln können Sie sicherstellen, dass Ihre Börsennotierungspreise nicht unter Ihren Kosten oder über einen festgelegten Preis liegen.

- Die Datensynchronisation zwischen dem Amazon-Verkaufskanal und Amazon wird durch Ihre [[!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) -Einstellungen gesteuert. Die integrierte Drosselung zwischen [!DNL Commerce] und Amazon trägt dazu bei, eine reibungslose und effiziente Datenübertragung sicherzustellen. Bei hohen eCommerce-Traffic-Zeiten (z. B. Black Friday) kann die Aktualisierung der Amazon-Systeme jedoch länger als üblich dauern. Setzen Sie Ihren [!DNL Commerce] Cron so, dass er einmal alle fünf Minuten ausgeführt wird.

- Der Amazon-Vertriebskanal importiert Ihre Amazon-Bestellinformationen. Um Ihre Amazon-Bestellungen im Amazon-Vertriebskanal zu verwalten, müssen Sie sicherstellen, dass Ihre [Bestelleinstellungen](./order-settings.md) für den Import definiert sind und für jede Amazon-Bestellung eine entsprechende [!DNL Commerce]-Bestellung erstellt wird. Wenn sie nicht definiert ist, können Sie nur Ihre Amazon-Bestellinformationen anzeigen. Alle Umsatzsteuern über Amazon werden weiterhin über Ihr [!DNL Amazon Seller Central] -Konto verwaltet und übertragen. In einigen Staaten ist Amazon verpflichtet, Steuern automatisch zu erheben und zu begrenzen. Für andere Staaten haben die Verkäufer die Möglichkeit, Steuern manuell oder automatisch zu berechnen. Siehe [Amazon: Steuerrichtlinien](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target="_blank"}. Möglicherweise müssen Sie sich bei Ihrem [!DNL Amazon Seller Central] -Konto anmelden, um die Dokumentation zu den Steuerrichtlinien von Amazon anzuzeigen.

- Für Regionen des Vereinigten Königreichs empfiehlt es sich, sich vor dem Onboarding des Amazon-Vertriebskanals beim [Amazon-Mehrwertsteuerberechnungsdienst](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"} anzumelden.

  >[!NOTE]
  >
  >Es kann 10-14 Tage dauern, bis Amazon Ihr Konto für den MwSt-Berechnungsdienst überprüft und aktiviert.

Zu den Einschränkungen gehören:

- Bundle, Geschenkkarten und gruppierte Produktarten, die Teil Ihres [!DNL Commerce]-Katalogs sind, werden vom Amazon-Vertriebskanal für die Auflistung in Amazon nicht unterstützt.

- Der Amazon-Vertriebskanal kann keine Liste für ein Produkt erstellen, das keine vorhandene oder vorherige Amazon-Liste hat. Wenn ein Produkt nicht in [!DNL Amazon Seller Central] mit einem ASIN vorhanden ist, muss es in [!DNL Amazon Seller Central] hinzugefügt werden, damit Amazon dem Produkt ein ASIN zuweisen kann. Nachdem ein Produkt in Amazon hinzugefügt und eine Liste erstellt wurde, kann die Liste mit Ihrem Katalog im Amazon-Vertriebskanal abgeglichen und synchronisiert werden.
