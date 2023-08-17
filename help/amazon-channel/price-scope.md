---
title: Amazon-Vertriebskanal - Preisbereich
description: Verwenden Sie den Umfang der Commerce-Preise, um die Preise nach mehreren Websites oder global zu verwalten.
feature: Sales Channels, Price Rules
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Preissegment

[!DNL Commerce] stellt die Konfiguration für Ihre [Preisgestaltung](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price) auf `Global` oder `Website`. Wenn die Preisfestsetzung auf `Global`, gibt es eine einzige Preisquelle für alle Websites. Wenn die Preisfestsetzung auf `Website`, können Ihre Websites ihre Preise variieren und auch einen Fallback-Standardwert für die Preisgestaltung aufweisen (siehe [Preissegment](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html)).

Wenn Sie den Umfang Ihres Katalogpreises von `Global` nach `Website`, ändern sich alle Preistypattribute ebenfalls in `Website`. Siehe [Hinzufügen von Websites](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites).

Wenn ein Website-Preis ausgewählt wird, gibt es zwei Preisquellen:

- Der Website-Preis
- Der Standardpreis (fallback)

Für die Amazon-Vertriebskanalintegration basierend auf Ihrer [Auflistungsregeln](./listing-rules.md)können Sie Produkte von mehreren Websites zu einer einzigen zuordnen [!DNL Amazon Marketplace] Land (definiert während [Store-Integration](./store-integration.md)). Mit dieser Zuordnung wird jedoch die Frage aufgeworfen, welcher Preis veröffentlicht werden sollte, wenn das Produkt auf mehreren Websites mit unterschiedlichen Preisen vorhanden ist.
