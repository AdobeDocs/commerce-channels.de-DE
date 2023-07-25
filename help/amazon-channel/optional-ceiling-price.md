---
title: "Intelligente Neupreisregel: Optionaler Höchstpreis"
description: Verwenden Sie optionale Preiseinstellungen, um Ihren höchsten Produktpreis vor den intelligenten Preisregeln zu schützen, die Ihre Amazon-Auflistungen verwalten.
feature: Sales Channels, Price Rules
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Intelligente Neupreisregel: Optionaler Höchstpreis

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- [Regeltyp auswählen](./intelligent-repricing-rules.md)
- [Bedingte Unterschiede zwischen Wettbewerbern](./competitor-conditional-variances.md)
- [Preisanpassung](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- Optionaler Höchstpreis

Die automatisierten Preiseinstellungen schützen automatisch Ihren höchsten Produktpreis vor intelligenten Preisregeln und ermöglichen es Ihnen, eine Obergrenze (den höchsten Preis) für Ihre intelligenten Preisregeln festzulegen.

## Optionalen Höchstpreis konfigurieren

Definieren Sie Ihre optionalen Einstellungen für den höchsten Preis in _[!UICONTROL Optional Ceiling Price]_Abschnitt.

1. Für **[!UICONTROL Ceiling Price Source]**, wählen Sie ein Attribut aus.

   Wählen Sie Ihre [!DNL Commerce] [Produktattribut](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) , der Ihre relative Obergrenze angibt. Wenn Sie beispielsweise nicht möchten, dass der Amazon-Listingpreis über dem MSRP Ihres Artikels liegt, wählen Sie die `Manufacturer's Suggested Retail Price` -Attribut.

1. Für **[!UICONTROL Ceiling Price Action]**, wählen Sie eine Option aus.

   - `Decrease By` - Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Ceiling Price Source]_-Wert, der nach unten angepasst werden soll, sodass ein niedrigerer Plafonds für die Regel entsteht, bevor sie an Amazon notiert wird.

   - `Increase By` - Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Ceiling Price Source]_-Wert, der angepasst werden soll, sodass ein höherer Plafonds für die Regel entsteht, bevor sie an Amazon notiert wird.

   - `Match` - Wählen Sie aus, wann der Listenpreis nicht über dem definierten Wert schwanken soll. _[!UICONTROL Ceiling Price Source]_-Wert. Wenn auf `Match`, die_[!UICONTROL Apply]_ und _[!UICONTROL Ceiling Adjustment Amount]_-Felder deaktiviert sind.

1. Lassen Sie die **[!UICONTROL Apply]** Standard `Apply as percentage`.

1. Für **[!UICONTROL Ceiling Adjustment Price]**, geben Sie den numerischen Wert für den Prozentsatz ein, um Ihre _[!UICONTROL Ceiling Price Source]_-Wert.

In diesem Beispiel wird der Höchstpreis auf 2 % unter dem MSRP des Artikels festgelegt.

![Intelligente Neupreisregelung - optionaler Höchstpreis](assets/ob-intelligent-price-rule-ceiling.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Ceiling Price Source] | Wählen Sie die [!DNL Commerce] [Produktattribut](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) , der Ihre relative Obergrenze angibt. Wenn Sie beispielsweise nicht möchten, dass der Produktlistenpreis über dem MSRP Ihres Artikels liegt, wählen Sie die `Manufacturer's Suggested Retail Price` -Attribut. |
| [!UICONTROL Ceiling Price Action] | Wählen Sie eine Preisanpassungsaktion. Optionen:<ul><li>**[!UICONTROL Decrease By]** - Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Ceiling Price Source]_-Wert, der nach unten angepasst werden soll, sodass ein niedrigerer Plafonds für die Regel entsteht, bevor sie an Amazon notiert wird.</li><li>**[!UICONTROL Increase By]** - Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Ceiling Price Source]_-Wert, der angepasst werden soll, sodass ein höherer Plafonds für die Regel entsteht, bevor sie an Amazon notiert wird.</li><li>**[!UICONTROL Match]** - Wählen Sie aus, wann der Listenpreis nicht über dem definierten Wert schwanken soll. _[!UICONTROL Ceiling Price Source]_-Wert. Wenn auf `Match`, die_[!UICONTROL Apply]_ und _[!UICONTROL Ceiling Adjustment Amount]_-Felder deaktiviert sind.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - prozentuale Anpassung im Verhältnis zum _[!UICONTROL Ceiling Price Source]_-Wert. |
| [!UICONTROL Ceiling Price Adjustment] | Geben Sie den numerischen Wert für den Prozentwert ein, um Ihre _[!UICONTROL Ceiling Price Source]_-Wert. |
