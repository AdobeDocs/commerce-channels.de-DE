---
title: Preisanpassung
description: Konfigurieren Sie Preisanpassungen, um die Preisberechnung zu definieren, wenn Sie die Preisquelle des Amazon-Konkurrenten ermittelt haben.
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Preisanpassung

>[!NOTE]
>
>Der Bereich Preisanpassung unterscheidet sich leicht von Standard- und Intelligent Reprice-Regeln. **[!UICONTROL Match Competitor Price]** ist nur verfügbar unter _[!UICONTROL Price Action]_wann **[!UICONTROL Rule Type]**ist eingestellt auf `Intelligent repricing rule`.

Zu den Abschnitten einer intelligenten Neubewertungsregel gehören:

- [Regeltyp auswählen](./intelligent-repricing-rules.md)
- [Bedingte Abweichungen des Konkurrenten](./competitor-conditional-variances.md)
- Preisanpassung
- [Floor-Preis](./floor-price.md)
- [Optionaler Höchstpreis](./optional-ceiling-price.md)

Die Preisanpassung definiert die Preisberechnung, wenn Sie die Preisquelle des Konkurrenten ermittelt haben.

## Preisanpassung konfigurieren

Definieren Sie Ihre Preisanpassung im _[!UICONTROL Price Adjustment]_Abschnitt.

1. für **[!UICONTROL Price Action]**, wählen Sie eine Option aus:

   - `Decrease By` - Wählen Sie aus, wann der festgelegte Wert der Preisquelle nach unten angepasst werden soll, um einen niedrigeren Preis für die Regel zu erzielen, bevor Sie sie für Amazon aufgeben.

   - `Increase By` - Wählen Sie aus, wann der festgelegte Wert der Preisquelle angepasst werden soll, um einen höheren Preis für die Regel zu erzielen, bevor Sie sie für Amazon aufgeben.

   - `Match Competitor Price` - (Nur intelligente Preisanpassungsregel) Wählen Sie aus, wann Sie Ihren Amazon-Listingpreis ändern möchten, um ihn an die [kleinster Konkurrent](./lowest-competitor-pricing.md) Preis, basierend auf Ihrem Konkurrent Feedback und Varianzparametern. Wenn festgelegt auf `Match Competitor Price`, _[!UICONTROL Apply]_und_[!UICONTROL Adjustment Amount]_ Felder werden entfernt.

1. für **[!UICONTROL Apply]**, wählen Sie eine Option aus:

   - `Apply as percentage` - Wählen Sie aus, wann die **[!UICONTROL Magento Price Source]** definiert in [Listingpreis](./listing-price.md) um einen Prozentsatz angepasst.

   - `Apply as fixed amount` - Wählen Sie aus, wann die **[!UICONTROL Magento Price Source]** definiert in [Listingpreis](./listing-price.md) angepasst um einen festen Betrag.

1. für **[!UICONTROL Adjustment Amount]** (erforderlich), geben Sie den numerischen Wert für die Preisanpassung ein.

   - Wann **[!UICONTROL Apply]** ist eingestellt auf `Apply as percentage`, geben Sie den Prozentwert ein (Beispiel: Eingabe `25` 25 % Anpassung).

   - Wann **[!UICONTROL Apply]** ist eingestellt auf `Apply as fixed amount`, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: Eingabe `25` für eine feste Anpassung um 25 Dollar).

![Intelligente Preisanpassungsregel - Preisanpassung](assets/amazon-price-adjustment.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Price Action] | Wählen Sie eine Preisanpassungsaktion aus. Optionen:<br>**[!UICONTROL Decrease By]**- Wählen Sie aus, wann die _[!UICONTROL Magento Price Source]_definiert in [Listingpreis](./listing-price.md) um nach unten korrigiert zu werden, was einen niedrigeren Preis für die Regel ergibt, bevor sie an Amazon notiert wird.<br>**[!UICONTROL Increase By]**- Wählen Sie aus, wann die_[!UICONTROL Magento Price Source]_ definiert in [Listingpreis](./listing-price.md) zu bereinigen, um einen höheren Preis für die Regel zu erzielen, bevor sie an Amazon notiert wird.<br>**[!UICONTROL Match Competitor Price]**- (Nur intelligente Preisanpassungsregel) Wählen Sie aus, wann Sie Ihren Amazon-Listingpreis ändern möchten, um ihn an die [kleinster Konkurrent](./lowest-competitor-pricing.md) Preis, basierend auf Ihrem Konkurrent Feedback und Varianzparametern. Bei Auswahl der _Übernehmen_ und _Anpassungsbetrag_ Felder werden entfernt. |
| [!UICONTROL Apply] | Optionen:<br>**[!UICONTROL Apply as percentage]**- Wählen Sie aus, wann die _[!UICONTROL Magento Price Source]_definiert in [Listingpreis](./listing-price.md) um einen Prozentsatz angepasst.<br>**[!UICONTROL Apply as fixed amount]**- Wählen Sie aus, wann die_[!UICONTROL Magento Price Source]_ definiert in [Listingpreis](./listing-price.md) angepasst um einen festen Betrag. |
| [!UICONTROL Adjustment Amount] | Erforderlich.<br>Wenn Sie möchten `Apply as percentage` für **[!UICONTROL Apply]**, geben Sie den Prozentwert ein (Beispiel: Eingabe `25` 25 % Anpassung).<br>Wenn Sie möchten `Apply as fixed amount` für **[!UICONTROL Apply]**, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: Eingabe `25` für eine feste Anpassung um 25 Dollar). |
