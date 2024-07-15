---
title: Aktualisieren erforderlicher Informationen zu Amazon
description: Der Amazon-Vertriebskanal bietet die Registerkarte Unvollständig , um Commerce-Katalogprodukte zu überwachen, bei denen die für Amazon erforderlichen Informationen fehlen.
feature: Sales Channels, Merchandising, Catalog Management, Products
exl-id: f278cd50-8f04-452e-b9c2-c87820f9faf2
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Aktualisieren erforderlicher Informationen (unvollständige Auflistung)

Auf der Registerkarte &quot;_[!UICONTROL Incomplete]_&quot;angezeigte Listen enthalten Ihre [!DNL Commerce] -Katalogprodukte, die Ihren Amazon-Eignungsregeln entsprechen, aber Informationen fehlen, die von Amazon vor der Auflistung benötigt werden.

## Aktualisierung erforderlicher Informationen (Zuweisung zur Amazon-Auflistung nicht möglich) {#update-required-info-unable-to-assign-to-amazon-listing}

1. Zeigen Sie die Auflistungen auf der Registerkarte _[!UICONTROL Incomplete]_in [Auflistungen verwalten](./managing-product-listings.md) an.

1. Klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie eine Übereinstimmung mit einer Amazon-Liste suchen.

1. Geben Sie für &quot;**[!UICONTROL Assign ASIN]**&quot;das von Amazon zugewiesene ASIN für die Liste ein, die mit dem Katalogprodukt übereinstimmen soll.

1. Klicken Sie auf **[!UICONTROL Save Listing Update]**, um die Produktübereinstimmung zu speichern.

Die Liste wird nun mit Ihrem Katalog abgeglichen, und die Liste wird dann aktualisiert und basierend auf Ihren Cron- und Listeneinstellungen in Amazon veröffentlicht. Sie wird auch aus der Registerkarte _[!UICONTROL Incomplete]_entfernt.

![Manuelles Zuweisen von ASIN für Nichtübereinstimmung mit einer Auflistung](assets/amazon-listing-update-assign-asin.png){width="600" zoomable="yes"}

## Erforderliche Informationen aktualisieren (mehrere Übereinstimmungen gefunden) {#update-required-info-multiple-matches-found}

1. Zeigen Sie die Listen auf der Registerkarte _[!UICONTROL Incomplete]_in [[!UICONTROL Manage Listings]](./managing-product-listings.md) an.

1. Klicken Sie in der Spalte _Aktion_ auf **Auswählen** > **Erforderliche Informationen aktualisieren** für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie eine Übereinstimmung mit einer Amazon-Liste suchen.

1. Wählen Sie für **[!UICONTROL Select Correct Amazon Listing]** das richtige ASIN für die Auflistung aus, die Sie mit diesem Produkt abgleichen möchten.

   Die hier aufgeführten Optionen umfassen Katalogprodukte, die als mögliche Übereinstimmungen identifiziert werden. Wenn keine der Optionen korrekt ist, können Sie `Manually Enter Correct ASIN` auswählen und das ASIN für das Produkt manuell eingeben.

1. Wenn Sie das ASIN manuell eingeben, geben Sie das richtige ASIN für **[!UICONTROL Manually Assign ASIN]** ein.

1. Klicken Sie auf **[!UICONTROL Save Listing Update]**, um die Produktübereinstimmung zu speichern.

![Wählen Sie ASIN manuell aus mehreren möglichen Übereinstimmungen aus](assets/amazon-listing-update-multiple-matches.png){width="600" zoomable="yes"}

## Erforderliche Informationen aktualisieren (enthält Varianten) {#update-required-info-has-variants}

1. Zeigen Sie die Listen auf der Registerkarte _[!UICONTROL Incomplete]_in [[!UICONTROL Manage Listings]](./managing-product-listings.md) an.

1. Klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie eine Übereinstimmung mit einer Amazon-Liste suchen.

1. Wählen Sie für **[!UICONTROL Select Correct Amazon Listing]** das richtige ASIN für die Auflistung aus, die Sie mit diesem Produkt abgleichen möchten.

   Die hier aufgeführten Optionen umfassen Katalogprodukte, die als mögliche Übereinstimmungen identifiziert werden. Wenn keine der Optionen korrekt ist, können Sie `Manually Enter Correct ASIN` auswählen und das ASIN für das Produkt manuell eingeben.

1. Wenn Sie das ASIN manuell eingeben, geben Sie das richtige ASIN für **[!UICONTROL Manually Assign ASIN]** ein.

1. Klicken Sie auf **[!UICONTROL Save Listing Update]**, um die Produktübereinstimmung zu speichern.

## Erforderliche Informationen aktualisieren (fehlende Bedingung) {#update-required-info-missing-condition}

1. Zeigen Sie die Auflistungen auf der Registerkarte _[!UICONTROL Incomplete]_in [Auflistungen verwalten](./managing-product-listings.md) an.

1. Klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie eine Übereinstimmung mit einer Amazon-Liste suchen.

1. Wählen Sie für **[!UICONTROL Condition]** die entsprechende Bedingung aus.

   Die Liste der verfügbaren Optionen hängt von Ihren Einstellungen für die [Produktauflistungsbedingung](./product-listing-condition.md) ab.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]** .

![Manuelles Aktualisieren der fehlenden Bedingung](assets/amazon-update-listing-missing-condition.png){width="600" zoomable="yes"}
