---
title: Alias Amazon Seller SKU erstellen
description: Sie können die Alias Amazon Seller SKU verwenden, um aus Ihren Commerce-Katalogprodukten regionenübergreifende Amazon-Listen zu erstellen.
feature: Sales Channels, Products
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# Alias Amazon Seller SKU erstellen

Mit dem Wert &quot;[!DNL Alias Amazon Seller SKU]&quot;können Sie eine Amazon-Liste aus demselben Produkt in Ihrem [!DNL Commerce] -Katalog erstellen. Wenn Sie ein erfahrener Amazon-Verkäufer sind, sind Sie möglicherweise mit der [Amazon Global SKU](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target="_blank"} und der Marketplace-spezifischen SKU für Inventar und Versand vertraut. Nach ähnlichen Prinzipien für den Amazon-Vertriebskanal kontrolliert die Amazon Seller SKU Produktanlistungsinformationen auf regionaler Ebene und die [!DNL Alias Amazon Seller SKU] kann verwendet werden, um Produktanlistungsinformationen auf regionsspezifischer Ebene zu steuern.

Mit dieser Funktion können zwei Funktionen ausgeführt werden:

- Erstellen Sie einen [!DNL Alias Amazon Seller SKU] für eines Ihrer [!DNL Commerce] -Katalogprodukte, um regionsspezifische Listendaten zu steuern.

  **Beispiel**: Sie sind ein Verkäufer in den USA und Kanada. Beachten Sie, dass jedem Ihrer Amazon-Verkaufskanalspeicher während der Einrichtung nur eine Amazon-Region zugewiesen werden kann. Sie verfügen also über einen Amazon-Verkaufskanalspeicher mit einer definierten US-Region und einen weiteren Store mit einer definierten Region in Kanada. Beide Stores verwenden Ihren [!DNL Commerce] -Katalog, um Informationen in beiden Regionen aufzulisten, einschließlich der Amazon Seller SKU und der ASIN-Produktattribute. Die Listen für das Katalogprodukt wären also in beiden Geschäften identisch, d. h. in den Bereichen Sharing-Preis, Lager/Menge und anderen Produktattributen. Aber Ihr Lager für Kanada wird von einem kanadischen Standort aus befördert, und Ihr US-Geschäft wird von einem US-Standort aus befördert. Daher sollten Sie die Listenmenge für die Auflistung für jeden Store separat kontrollieren. Um diese Art von regionsspezifischer Kontrolle auszuführen, können Sie eine Alias Amazon Seller SKU erstellen.

  Im Grunde können Sie eine Alias Amazon Seller SKU erstellen, die mit demselben Katalogprodukt verknüpft ist und verwendet werden kann, um dieselbe Liste in dieser Region erneut zu veröffentlichen.

- Erstellen Sie einen [!DNL Alias Amazon Seller SKU] und ordnen Sie eines Ihrer [!DNL Commerce] -Katalogprodukte zwei Amazon-Auflistungen zu.

  **Beispiel**: Sie haben ein Katalogprodukt, das mit einer Amazon-Auflistung übereinstimmt. Da Amazon häufig über mehrere Auflistungen verfügt, die dasselbe Produkt repräsentieren, finden Sie eine weitere Amazon-Liste für dasselbe Produkt, Amazon hat der Auflistung jedoch ein anderes ASIN zugewiesen. Um die Sichtbarkeit Ihres Produkts zu erhöhen und einzubeziehen, möchten Sie Ihr Katalogprodukt mit den verschiedenen ASIN-Werten abgleichen und Auflistungen für beide ASIN-Werte erstellen. Dazu können Sie eine Alias Amazon Seller SKU erstellen.

  Im Grunde können Sie einen [!DNL Alias Amazon Seller SKU] erstellen, der verwendet werden kann, um ein einzelnes Katalogprodukt einer zweiten Amazon-Auflistung zuzuordnen und eine Liste für das neu übereinstimmende ASIN zu erstellen. In diesem Szenario würden Sie zwei Amazon-Auflistungen für dasselbe Katalogprodukt haben.

  Nachdem Sie eine Alias Amazon Seller-SKU erstellt haben, können Sie Ihre Listeneinstellungen, Regeln und Überschreibungen verwenden, um die Listeninformationen für die Region zu steuern. Zu den Produktattributen, die pro Region für eine Auflistung definiert werden können, gehören Menge/Lager, Erfüllungsmethode, Bedingung, Produkteignung und Bearbeitungszeit.

## Wird für einen regionsspezifischen Zweck verwendet {#region-specific}

Zeigen Sie die Liste auf der Seite _[!UICONTROL Product Listings]_an ( Registerkarte_[!UICONTROL Inactive]_, _Aktiv_, _Nicht qualifiziert_ oder _Beendet_).

1. Klicken Sie unter _[!UICONTROL Actions]_auf **[!UICONTROL Create Alias Seller SKU]**.

1. Geben Sie für &quot;**[!UICONTROL Assign New Seller SKU]**&quot;einen eindeutigen alphanumerischen Wert ein.

   Dieser Wert muss eindeutig sein (nicht für andere Produkte oder Alias in Ihrem Katalog).

1. Nehmen Sie für **[!UICONTROL Assign New ASIN]** keine Änderung vor.

   Dieser Wert wird automatisch mit dem Produkt-ASIN ausgefüllt, das mit Ihrem Katalogprodukt übereinstimmt. Wenn Sie diesen Wert ändern, wird Ihr Katalogprodukt basierend auf dem ASIN in zwei Amazon-Listen überführt.

1. Schalten Sie die Option **[!UICONTROL Remove Existing Seller SKU]** nach Bedarf um.

   - `Yes` - Wählen Sie aus, die Liste zu löschen und mithilfe der neuen Informationen eine Liste zu erstellen.

   - `No` - Wählen Sie aus, eine Liste zu erstellen und die alte Liste unverändert zu lassen.

1. Klicken Sie auf **[!UICONTROL Save Listing Update]**.

## Wird verwendet, um ein einzelnes Katalogprodukt mit zwei Amazon-Listen abzugleichen

1. Zeigen Sie die Liste auf der Seite _[!UICONTROL Product Listings]_an ( Registerkarten_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_ oder _[!UICONTROL Ended]_).

1. Klicken Sie unter _[!UICONTROL Actions]_auf **[!UICONTROL Create Alias Seller SKU]**.

1. Geben Sie für &quot;**[!UICONTROL Assign New Seller SKU]**&quot;einen eindeutigen alphanumerischen Wert ein.

   Dieser Wert muss eindeutig sein (nicht für andere Produkte oder Alias in Ihrem Katalog).

1. Geben Sie für &quot;**[!UICONTROL Assign New ASIN]**&quot;einen eindeutigen alphanumerischen Wert ein.

   Dieser Wert wird automatisch mit dem Produkt-ASIN ausgefüllt, das mit Ihrem Katalogprodukt übereinstimmt. Wenn Sie diesen Wert ändern, wird Ihr Katalogprodukt basierend auf dem ASIN in zwei Amazon-Listen überführt.

1. Schalten Sie die Option **[!UICONTROL Remove Existing Seller SKU]** nach Bedarf um.

   - `Yes` - Wählen Sie aus, die Liste zu löschen und mithilfe der neuen Informationen eine Liste zu erstellen.

   - `No` - Wählen Sie aus, eine weitere Liste zu erstellen und die alte Liste unverändert zu lassen.

1. Klicken Sie auf **[!UICONTROL Save Listing Update]**.

![Erstellen einer Alias-Amazon-Verkäufer-SKU](assets/amazon-alias-sku-create.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Assign New Seller SKU] | Geben Sie einen neuen, eindeutigen alphanumerischen Wert ein, der mit der Amazon Seller SKU verknüpft werden soll. Diese Nummer wird nur vom Amazon-Vertriebskanal verwendet, um sie mit Ihrem Katalogprodukt abzustimmen. Sie können einen beliebigen SKU-Wert verwenden, der Wert kann jedoch nur einmal in Ihrem Katalog verwendet werden. |
| [!UICONTROL Assign New ASIN] | Geben Sie den ASIN-Wert für die Auflistung ein, mit der Sie Ihr Katalogprodukt abgleichen möchten. Ändern Sie dieses Feld nur, wenn Sie ein einzelnes Katalogprodukt mit dem ASIN für eine andere Liste desselben Produkts verknüpfen. Dieser Wert muss mit dem von Amazon zugewiesenen ASIN übereinstimmen. Andernfalls wird die Liste von Amazon nicht abgelehnt. |
| [!UICONTROL Remove Existing Seller SKU] | Optionen:<ul><li>**[!UICONTROL Yes]** - Wählen Sie aus, die Liste zu löschen und mithilfe der neuen Informationen eine Liste zu erstellen. Die neue Liste wird auf der Registerkarte _[!UICONTROL Active]_angezeigt und die alte Liste wird auf die Registerkarte_ Beendet _verschoben.</li><li>**[!UICONTROL No]** - Wählen Sie aus, eine weitere Liste zu erstellen und die alte Liste unverändert zu lassen. Beide Listen werden auf der Registerkarte Aktiv angezeigt, nachdem die neue Liste erstellt wurde.</li></ul> |
