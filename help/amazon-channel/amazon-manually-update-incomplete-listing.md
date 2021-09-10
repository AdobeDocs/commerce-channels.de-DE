---
title: Aktualisieren erforderlicher Informationen (unvollständige Auflistung)
description: Der Amazon-Vertriebskanal bietet die Registerkarte Unvollständig , um Commerce-Katalogprodukte zu überwachen, bei denen die für Amazon erforderlichen Informationen fehlen.
exl-id: f278cd50-8f04-452e-b9c2-c87820f9faf2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Erforderliche Informationen aktualisieren (unvollständige Auflistung)

Die auf dem Tab _[!UICONTROL Incomplete]_angezeigten Listen enthalten Ihre [!DNL Commerce] -Katalogprodukte, die Ihren Amazon-Eignungsregeln entsprechen, aber denen Informationen fehlen, die von Amazon vor der Auflistung benötigt werden.

## Erforderliche Informationen aktualisieren (Amazon-Auflistung kann nicht zugewiesen werden) {#update-required-info-unable-to-assign-to-amazon-listing}

1. Zeigen Sie die Listen auf der Registerkarte _[!UICONTROL Incomplete]_in [Listen verwalten](./managing-product-listings.md) an.

1. Klicken Sie in der Spalte _[!UICONTROL Action]_für die Liste, die Sie aktualisieren möchten, auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie versuchen, eine Übereinstimmung mit einer Amazon-Liste zu finden.

1. Geben Sie für **[!UICONTROL Assign ASIN]** das von Amazon zugewiesene ASIN für die Liste ein, die Sie mit dem Katalogprodukt abgleichen möchten.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]**.

Die Liste wird nun mit Ihrem Katalog abgeglichen, und die Liste wird dann aktualisiert und basierend auf Ihren Cron- und Listeneinstellungen in Amazon veröffentlicht. Sie wird auch aus der Registerkarte _[!UICONTROL Incomplete]_entfernt.

![Manuelles Zuweisen von ASIN für Nichtauflistungsübereinstimmung](assets/amazon-listing-update-assign-asin.png)

## Erforderliche Informationen aktualisieren (Mehrere Übereinstimmungen gefunden) {#update-required-info-multiple-matches-found}

1. Zeigen Sie die Listen auf der Registerkarte _[!UICONTROL Incomplete]_in [[!UICONTROL Manage Listings]](./managing-product-listings.md) an.

1. Klicken Sie in der Spalte _Aktion_ auf **Wählen Sie** > **Erforderliche Informationen aktualisieren** für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie versuchen, eine Übereinstimmung mit einer Amazon-Liste zu finden.

1. Wählen Sie für **[!UICONTROL Select Correct Amazon Listing]** das richtige ASIN für die Auflistung aus, die Sie mit diesem Produkt abgleichen möchten.

   Die hier aufgeführten Optionen umfassen Katalogprodukte, die als mögliche Übereinstimmungen identifiziert werden. Wenn keine der Optionen korrekt ist, können Sie `Manually Enter Correct ASIN` auswählen und manuell das ASIN für das Produkt eingeben.

1. Wenn Sie das ASIN manuell eingeben, geben Sie das richtige ASIN für **[!UICONTROL Manually Assign ASIN]** ein.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]**.

![Manuelles Auswählen von ASIN aus mehreren möglichen Übereinstimmungen](assets/amazon-listing-update-multiple-matches.png)

## Erforderliche Informationen aktualisieren (enthält Varianten) {#update-required-info-has-variants}

1. Zeigen Sie die Listen auf der Registerkarte _[!UICONTROL Incomplete]_in [[!UICONTROL Manage Listings]](./managing-product-listings.md) an.

1. Klicken Sie in der Spalte _[!UICONTROL Action]_für die Liste, die Sie aktualisieren möchten, auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie versuchen, eine Übereinstimmung mit einer Amazon-Liste zu finden.

1. Wählen Sie für **[!UICONTROL Select Correct Amazon Listing]** das richtige ASIN für die Auflistung aus, die Sie mit diesem Produkt abgleichen möchten.

   Die hier aufgeführten Optionen umfassen Katalogprodukte, die als mögliche Übereinstimmungen identifiziert werden. Wenn keine der Optionen korrekt ist, können Sie `Manually Enter Correct ASIN` auswählen und das ASIN für das Produkt manuell eingeben.

1. Wenn Sie das ASIN manuell eingeben, geben Sie das richtige ASIN für **[!UICONTROL Manually Assign ASIN]** ein.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]**.

![Manuelles Auswählen von ASIN aus möglichen Variantenübereinstimmungen](assets/amazon-listing-update-multiple-matches.png)

## Erforderliche Informationen aktualisieren (fehlende Bedingung) {#update-required-info-missing-condition}

1. Zeigen Sie die Listen auf der Registerkarte _[!UICONTROL Incomplete]_in [Listen verwalten](./managing-product-listings.md) an.

1. Klicken Sie in der Spalte _[!UICONTROL Action]_für die Liste, die Sie aktualisieren möchten, auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie versuchen, eine Übereinstimmung mit einer Amazon-Liste zu finden.

1. Wählen Sie für **[!UICONTROL Condition]** die entsprechende Bedingung aus.

   Die Liste der verfügbaren Optionen hängt von Ihren Einstellungen für [Produktlistenbedingung](./product-listing-condition.md) ab.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]** .

![Fehlende Bedingung manuell aktualisieren](assets/amazon-update-listing-missing-condition.png)
