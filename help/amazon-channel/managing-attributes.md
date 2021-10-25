---
title: Attribute verwalten
description: Sie können die Zuordnung von Commerce-Produktattributen zu den Amazon-Attributen verwalten, um genaue Produktinformationen zwischen den Systemen zu gewährleisten.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Attribute verwalten

Amazon und [!DNL Commerce] beide verwenden ein System von Produkteigenschaften, die als Attribute bezeichnet werden und zur Definition eines Produkts verwendet werden. Attribute definieren die Beschreibung, den Inhalt, die Bilder, die Preise und verschiedene Daten für Ihre Produkte.

Eine erfolgreiche Kommunikation zwischen Handel und Amazon erfordert Folgendes: [!DNL Commerce] -Attributen korrekt dem entsprechenden Amazon-Attribut zugeordnet (oder zugeordnet) werden. Bei der Integration mit Amazon ordnen Sie diese Attribute Amazon-Attributen zu. Wenn abgeschlossen, [!DNL Commerce] Ihre Amazon-Listen können mit Ihren [!DNL Commerce] Produktkatalog.

Stellen Sie sich beispielsweise vor, Sie haben das gleiche Element in Ihrem [!DNL Commerce] Kataloge und Amazon-Listen. Ein Attribut für das Produkt kann der Börsenkurs des Artikels sein. Der Name des Börsenkurses in [!DNL Commerce] kann benannt werden `Price`, während der Börsennotierungspreis für Amazon benannt werden könnte `ListingPrice`. Du musst dir Anweisungen geben [!DNL Commerce] dass bei der Kommunikation mit Amazon [!DNL Commerce] Attribut benannt `Price` entspricht dem Amazon-Attribut mit dem Namen `ListingPrice`. Dieser Prozess wird _Attribute verwalten_, einschließlich der Erstellung neuer und Bearbeitung vorhandener Attribute. Durch die korrekte Zuordnung der Attribute wird eine korrekte Kommunikation zwischen [!DNL Commerce] und Amazon.

Wenn die Attributzuordnung eingerichtet ist, [!DNL Commerce] kann Produktinformationen mit Amazon hin und her kommunizieren. Wenn Sie Amazon-Produktlisten haben, [!DNL Commerce] kann Amazon-Produkte und -Details in Ihre [!DNL Commerce] -Katalog, mit dem Sie Ihre Amazon-Auflistungen aus einem einzigen, zentralen Produktkatalog verwalten können.

Mit dem Amazon Sales Kanal können Sie bei Bedarf auf Attribute zugreifen, diese überprüfen, erstellen und verwalten im [_[!UICONTROL Attributes]_Ansicht](./attributes-view.md) auf der Amazon Sales Kanal Startseite. Wenn Sie dem Attribut [!DNL Commerce] -Katalogeintrag, kann eine Aktualisierung dieser Werte für alle Produkte erforderlich sein.

Für weitere Informationen über [!DNL Commerce] und Amazon-Attributsätze und -werte:

- [Grundlagen zu Attributen verwalten](https://docs.magento.com/user-guide/catalog/product-attributes.html){Zielgruppe=&quot;_blank&quot;}
- [Attribut erstellen](./creating-attributes.md#create-an-attribute)
- [Vorhandenes Attribut bearbeiten](./creating-attributes.md#edit-an-attribute)
- [Ansicht-Attributzuordnung](./amazon-matching-attributes-values.md)
- [Attributzuordnung bearbeiten oder erstellen](./amazon-manually-update-incomplete-listing.md)
