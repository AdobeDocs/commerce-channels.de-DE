---
title: Preisumfang
description: Verwenden Sie den Umfang der Commerce-Preise, um die Preise nach mehreren Websites oder global zu verwalten.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Preissegment

[!DNL Commerce] stellt eine Konfiguration bereit, damit Ihr  [Preisbereich](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target=&quot;_blank&quot;} auf  `Global` oder  `Website`gesetzt wird. Wenn der Preis auf `Global` festgelegt ist, gibt es eine einzige Preisquelle für alle Websites. Wenn die Preisgestaltung auf `Website` festgelegt ist, können Ihre Websites ihre Preise variieren und außerdem einen Fallback-Standardwert für die Preisgestaltung aufweisen. Siehe [Catalog Price](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target=&quot;_blank&quot;} im Benutzerhandbuch zu Commerce-Kerndiensten.

Wenn Sie den Umfang Ihres Katalogpreises von `Global` in `Website` ändern, ändern sich auch alle Preisattribute in `Website`. Siehe [Websites hinzufügen](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){:target=&quot;_blank&quot;}.

Wenn ein Website-Preis ausgewählt wird, gibt es zwei Preisquellen:

- Der Website-Preis
- Der Standardpreis (fallback)

Für die Amazon-Integration mit Vertriebskanälen, die auf Ihren [Listening-Regeln](./listing-rules.md) basiert, können Sie Produkte von mehreren Websites einem einzigen [!DNL Amazon Marketplace] -Land zuordnen (definiert während [Store-Integration](./store-integration.md)). Mit dieser Zuordnung wird jedoch die Frage aufgeworfen, welcher Preis veröffentlicht werden sollte, wenn das Produkt auf mehreren Websites mit unterschiedlichen Preisen vorhanden ist.
