---
title: Attribute verwalten
description: Sie können die Zuordnung von Commerce-Produktattributen zu den Amazon-Attributen verwalten, um genaue Produktinformationen zwischen den Systemen sicherzustellen.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Attribute verwalten

Amazon und [!DNL Commerce] verwenden beide ein System von Produkteigenschaften, die als Attribute bezeichnet werden und zur Definition eines Produkts verwendet werden. Attribute definieren die Beschreibung, den Inhalt, die Bilder, die Preise und verschiedene Daten für Ihre Produkte.

Für eine erfolgreiche Kommunikation zwischen Commerce und Amazon müssen die [!DNL Commerce]-Attribute dem entsprechenden Amazon-Attribut korrekt zugeordnet (oder zugeordnet) werden. Bei der Integration mit Amazon ordnen Sie diese Attribute Amazon-Attributen zu. Wenn Sie fertig sind, kann [!DNL Commerce] Ihre Amazon-Listen mit Ihrem [!DNL Commerce]-Produktkatalog synchronisieren und verwalten.

Angenommen, Sie haben denselben Artikel in Ihrem [!DNL Commerce] -Katalog und in Amazon-Auflistungen. Ein Attribut für das Produkt kann der Listenpreis des Artikels sein. Der Name für den Listingpreis in [!DNL Commerce] könnte `Price` lauten, während der Listenpreis für Amazon möglicherweise `ListingPrice` heißt. Sie müssen [!DNL Commerce] anweisen, dass bei der Kommunikation mit Amazon das [!DNL Commerce]-Attribut `Price` mit dem Amazon-Attribut `ListingPrice` übereinstimmt. Dieser Prozess wird als _Verwalten von Attributen_ bezeichnet und umfasst das Erstellen neuer und Bearbeiten vorhandener Attribute. Wenn Sie sicherstellen, dass Attribute richtig zugeordnet sind, wird eine korrekte Kommunikation zwischen [!DNL Commerce] und Amazon sichergestellt.

Wenn die Attributzuordnung eingerichtet ist, kann [!DNL Commerce] Produktinformationen mit Amazon hin und her kommunizieren. Wenn Sie über Amazon-Produktlisten verfügen, kann [!DNL Commerce] Ihre Amazon-Produkte und -Details in Ihren [!DNL Commerce]-Katalog importieren, sodass Sie Ihre Amazon-Auflistungen aus einem zentralen Produktkatalog verwalten können.

Mit dem Amazon-Vertriebskanal können Sie nach Bedarf in der [_[!UICONTROL Attributes]_-Ansicht](./attributes-view.md) auf der Homepage des Amazon-Vertriebskanals auf Attribute zugreifen, diese überprüfen, erstellen und verwalten. Wenn Sie Ihrem [!DNL Commerce]-Katalog ein Attribut hinzufügen, muss dieser möglicherweise für alle Produkte aktualisiert werden.

Weitere Informationen zu [!DNL Commerce] und Amazon-Attributsätzen und -werten finden Sie unter:

- [Grundlagen zum Verwalten von Attributen](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}
- [Attribut erstellen](./creating-attributes.md#create-an-attribute)
- [Vorhandenes Attribut bearbeiten](./creating-attributes.md#edit-an-attribute)
- [Anzeigen der Attributzuordnung](./amazon-matching-attributes-values.md)
- [Bearbeiten oder Erstellen der Attributzuordnung](./amazon-manually-update-incomplete-listing.md)
