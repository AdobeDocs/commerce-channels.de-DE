---
title: Attribute verwalten
description: Sie können die Zuordnung von Commerce-Produktattributen zu den Amazon-Attributen verwalten, um genaue Produktinformationen zwischen den Systemen sicherzustellen.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Attribute verwalten

Amazon und [!DNL Commerce] Beide verwenden ein System von Produkteigenschaften, die als Attribute bezeichnet werden und zur Definition eines Produkts verwendet werden. Attribute definieren die Beschreibung, den Inhalt, die Bilder, die Preise und verschiedene Daten für Ihre Produkte.

Eine erfolgreiche Kommunikation zwischen Commerce und Amazon erfordert Folgendes: [!DNL Commerce] -Attribute korrekt dem entsprechenden Amazon-Attribut zugeordnet (oder zugeordnet) werden. Bei der Integration mit Amazon ordnen Sie diese Attribute Amazon-Attributen zu. Wenn abgeschlossen, [!DNL Commerce] Sie können Ihre Amazon-Listen mit Ihren [!DNL Commerce] Produktkatalog.

Angenommen, Sie haben dasselbe Element in Ihrem [!DNL Commerce] Katalog- und Amazon-Listen. Ein Attribut für das Produkt kann der Listenpreis des Artikels sein. Der Name des Listenpreises in [!DNL Commerce] könnte `Price`, während der Listenpreis für Amazon `ListingPrice`. Sie müssen [!DNL Commerce] bei der Kommunikation mit Amazon [!DNL Commerce] Attribut benannt `Price` entspricht dem Amazon-Attribut namens `ListingPrice`. Dieser Prozess heißt _Verwalten von Attributen_ und umfasst das Erstellen neuer und Bearbeiten vorhandener Attribute. Sicherstellen, dass Attribute richtig zugeordnet werden, stellt eine korrekte Kommunikation zwischen [!DNL Commerce] und Amazon.

Wenn die Attributzuordnung eingerichtet ist, [!DNL Commerce] kann Produktinformationen mit Amazon hin und her kommunizieren. Wenn Sie Amazon-Produktlisten haben, [!DNL Commerce] Sie können Ihre Amazon-Produkte und -Details in Ihre [!DNL Commerce] -Katalog, in dem Sie Ihre Amazon-Auflistungen aus einem zentralen Produktkatalog verwalten können.

Mit dem Amazon-Vertriebskanal können Sie nach Bedarf Attribute im [_[!UICONTROL Attributes]_Ansicht](./attributes-view.md) auf der Startseite des Amazon-Vertriebskanals. Wenn Sie Ihrem [!DNL Commerce] -Kataloge verwenden, könnte eine Aktualisierung dieser Werte für alle Produkte erforderlich sein.

Weitere Informationen finden Sie unter [!DNL Commerce] und Amazon-Attributsätze und -werte finden Sie unter:

- [Grundlagen zum Verwalten von Attributen](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"}
- [Attribut erstellen](./creating-attributes.md#create-an-attribute)
- [Vorhandenes Attribut bearbeiten](./creating-attributes.md#edit-an-attribute)
- [Anzeigen der Attributzuordnung](./amazon-matching-attributes-values.md)
- [Bearbeiten oder Erstellen der Attributzuordnung](./amazon-manually-update-incomplete-listing.md)
