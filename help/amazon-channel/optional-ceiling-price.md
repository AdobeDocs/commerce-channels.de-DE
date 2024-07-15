---
title: "Intelligente Neupreisregel: Optionaler Höchstpreis"
description: Verwenden Sie optionale Preiseinstellungen, um Ihren höchsten Produktpreis vor den intelligenten Preisregeln zu schützen, die Ihre Amazon-Auflistungen verwalten.
feature: Sales Channels, Price Rules
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Intelligente Neupreisregel: Optionaler Höchstpreis

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- [Regeltyp auswählen](./intelligent-repricing-rules.md)
- [Bedingte Unterschiede zwischen Wettbewerbern](./competitor-conditional-variances.md)
- [Preisanpassung](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- Optionaler Höchstpreis

Die automatisierten Preiseinstellungen für die Obergrenze schützen automatisch Ihren höchsten Produktpreis vor intelligenten Preisregeln und ermöglichen es Ihnen, eine Obergrenze (den höchsten Preis) für Ihre intelligenten Preisregeln festzulegen.

## Optionalen Höchstpreis konfigurieren

Definieren Sie Ihre optionalen Einstellungen für den höchsten Preis im Abschnitt _[!UICONTROL Optional Ceiling Price]_.

1. Wählen Sie für **[!UICONTROL Ceiling Price Source]** ein Attribut aus.

   Wählen Sie Ihr [!DNL Commerce] [Produktattribut](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) aus, das Ihre relative Obergrenze angibt. Wenn Sie beispielsweise nicht möchten, dass der Listenpreis für Amazon über dem MSRP Ihres Artikels liegt, wählen Sie das Attribut `Manufacturer's Suggested Retail Price` aus.

1. Wählen Sie für **[!UICONTROL Ceiling Price Action]** eine Option aus.

   - `Decrease By` - Wählen Sie aus, wann der definierte _[!UICONTROL Ceiling Price Source]_-Wert nach unten angepasst werden soll, um einen niedrigeren Plafonds für die Regel zu erstellen, bevor Sie sie in Amazon auflisten.

   - `Increase By` - Wählen Sie aus, wann der definierte _[!UICONTROL Ceiling Price Source]_-Wert angepasst werden soll, um einen höheren Plafonds für die Regel zu erstellen, bevor Sie sie in Amazon auflisten.

   - `Match` - Wählen Sie aus, wann der Listenpreis nicht über dem definierten _[!UICONTROL Ceiling Price Source]_-Wert schwanken soll. Wenn der Wert auf `Match` gesetzt ist, sind die Felder_[!UICONTROL Apply]_ und _[!UICONTROL Ceiling Adjustment Amount]_deaktiviert.

1. Belassen Sie den Standardwert **[!UICONTROL Apply]** auf `Apply as percentage`.

1. Geben Sie für **[!UICONTROL Ceiling Adjustment Price]** den numerischen Wert für den Prozentsatz ein, um Ihren _[!UICONTROL Ceiling Price Source]_-Wert anzupassen.

In diesem Beispiel wird der Höchstpreis auf 2 % unter dem MSRP des Artikels festgelegt.

![Intelligente Neupreisregel - optionaler Höchstpreis](assets/ob-intelligent-price-rule-ceiling.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Ceiling Price Source] | Wählen Sie das [!DNL Commerce] [Produktattribut](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) aus, das Ihre relative Obergrenze angibt. Wenn Sie beispielsweise nicht möchten, dass der Preis für die Produktliste über dem MSRP Ihres Artikels liegt, wählen Sie das Attribut `Manufacturer's Suggested Retail Price` aus. |
| [!UICONTROL Ceiling Price Action] | Wählen Sie eine Preisanpassungsaktion. Optionen:<ul><li>**[!UICONTROL Decrease By]** - Wählen Sie aus, wann der definierte _[!UICONTROL Ceiling Price Source]_-Wert nach unten angepasst werden soll, um einen niedrigeren Plafonds für die Regel zu erstellen, bevor Sie sie in Amazon auflisten.</li><li>**[!UICONTROL Increase By]** - Wählen Sie aus, wann der definierte _[!UICONTROL Ceiling Price Source]_-Wert angepasst werden soll, um einen höheren Plafonds für die Regel zu erstellen, bevor Sie sie in Amazon auflisten.</li><li>**[!UICONTROL Match]** - Wählen Sie aus, wann der Listenpreis nicht über dem definierten _[!UICONTROL Ceiling Price Source]_-Wert schwanken soll. Wenn der Wert auf `Match` gesetzt ist, sind die Felder_[!UICONTROL Apply]_ und _[!UICONTROL Ceiling Adjustment Amount]_deaktiviert.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Eine prozentuale Anpassung in Bezug auf den _[!UICONTROL Ceiling Price Source]_-Wert. |
| [!UICONTROL Ceiling Price Adjustment] | Geben Sie den numerischen Wert für den Prozentwert ein, um den _[!UICONTROL Ceiling Price Source]_-Wert anzupassen. |
