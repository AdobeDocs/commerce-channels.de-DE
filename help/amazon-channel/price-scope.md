---
title: Preisumfang
description: Verwenden Sie den Umfang der Commerce-Preise, um die Preise nach mehreren Websites oder global zu verwalten.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Preissegment

[!DNL Commerce] bietet Konfiguration für Ihre [Preisgestaltung](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target=&quot;_blank&quot;} festzulegen auf `Global` oder `Website`. Wenn der Preis auf `Global`, gibt es eine einzige Preisquelle für alle Websites. Wenn der Preis auf `Website`können Ihre Websites ihre Preise variieren und außerdem einen Fallback-Standardwert für die Preisgestaltung aufweisen. Siehe [Katalogpreis](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target=&quot;_blank&quot;} im Benutzerhandbuch zu Commerce-Kernthemen.

Wenn Sie den Umfang Ihres Katalogpreises von `Global` nach `Website`, ändern sich alle Preistypattribute ebenfalls in `Website`. Siehe [Hinzufügen von Websites](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target=&quot;_blank&quot;}.

Wenn ein Website-Preis ausgewählt wird, gibt es zwei Preisquellen:

- Der Website-Preis
- Der Standardpreis (fallback)

Für die Amazon-Vertriebskanalintegration basierend auf Ihrer [Auflistungsregeln](./listing-rules.md)können Sie Produkte von mehreren Websites zu einer einzigen zuordnen [!DNL Amazon Marketplace] Land (definiert während [Store-Integration](./store-integration.md)). Mit dieser Zuordnung wird jedoch die Frage aufgeworfen, welcher Preis veröffentlicht werden sollte, wenn das Produkt auf mehreren Websites mit unterschiedlichen Preisen vorhanden ist.
