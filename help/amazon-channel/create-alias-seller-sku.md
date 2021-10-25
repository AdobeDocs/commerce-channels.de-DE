---
title: Alias Amazon Seller SKU erstellen
description: Sie können die Alias Amazon Seller SKU verwenden, um aus Ihren Commerce-Katalogprodukten regionenübergreifende Amazon-Listen zu erstellen.
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Alias Amazon Seller SKU erstellen

An [!DNL Alias Amazon Seller SKU] wird verwendet, um eine Amazon-Liste aus demselben Produkt in Ihrem [!DNL Commerce] Katalog. Wenn Sie ein erfahrener Amazon-Verkäufer sind, kennen Sie die [Amazon Global SKU](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){Zielgruppe=&quot;_blank&quot;} und Marketplace-spezifische SKU für Inventar und Versand. Nach ähnlichen Grundsätzen für Amazon Sales Kanal kontrolliert die Amazon Seller SKU die Produktitelauflistungsinformationen auf multiregionaler Ebene und [!DNL Alias Amazon Seller SKU] kann zur Kontrolle der Produktlistungsinformationen auf regionaler Ebene verwendet werden.

Diese Funktion kann zwei Funktionen erfüllen:

- Erstellen Sie eine [!DNL Alias Amazon Seller SKU] für einen Ihrer [!DNL Commerce] Katalogprodukte zur Kontrolle regionsspezifischer Listungsinformationen.

   **Beispiel**: Sie sind Verkäufer sowohl in den USA als auch in Kanada. Achten Sie darauf, dass jedem Ihrer Amazon Sales Kanal Stores während des Setups nur eine Amazon Region zugewiesen werden kann. Sie haben also einen Amazon Sales Kanal Store mit einer definierten US-Region und einen anderen Store mit einer bestimmten kanadischen Region. Beide Läden teilen sich Ihre [!DNL Commerce] Katalog zur Auflistung von Informationen in beiden Regionen, einschließlich der Amazon Seller SKU und ASIN Produktattribute. Die Auflistungen für das Katalogprodukt wären also in beiden Geschäften gleich, Preisfreigabe, Lager-/Mengenangabe und andere Produktattribute. Aber Ihr Bestand für Kanada speichert Schiffe von einem kanadischen Standort aus, und Ihre USA speichern Schiffe von einem US-amerikanischen Standort. Daher sollten Sie die Listungsmenge für die Auflistung für jeden Laden separat kontrollieren. Um diese Art von regionsspezifischer Steuerung zu erreichen, können Sie eine Alias Amazon Seller SKU erstellen.

   Im Wesentlichen können Sie eine Alias Amazon Seller SKU erstellen, die mit demselben Katalogprodukt verknüpft ist und dazu verwendet werden kann, dieselbe Auflistung in diesem Bereich erneut zu veröffentlichen.

- Erstellen Sie eine [!DNL Alias Amazon Seller SKU] und einem Ihrer [!DNL Commerce] in zwei Amazon-Auflistungen.

   **Beispiel**: Sie verfügen über ein Katalogprodukt, das mit einer Amazon-Auflistung übereinstimmt. Da Amazon häufig mehrere Auflistungen hat, die dasselbe Produkt darstellen, entdecken Sie eine andere Amazon-Liste für dasselbe Produkt, aber Amazon hat der Liste ein anderes ASIN zugewiesen. Um die Sichtbarkeit Ihres Produkts zu erhöhen und es einzuschließen, sollten Sie Ihr Katalogprodukt mit den verschiedenen ASIN abgleichen und Auflistungen für beide ASIN-Werte erstellen. Dazu können Sie eine Alias Amazon Seller SKU erstellen.

   Im Grunde können Sie eine [!DNL Alias Amazon Seller SKU] die verwendet werden kann, um ein einzelnes Katalogprodukt einer zweiten Amazon-Auflistung zuzuordnen und eine Liste für das neu übereinstimmende ASIN zu erstellen. In diesem Fall würden Sie zwei Amazon-Einträge für dasselbe Katalogprodukt haben.

   Nachdem Sie eine Alias Amazon Seller SKU erstellt haben, können Sie die Listeneinstellungen, -regeln und -überschreibungen verwenden, um die Listungsinformationen für die Region zu steuern. Zu den Produktmerkmalen, die pro Region für eine Auflistung definiert werden können, gehören Quantität/Bestand, Fulfillment-Methode, Bedingung, Produktberechtigung und Bearbeitungszeit.

## für einen regionsspezifischen Zweck verwendet werden {#region-specific}

Ansicht der Auflistung im _[!UICONTROL Product Listings]_Seite (_[!UICONTROL Inactive]_, _Aktiv_, _Nicht förderfähig_ oder _Beendet_ Tabulator).

1. Unter _[!UICONTROL Actions]_, klicken **[!UICONTROL Create Alias Seller SKU]**.

1. für **[!UICONTROL Assign New Seller SKU]**, geben Sie einen eindeutigen alphanumerischen Wert ein.

   Dieser Wert muss eindeutig sein (wird nicht für ein anderes Produkt oder einen anderen Alias in Ihrem Katalog verwendet).

1. für **[!UICONTROL Assign New ASIN]**, keine Änderung.

   Dieser Wert wird automatisch mit dem Produkt-ASIN gefüllt, das mit Ihrem Katalogprodukt übereinstimmt. Wenn Sie diesen Wert ändern, wird Ihr Katalogprodukt auf zwei Amazon-Auflistungen basierend auf ASIN angezeigt.

1. Umschalten **[!UICONTROL Remove Existing Seller SKU]** bei Bedarf.

   - `Yes` - Wählen Sie, um die Liste zu löschen und eine Liste mit den neuen Informationen zu erstellen.

   - `No` - Wählen Sie , um eine Liste zu erstellen und die alte Liste unverändert beizubehalten.

1. Klick **[!UICONTROL Save Listing Update]**.

## Wird verwendet, um ein einzelnes Katalogprodukt mit zwei Amazon-Auflistungen abzugleichen

1. Ansicht der Auflistung im _[!UICONTROL Product Listings]_Seite (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_ oder _[!UICONTROL Ended]_Tabulatoren).

1. Unter _[!UICONTROL Actions]_, klicken **[!UICONTROL Create Alias Seller SKU]**.

1. für **[!UICONTROL Assign New Seller SKU]**, geben Sie einen eindeutigen alphanumerischen Wert ein.

   Dieser Wert muss eindeutig sein (wird nicht für ein anderes Produkt oder einen anderen Alias in Ihrem Katalog verwendet).

1. für **[!UICONTROL Assign New ASIN]**, geben Sie einen eindeutigen alphanumerischen Wert ein.

   Dieser Wert wird automatisch mit dem Produkt-ASIN gefüllt, das mit Ihrem Katalogprodukt übereinstimmt. Wenn Sie diesen Wert ändern, wird Ihr Katalogprodukt auf zwei Amazon-Auflistungen basierend auf ASIN angezeigt.

1. Umschalten **[!UICONTROL Remove Existing Seller SKU]** bei Bedarf.

   - `Yes` - Wählen Sie, um die Liste zu löschen und eine Liste mit den neuen Informationen zu erstellen.

   - `No` - Wählen Sie , um eine andere Liste zu erstellen und die alte Liste unverändert zu lassen.

1. Klick **[!UICONTROL Save Listing Update]**.

![Alias Amazon Seller SKU erstellen](assets/amazon-alias-sku-create.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Assign New Seller SKU] | Geben Sie einen neuen, eindeutigen alphanumerischen Wert ein, der mit der ursprünglichen Amazon Seller-SKU verknüpft werden soll. Diese Nummer wird nur von Amazon Sales Kanal verwendet, um mit Ihrem Katalogprodukt zu übereinstimmen. Sie können einen beliebigen SKU-Wert verwenden, der Wert kann jedoch nur einmal in Ihrem Katalog verwendet werden. |
| [!UICONTROL Assign New ASIN] | Geben Sie den ASIN-Wert für die Liste ein, mit der Sie Ihr Katalogprodukt abgleichen möchten. Ändern Sie dieses Feld nur, wenn Sie ein einzelnes Katalogprodukt mit dem ASIN für eine andere Auflistung für dasselbe Produkt abgleichen. Dieser Wert muss mit dem von Amazon zugewiesenen ASIN übereinstimmen. Andernfalls wird die Auflistung von Amazon nicht abgelehnt. |
| [!UICONTROL Remove Existing Seller SKU] | Optionen:<ul><li>**[!UICONTROL Yes]** - Wählen Sie, um die Liste zu löschen und eine Liste mit den neuen Informationen zu erstellen. Die neue Liste erscheint im _[!UICONTROL Active]_und die alte Liste wird in die_ Beendet _Tabulator.</li><li>**[!UICONTROL No]** - Wählen Sie , um eine andere Liste zu erstellen und die alte Liste unverändert zu lassen. Beide Einträge werden nach dem Erstellen der neuen Liste im Register Aktiv angezeigt.</li></ul> |
