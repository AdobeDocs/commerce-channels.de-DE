---
title: Preisumfang
description: Verwenden Sie den Umfang der Commerce-Preise, um die Preise nach mehreren Websites oder global zu verwalten.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Preisumfang

[!DNL Commerce] bietet Konfiguration für Ihre [Preisgestaltung](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} to be set to `Global` or `Website`. If pricing is set to `Global`, there is a single price source for all websites. If pricing is set to `Website`, your websites can vary their pricing across and also have a fallback default pricing value. See [Catalog Price](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} im Commerce-Benutzerhandbuch.

Wenn Sie den Umfang Ihres Katalogpreises von `Global` nach `Website`, ändern sich alle Preistypattribute ebenfalls in `Website`. Siehe [Hinzufügen von Websites](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target="_blank"}.

Wenn ein Website-Preis ausgewählt wird, gibt es zwei Preisquellen:

- Der Website-Preis
- Der Standardpreis (fallback)

Für die Amazon-Vertriebskanalintegration basierend auf Ihrer [Auflistungsregeln](./listing-rules.md)können Sie Produkte von mehreren Websites zu einer einzigen zuordnen [!DNL Amazon Marketplace] Land (definiert während [Store-Integration](./store-integration.md)). Mit dieser Zuordnung wird jedoch die Frage aufgeworfen, welcher Preis veröffentlicht werden sollte, wenn das Produkt auf mehreren Websites mit unterschiedlichen Preisen vorhanden ist.
