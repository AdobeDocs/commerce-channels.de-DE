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

Auf der Seite _[!UICONTROL Incomplete]_einschließen [!DNL Commerce] Katalogprodukte, die Ihren Amazon-Eignungsanforderungen gemäß Ihren Listening-Regeln entsprechen, aber Informationen fehlen, die von Amazon vor der Auflistung benötigt werden.

## Erforderliche Informationen aktualisieren (Amazon-Auflistung kann nicht zugewiesen werden) {#update-required-info-unable-to-assign-to-amazon-listing}

1. Die Listen im _[!UICONTROL Incomplete]_Registerkarte in [Verwalten von Listen](./managing-product-listings.md).

1. Im _[!UICONTROL Action]_Spalte, klicken Sie auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie eine Übereinstimmung mit einer Amazon-Liste suchen.

1. Für **[!UICONTROL Assign ASIN]** Geben Sie das von Amazon zugewiesene ASIN für die Auflistung ein, die Sie mit dem Katalogprodukt abgleichen möchten.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]**.

Die Liste wird nun mit Ihrem Katalog abgeglichen, und die Liste wird dann aktualisiert und basierend auf Ihren Cron- und Listeneinstellungen in Amazon veröffentlicht. Es wird auch aus dem _[!UICONTROL Incomplete]_Registerkarte.

![Manuelles Zuweisen von ASIN für Nichtauflistungsübereinstimmung](assets/amazon-listing-update-assign-asin.png)

## Erforderliche Informationen aktualisieren (Mehrere Übereinstimmungen gefunden) {#update-required-info-multiple-matches-found}

1. Die Listen im _[!UICONTROL Incomplete]_Registerkarte in [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. Im _Aktion_ Spalte, klicken Sie auf **Auswählen** > **Erforderliche Informationen aktualisieren** für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie eine Übereinstimmung mit einer Amazon-Liste suchen.

1. Für **[!UICONTROL Select Correct Amazon Listing]**, wählen Sie das richtige ASIN für die Auflistung aus, die Sie diesem Produkt zuordnen möchten.

   Die hier aufgeführten Optionen umfassen Katalogprodukte, die als mögliche Übereinstimmungen identifiziert werden. Wenn keine der Optionen korrekt ist, können Sie `Manually Enter Correct ASIN` und geben Sie das ASIN für das Produkt manuell ein.

1. Wenn Sie das ASIN manuell eingeben, geben Sie das richtige ASIN für **[!UICONTROL Manually Assign ASIN]**.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]**.

![Manuelles Auswählen von ASIN aus mehreren möglichen Übereinstimmungen](assets/amazon-listing-update-multiple-matches.png)

## Erforderliche Informationen aktualisieren (enthält Varianten) {#update-required-info-has-variants}

1. Die Listen im _[!UICONTROL Incomplete]_Registerkarte in [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. Im _[!UICONTROL Action]_Spalte, klicken Sie auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie eine Übereinstimmung mit einer Amazon-Liste suchen.

1. Für **[!UICONTROL Select Correct Amazon Listing]**, wählen Sie das richtige ASIN für die Auflistung aus, die Sie diesem Produkt zuordnen möchten.

   Die hier aufgeführten Optionen umfassen Katalogprodukte, die als mögliche Übereinstimmungen identifiziert werden. Wenn keine der Optionen korrekt ist, können Sie `Manually Enter Correct ASIN` und geben Sie das ASIN für das Produkt manuell ein.

1. Wenn Sie das ASIN manuell eingeben, geben Sie das richtige ASIN für **[!UICONTROL Manually Assign ASIN]**.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]**.

![Manuelles Auswählen von ASIN aus möglichen Variantenübereinstimmungen](assets/amazon-listing-update-multiple-matches.png)

## Erforderliche Informationen aktualisieren (fehlende Bedingung) {#update-required-info-missing-condition}

1. Die Listen im _[!UICONTROL Incomplete]_Registerkarte in [Verwalten von Listen](./managing-product-listings.md).

1. Im _[!UICONTROL Action]_Spalte, klicken Sie auf **[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**für die Liste, die Sie aktualisieren möchten.

1. Überprüfen Sie die Katalogproduktinformationen (SKU und Produktname), für die Sie eine Übereinstimmung mit einer Amazon-Liste suchen.

1. Für **[!UICONTROL Condition]**, wählen Sie die entsprechende Bedingung aus.

   Die Liste der verfügbaren Optionen hängt von Ihrer [Produktlistenbedingung](./product-listing-condition.md) -Einstellungen.

1. Um die Produktübereinstimmung zu speichern, klicken Sie auf **[!UICONTROL Save Listing Update]** .

![Fehlende Bedingung manuell aktualisieren](assets/amazon-update-listing-missing-condition.png)
