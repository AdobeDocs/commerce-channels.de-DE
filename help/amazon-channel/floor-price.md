---
title: "Intelligente Neupreisregel: Floor Price"
description: Verwenden Sie die Einstellungen für den Tiefstpreis, um den niedrigsten Preis für eine intelligente Preisregel zur Verwaltung Ihrer Amazon-Auflistungen zu ermitteln.
feature: Sales Channels, Price Rules
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Intelligente Neupreisregel: Grundpreis

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Die Einstellungen für den [Grundpreis](./floor-price.md) schützen automatisch Ihren niedrigsten Produktpreis vor den intelligenten Preisregeln. Verwenden Sie diese Einstellungen, um eine Untergrenze (niedrigsten Preis) für Ihre intelligenten Preisregeln festzulegen und sicherzustellen, dass Ihre Produkte nicht unter einem gewünschten Preis aufgeführt werden.

Floor-Preisattribute basieren auf dem Umfang der Website, wenn Ihr [!DNL Commerce]-Store den Umfang der Website-Preise verwendet. Siehe [Preisumfang](./price-scope.md).

Der Floor-Preis wird nur verwendet, wenn **[!UICONTROL Rule Type]** auf `Intelligent repricing rule` gesetzt ist.

## Grundpreis konfigurieren

Definieren Sie Ihre niedrigste Preiseinstellung im Abschnitt _[!UICONTROL Floor Price]_.

1. Wählen Sie für **[!UICONTROL Floor Price Source]** ein Preisquellenattribut aus.

   Wählen Sie das [!DNL Commerce] [Produktattribut](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) aus, das Ihre relative Bodenbegrenzung angibt. Wenn Sie beispielsweise nicht möchten, dass der Listenpreis in Amazon unter den Kosten Ihres Artikels liegt, wählen Sie das Attribut *Kosten* aus.

1. Wählen Sie für **[!UICONTROL Floor Price Action]** eine Option aus.

   - `Decrease By` - Legen Sie fest, wann der definierte _[!UICONTROL Floor Price Source]_-Wert nach unten angepasst werden soll, um einen niedrigeren Tiefstpreis für die Regel zu erstellen, bevor Sie sie in Amazon auflisten.

   - `Increase By` - Legen Sie fest, wann der definierte _[!UICONTROL Floor Price Source]_-Wert angepasst werden soll, um einen höheren Unterbietungspreis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.

   - `Match` - Wählen Sie aus, wann der Listenpreis nicht unter dem definierten _[!UICONTROL Floor Price Source]_-Wert schwanken soll. Wenn der Wert auf `Match` gesetzt ist, sind die Felder_[!UICONTROL Apply]_ und _[!UICONTROL Floor Adjustment Amount]_deaktiviert.

1. Belassen Sie den Standardwert **[!UICONTROL Apply]** auf `Apply as percentage`.

1. Geben Sie für **[!UICONTROL Floor Adjustment Price]** den numerischen Wert für den Prozentsatz ein, um Ihren _[!UICONTROL Floor Price Source]_-Wert anzupassen.

In diesem Beispiel wird der Grundpreis auf 3 % über den Kosten des Artikels festgelegt.

![Beispiel für eine intelligente Neupreisregel - Grundpreis](assets/ob-intelligent-pricde-rule-floor-price.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Floor Price Source] | Wählen Sie das Attribut [!DNL Commerce] aus, das Ihre relative Untergrenze (niedrigster Preis) angibt. Wenn Sie beispielsweise nicht möchten, dass der Listenpreis für Amazon unter den Kosten Ihres Artikels liegt, wählen Sie das Attribut `Cost` aus. |
| [!UICONTROL Floor Price Action] | Wählen Sie eine Preisanpassungsaktion. Optionen:<ul><li>**[!UICONTROL Decrease By]** - Legen Sie fest, wann der definierte _[!UICONTROL Floor Price Source]_-Wert nach unten angepasst werden soll, um einen niedrigeren Tiefstpreis für die Regel zu erstellen, bevor Sie sie in Amazon auflisten.</li><li>**[!UICONTROL Increase By]** - Legen Sie fest, wann der definierte _[!UICONTROL Floor Price Source]_-Wert angepasst werden soll, um einen höheren Unterbietungspreis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.</li><li>**[!UICONTROL Match]** - Wählen Sie aus, wann der Listenpreis nicht unter dem definierten _[!UICONTROL Floor Price Source]_-Wert schwanken soll. Wenn diese Option aktiviert ist, sind die Felder_[!UICONTROL Apply]_ und _[!UICONTROL Floor Adjustment Amount]_deaktiviert.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Eine prozentuale Anpassung in Bezug auf den _[!UICONTROL Floor Price Source]_-Wert. |
| [!UICONTROL Floor Adjustment Amount] | Geben Sie den numerischen Wert für den Prozentwert ein, um den _[!UICONTROL Floor Price Source]_-Wert anzupassen. |
