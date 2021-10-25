---
title: '"Intelligente Preisanpassungsregel: Floor Price'''
description: Verwenden Sie Tiefstpreiseinstellungen, um den niedrigsten Preis für eine intelligente Preisregel zur Verwaltung Ihrer Amazon-Auflistungen zu bestimmen.
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Intelligente Preisanpassungsregel: Tiefstpreis

Zu den Abschnitten einer intelligenten Neubewertungsregel gehören:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Die [Tiefstpreis](./floor-price.md) schützt automatisch Ihren niedrigsten Produktpreis vor den intelligenten Preisregeln. Verwenden Sie diese Einstellungen, um einen Tiefstwert (niedrigster Preis) für Ihre intelligenten Preisregeln festzulegen und sicherzustellen, dass Ihre Produkte nicht unter dem gewünschten Preis aufgeführt werden.

Floor-Preisattribute basieren auf dem Websitebereich, wenn Ihre [!DNL Commerce] Store verwendet Website-Preisbereich. Siehe [Preisumfang](./price-scope.md).

Floor-Preis wird nur verwendet, wenn **[!UICONTROL Rule Type]** ist eingestellt auf `Intelligent repricing rule`.

## Tiefstpreis konfigurieren

Definieren Sie die niedrigste Preiseinstellung im _[!UICONTROL Floor Price]_Abschnitt.

1. für **[!UICONTROL Floor Price Source]**, wählen Sie ein Preisquellenattribut.

   Wählen Sie [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){Zielgruppe=&quot;_blank&quot;}, die Ihre relative Bodengrenze angibt. Wenn Sie z. B. nicht möchten, dass der Amazon-Listungspreis unter den Kosten Ihres Artikels liegt, wählen Sie *Kosten* Attribut.

1. für **[!UICONTROL Floor Price Action]**, wählen Sie eine Option aus.

   - `Decrease By` - Wählen Sie aus, wann die _[!UICONTROL Floor Price Source]_-Wert nach unten zu korrigieren, um einen niedrigeren Tiefstpreis für die Regel zu erzielen, bevor sie an Amazon notiert wird.

   - `Increase By` - Wählen Sie aus, wann die _[!UICONTROL Floor Price Source]_-Wert anzupassen, um einen höheren Tiefstpreis für die Regel zu erzielen, bevor sie an Amazon notiert wird.

   - `Match` - Wählen Sie aus, wenn der Börsennotierungspreis nicht unter dem definierten Wert schwanken soll _[!UICONTROL Floor Price Source]_Wert. Wenn festgelegt auf `Match`,_[!UICONTROL Apply]_ und _[!UICONTROL Floor Adjustment Amount]_Felder sind deaktiviert.

1. Verlassen Sie die **[!UICONTROL Apply]** default as `Apply as percentage`.

1. für **[!UICONTROL Floor Adjustment Price]**, geben Sie den numerischen Wert für den Prozentwert ein, um Ihre _[!UICONTROL Floor Price Source]_Wert.

In diesem Beispiel wird der Tiefstpreis auf 3 % über den Kosten des Artikels festgesetzt.

![Beispiel für intelligente Preisanpassungsregeln - Tiefstpreis](assets/ob-intelligent-pricde-rule-floor-price.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Floor Price Source] | Wählen Sie [!DNL Commerce] Attribut, das Ihre relative Untergrenze (niedrigster Preis) angibt. Wenn Sie z. B. nicht möchten, dass der Amazon-Listungspreis unter den Kosten Ihres Artikels liegt, wählen Sie `Cost` Attribut. |
| [!UICONTROL Floor Price Action] | Wählen Sie eine Preisanpassungsaktion aus. Optionen:<ul><li>**[!UICONTROL Decrease By]** - Wählen Sie aus, wann die _[!UICONTROL Floor Price Source]_-Wert nach unten zu korrigieren, um einen niedrigeren Tiefstpreis für die Regel zu erzielen, bevor sie an Amazon notiert wird.</li><li>**[!UICONTROL Increase By]** - Wählen Sie aus, wann die _[!UICONTROL Floor Price Source]_-Wert anzupassen, um einen höheren Tiefstpreis für die Regel zu erzielen, bevor sie an Amazon notiert wird.</li><li>**[!UICONTROL Match]** - Wählen Sie aus, wenn der Börsennotierungspreis nicht unter dem definierten Wert schwanken soll _[!UICONTROL Floor Price Source]_Wert. Bei Auswahl der_[!UICONTROL Apply]_ und _[!UICONTROL Floor Adjustment Amount]_Felder sind deaktiviert.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - Eine prozentuale Anpassung in Bezug auf _[!UICONTROL Floor Price Source]_Wert. |
| [!UICONTROL Floor Adjustment Amount] | Geben Sie den numerischen Wert für den Prozentwert ein, um Ihre _[!UICONTROL Floor Price Source]_Wert. |
