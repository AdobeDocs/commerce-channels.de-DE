---
title: Verwalten von Attributen für Amazon-Listen
description: Sie können die Zuordnung von Commerce-Produktattributen zu den Amazon-Attributen verwalten, um genaue Produktinformationen zwischen den Systemen sicherzustellen.
feature: Sales Channels, Products, Configuration
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Verwalten von Attributen für Amazon-Listen

Sowohl Amazon als auch [!DNL Commerce] verwenden ein System von Produkteigenschaften, die als Attribute bezeichnet werden und zur Definition eines Produkts verwendet werden. Attribute definieren die Beschreibung, den Inhalt, die Bilder, die Preise und verschiedene Daten für Ihre Produkte.

Für eine erfolgreiche Kommunikation zwischen Commerce und Amazon ist es erforderlich, dass [!DNL Commerce] -Attribute korrekt mit dem entsprechenden Amazon-Attribut verknüpft (oder abgeglichen) werden. Bei der Integration mit Amazon ordnen Sie diese Attribute Amazon-Attributen zu. Nach Abschluss kann [!DNL Commerce] Ihre Amazon-Listen mit Ihrem [!DNL Commerce] -Produktkatalog synchronisieren und verwalten.

Angenommen, Sie haben dasselbe Element in Ihrem [!DNL Commerce] -Katalog und in Amazon-Auflistungen. Ein Attribut für das Produkt kann der Listenpreis des Artikels sein. Der Name für den Listenpreis in [!DNL Commerce] könnte `Price` heißen, während der Listenpreis für Amazon `ListingPrice` lautet. Sie müssen [!DNL Commerce] anweisen, dass bei der Kommunikation mit Amazon das Attribut [!DNL Commerce] mit dem Namen `Price` mit dem Amazon-Attribut mit dem Namen `ListingPrice` übereinstimmt. Dieser Prozess wird als _Verwalten von Attributen_ bezeichnet und umfasst das Erstellen neuer und Bearbeiten vorhandener Attribute. Wenn Sie sicherstellen, dass Attribute richtig übereinstimmen, wird eine korrekte Kommunikation zwischen [!DNL Commerce] und Amazon sichergestellt.

Wenn die Attributzuordnung eingerichtet ist, kann [!DNL Commerce] Produktinformationen mit Amazon hin und her kommunizieren. Wenn Sie über Amazon-Produktlisten verfügen, kann [!DNL Commerce] Ihre Amazon-Produkte und -Details in Ihren [!DNL Commerce] -Katalog importieren, sodass Sie Ihre Amazon-Auflistungen aus einem zentralen Produktkatalog verwalten können.

Mit dem Amazon-Vertriebskanal können Sie nach Bedarf in der [_[!UICONTROL Attributes]_-Ansicht](./attributes-view.md) auf der Homepage des Amazon-Vertriebskanals auf Attribute zugreifen, diese überprüfen, erstellen und verwalten. Wenn Sie Ihrem [!DNL Commerce] -Katalog ein Attribut hinzufügen, muss dieser möglicherweise für alle Produkte aktualisiert werden.

Weitere Informationen zu [!DNL Commerce] und Amazon-Attributsätzen und -werten finden Sie unter:

- [Grundlagen zum Verwalten von Attributen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [Attribut erstellen](./creating-attributes.md#create-an-attribute)
- [Vorhandenes Attribut bearbeiten](./creating-attributes.md#edit-an-attribute)
- [Anzeigen der Attributzuordnung](./amazon-matching-attributes-values.md)
- [Bearbeiten oder Erstellen der Attributzuordnung](./amazon-manually-update-incomplete-listing.md)
