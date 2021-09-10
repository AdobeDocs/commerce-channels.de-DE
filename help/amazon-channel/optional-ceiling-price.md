---
title: '"Intelligente Neupreisregel: Optionaler Höchstpreis"'
description: Verwenden Sie optionale Preiseinstellungen, um Ihren höchsten Produktpreis vor den intelligenten Preisregeln zu schützen, die Ihre Amazon-Auflistungen verwalten.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Intelligente Neupreisregel: fakultativer Höchstpreis

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- [Regeltyp auswählen](./intelligent-repricing-rules.md)
- [Bedingte Unterschiede zwischen Wettbewerbern](./competitor-conditional-variances.md)
- [Preisanpassung](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- Optionaler Höchstpreis

Die automatisierten Preiseinstellungen schützen automatisch Ihren höchsten Produktpreis vor intelligenten Preisregeln und ermöglichen es Ihnen, eine Obergrenze (den höchsten Preis) für Ihre intelligenten Preisregeln festzulegen.

## Optionalen Höchstpreis konfigurieren

Definieren Sie Ihre optionalen Einstellungen für den höchsten Preis im Abschnitt _[!UICONTROL Optional Ceiling Price]_.

1. Wählen Sie für **[!UICONTROL Ceiling Price Source]** ein Attribut aus.

   Wählen Sie Ihr [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;} aus, das Ihre relative Obergrenze angibt. Wenn Sie z. B. nicht möchten, dass der Amazon-Listenpreis über dem MSRP Ihres Artikels liegt, wählen Sie das Attribut `Manufacturer's Suggested Retail Price`.

1. Wählen Sie für **[!UICONTROL Ceiling Price Action]** eine Option aus.

   - `Decrease By` - Wählen Sie aus, wann der definierte  _[!UICONTROL Ceiling Price Source]_Wert angepasst werden soll, und erstellen Sie einen niedrigeren Maximalwert für die Regel, bevor Sie sie in Amazon auflisten.

   - `Increase By` - Wählen Sie aus, wann der definierte  _[!UICONTROL Ceiling Price Source]_Wert angepasst werden soll, wodurch ein höherer Plafonds für die Regel entsteht, bevor Sie sie in Amazon auflisten.

   - `Match` - Wählen Sie aus, wann der Listenpreis nicht über dem definierten  _[!UICONTROL Ceiling Price Source]_Wert schwanken soll. Wenn auf `Match` gesetzt, sind die Felder_[!UICONTROL Apply]_ und _[!UICONTROL Ceiling Adjustment Amount]_deaktiviert.

1. Behalten Sie den Standardwert **[!UICONTROL Apply]** bei `Apply as percentage`.

1. Geben Sie für **[!UICONTROL Ceiling Adjustment Price]** den numerischen Wert für den Prozentwert ein, um den Wert _[!UICONTROL Ceiling Price Source]_anzupassen.

In diesem Beispiel wird der Höchstpreis auf 2 % unter dem MSRP des Artikels festgelegt.

![Intelligente Neupreisregelung - optionaler Höchstpreis](assets/ob-intelligent-price-rule-ceiling.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Ceiling Price Source] | Wählen Sie das [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;} aus, das Ihre relative Obergrenze angibt. Wenn Sie beispielsweise nicht möchten, dass der Preis für die Produktauflistung über dem MSRP Ihres Artikels liegt, wählen Sie das Attribut `Manufacturer's Suggested Retail Price`. |
| [!UICONTROL Ceiling Price Action] | Wählen Sie eine Preisanpassungsaktion. Optionen:<ul><li>**[!UICONTROL Decrease By]** - Wählen Sie aus, wann der definierte  _[!UICONTROL Ceiling Price Source]_Wert angepasst werden soll, und erstellen Sie einen niedrigeren Maximalwert für die Regel, bevor Sie sie in Amazon auflisten.</li><li>**[!UICONTROL Increase By]** - Wählen Sie aus, wann der definierte  _[!UICONTROL Ceiling Price Source]_Wert angepasst werden soll, wodurch ein höherer Plafonds für die Regel entsteht, bevor Sie sie in Amazon auflisten.</li><li>**[!UICONTROL Match]** - Wählen Sie aus, wann der Listenpreis nicht über dem definierten  _[!UICONTROL Ceiling Price Source]_Wert schwanken soll. Wenn auf `Match` gesetzt, sind die Felder_[!UICONTROL Apply]_ und _[!UICONTROL Ceiling Adjustment Amount]_deaktiviert.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Eine prozentuale Anpassung in Bezug auf den  _[!UICONTROL Ceiling Price Source]_Wert. |
| [!UICONTROL Ceiling Price Adjustment] | Geben Sie den numerischen Wert für den Prozentwert ein, um den Wert _[!UICONTROL Ceiling Price Source]_anzupassen. |
