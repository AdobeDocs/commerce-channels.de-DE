---
title: Amazon-Vertriebskanal - Preisbereich
description: Verwenden Sie den Commerce-Preisbereich, um die Preise nach mehreren Websites oder global zu verwalten.
feature: Sales Channels, Price Rules
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Preissegment

[!DNL Commerce] stellt die Konfiguration bereit, damit Ihr [Preisbereich](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price) auf `Global` oder `Website` eingestellt wird. Wenn der Preis auf &quot;`Global`&quot;festgelegt ist, gibt es eine einzige Preisquelle für alle Websites. Wenn der Preis auf &quot;`Website`&quot;festgelegt ist, können Ihre Websites ihre Preise variieren und außerdem einen Fallback-Standardwert für die Preisgestaltung aufweisen (siehe [Preisbereich](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html)).

Wenn Sie den Umfang Ihres Katalogpreises von `Global` in `Website` ändern, ändern sich alle Preistypattribute ebenfalls in `Website`. Siehe [Hinzufügen von Websites](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites).

Wenn ein Website-Preis ausgewählt wird, gibt es zwei Preisquellen:

- Der Website-Preis
- Der Standardpreis (fallback)

Für die Amazon-Integration mit Vertriebskanälen können Sie basierend auf Ihren [Listening-Regeln](./listing-rules.md) Produkte von mehreren Websites einem einzigen [!DNL Amazon Marketplace] Land zuordnen (definiert während der [Store-Integration](./store-integration.md)). Mit dieser Zuordnung wird jedoch die Frage aufgeworfen, welcher Preis veröffentlicht werden sollte, wenn das Produkt auf mehreren Websites mit unterschiedlichen Preisen vorhanden ist.
