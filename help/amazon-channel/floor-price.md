---
title: '"Intelligente Neupreisregel: Floor Price'''
description: Verwenden Sie die Einstellungen für den Tiefstpreis, um den niedrigsten Preis für eine intelligente Preisregel zur Verwaltung Ihrer Amazon-Auflistungen zu ermitteln.
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Intelligente Neupreisregel: Grundpreis

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Die [Grundpreis](./floor-price.md) -Einstellungen schützen automatisch Ihren niedrigsten Produktpreis vor den intelligenten Preisregeln. Verwenden Sie diese Einstellungen, um eine Untergrenze (niedrigsten Preis) für Ihre intelligenten Preisregeln festzulegen und sicherzustellen, dass Ihre Produkte nicht unter einem gewünschten Preis aufgeführt werden.

Floor-Preisattribute basieren auf dem Umfang der Website, wenn Ihre [!DNL Commerce] Store verwendet den Umfang der Website-Preise. Siehe [Preisumfang](./price-scope.md).

Der Floor-Preis wird nur verwendet, wenn **[!UICONTROL Rule Type]** auf `Intelligent repricing rule`.

## Grundpreis konfigurieren

Definieren Sie Ihre niedrigste Preiseinstellung im _[!UICONTROL Floor Price]_Abschnitt.

1. Für **[!UICONTROL Floor Price Source]**, wählen Sie ein Preisquellenattribut aus.

   Wählen Sie die [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}, das Ihre relative Bodenbegrenzung angibt. Wenn Sie beispielsweise nicht möchten, dass der Listenpreis für Amazon unter den Artikelkosten liegt, wählen Sie die *Kosten* -Attribut.

1. Für **[!UICONTROL Floor Price Action]**, wählen Sie eine Option aus.

   - `Decrease By` - Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Floor Price Source]_-Wert, der nach unten angepasst werden soll, sodass ein niedrigerer Mindestpreis für die Regel entsteht, bevor sie an Amazon notiert wird.

   - `Increase By` - Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Floor Price Source]_-Wert, der angepasst werden soll, wodurch ein höherer Grundpreis für die Regel entsteht, bevor sie an Amazon notiert wird.

   - `Match` - Wählen Sie aus, wann der Listenpreis nicht unter dem definierten Wert schwanken soll. _[!UICONTROL Floor Price Source]_-Wert. Wenn auf `Match`, die_[!UICONTROL Apply]_ und _[!UICONTROL Floor Adjustment Amount]_-Felder deaktiviert sind.

1. Lassen Sie die **[!UICONTROL Apply]** Standard `Apply as percentage`.

1. Für **[!UICONTROL Floor Adjustment Price]**, geben Sie den numerischen Wert für den Prozentsatz ein, um Ihre _[!UICONTROL Floor Price Source]_-Wert.

In diesem Beispiel wird der Grundpreis auf 3 % über den Kosten des Artikels festgelegt.

![Beispiel einer intelligenten Neupreisregel - Grundpreis](assets/ob-intelligent-pricde-rule-floor-price.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Floor Price Source] | Wählen Sie die [!DNL Commerce] -Attribut, das Ihre relative Untergrenze (niedrigster Preis) angibt. Wenn Sie beispielsweise nicht möchten, dass der Listenpreis für Amazon unter den Artikelkosten liegt, wählen Sie die `Cost` -Attribut. |
| [!UICONTROL Floor Price Action] | Wählen Sie eine Preisanpassungsaktion. Optionen:<ul><li>**[!UICONTROL Decrease By]** - Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Floor Price Source]_-Wert, der nach unten angepasst werden soll, sodass ein niedrigerer Mindestpreis für die Regel entsteht, bevor sie an Amazon notiert wird.</li><li>**[!UICONTROL Increase By]** - Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Floor Price Source]_-Wert, der angepasst werden soll, wodurch ein höherer Grundpreis für die Regel entsteht, bevor sie an Amazon notiert wird.</li><li>**[!UICONTROL Match]** - Wählen Sie aus, wann der Listenpreis nicht unter dem definierten Wert schwanken soll. _[!UICONTROL Floor Price Source]_-Wert. Wenn ausgewählt, wird die_[!UICONTROL Apply]_ und _[!UICONTROL Floor Adjustment Amount]_-Felder deaktiviert sind.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - prozentuale Anpassung im Verhältnis zum _[!UICONTROL Floor Price Source]_-Wert. |
| [!UICONTROL Floor Adjustment Amount] | Geben Sie den numerischen Wert für den Prozentwert ein, um Ihre _[!UICONTROL Floor Price Source]_-Wert. |
