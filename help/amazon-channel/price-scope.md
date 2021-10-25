---
title: Preisumfang
description: Verwenden Sie den Commerce-Preisbereich, um die Preise nach mehreren Websites oder global zu verwalten.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Preisbereich

[!DNL Commerce] bietet Konfiguration für [Preisgestaltung](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price)Einstellung von {Zielgruppe=&quot;_blank&quot;} auf `Global` oder `Website`. Wenn die Preisgestaltung auf `Global`, gibt es eine einzige Preisquelle für alle Websites. Wenn die Preisgestaltung auf `Website`, können Ihre Websites ihre Preise variieren und haben auch einen Fallback-Standard-Preiswert. Siehe [Katalogpreis](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){Zielgruppe=&quot;_blank&quot;} im zentralen Commerce-Benutzerhandbuch.

Wenn Sie Ihren Katalogpreisbereich ändern von `Global` nach `Website`, ändern sich alle Preistypattribute ebenfalls in `Website`. Siehe [Websites hinzufügen](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){Zielgruppe=&quot;_blank&quot;}.

Bei der Auswahl eines Website-Preises gibt es zwei Preisquellen:

- Der Preis der Website
- Der Preis für den Ausfall (Fall-back)

Für die Amazon Sales Kanal-Integration, basierend auf Ihren [Listungsregeln](./listing-rules.md)können Sie Produkte aus mehreren Websites zu einem einzigen zuordnen [!DNL Amazon Marketplace] Land (definiert während [Speicherintegration](./store-integration.md)). Diese Kartierung führt jedoch die Frage auf, welcher Preis veröffentlicht werden soll, wenn das Produkt auf mehreren Websites mit unterschiedlichen Preisen vorhanden ist.
