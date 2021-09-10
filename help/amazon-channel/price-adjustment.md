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
>Der Abschnitt &quot;Preisanpassung&quot;unterscheidet sich geringfügig für Standard- und intelligente Neupreisregeln. **[!UICONTROL Match Competitor Price]** ist nur verfügbar unter  _[!UICONTROL Price Action]_, wenn **[!UICONTROL Rule Type]**auf  `Intelligent repricing rule`gesetzt ist.

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- [Regeltyp auswählen](./intelligent-repricing-rules.md)
- [Bedingte Unterschiede zwischen Wettbewerbern](./competitor-conditional-variances.md)
- Preisanpassung
- [Floor Price](./floor-price.md)
- [Optionaler Höchstpreis](./optional-ceiling-price.md)

Die Preisanpassung definiert die Preisberechnung, wenn Sie die Preisquelle des Konkurrenten ermittelt haben.

## Preisanpassung konfigurieren

Definieren Sie Ihre Preisanpassung im Abschnitt _[!UICONTROL Price Adjustment]_.

1. Wählen Sie für **[!UICONTROL Price Action]** eine Option:

   - `Decrease By` - Wählen Sie aus, wann der definierte Preis-Quellwert angepasst werden soll, um einen niedrigeren Preis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.

   - `Increase By` - Wählen Sie aus, wann der definierte Preisquellenwert angepasst werden soll, um einen höheren Preis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.

   - `Match Competitor Price` - (Nur intelligente Neupreisregel) Wählen Sie aus, wann Sie Ihren Amazon-Listingpreis basierend auf Ihrem Konkurrenten-Feedback und Ihren Varianzparametern an den  [niedrigsten ](./lowest-competitor-pricing.md) Wettbewerbspreis anpassen möchten. Wenn auf `Match Competitor Price` gesetzt, werden die Felder _[!UICONTROL Apply]_und_[!UICONTROL Adjustment Amount]_ entfernt.

1. Wählen Sie für **[!UICONTROL Apply]** eine Option:

   - `Apply as percentage` - Wählen Sie aus, wann die in Ihrem  **[!UICONTROL Magento Price Source]** Listing- [ ](./listing-price.md) Preis definierte Variable um einen Prozentwert angepasst werden soll.

   - `Apply as fixed amount` - Wählen Sie aus, wann die in Ihrem  **[!UICONTROL Magento Price Source]** Listing- [ ](./listing-price.md) Preis definierte Variable um einen festen Betrag angepasst werden soll.

1. Geben Sie für **[!UICONTROL Adjustment Amount]** (erforderlich) den numerischen Wert für die Preisanpassung ein.

   - Wenn **[!UICONTROL Apply]** auf `Apply as percentage` gesetzt ist, geben Sie den Prozentwert ein (Beispiel: `25` für eine 25%ige Anpassung eingeben).

   - Wenn **[!UICONTROL Apply]** auf `Apply as fixed amount` gesetzt ist, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: `25` für eine feste Anpassung von 25 USD eingeben).

![Intelligente Neupreisregelung - Preisanpassung](assets/amazon-price-adjustment.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Price Action] | Wählen Sie eine Preisanpassungsaktion. Optionen:<br>**[!UICONTROL Decrease By]**- Wählen Sie aus, wann der in [Listing Price](./listing-price.md) definierte definierte _[!UICONTROL Magento Price Source]_-Wert angepasst werden soll, um einen niedrigeren Preis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.<br>**[!UICONTROL Increase By]**- Wählen Sie aus, wann die in Ihrem_[!UICONTROL Magento Price Source]_ Listing- [Preis ](./listing-price.md) definierte Regel angepasst werden soll, um einen höheren Preis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.<br>**[!UICONTROL Match Competitor Price]**- (Nur intelligente Neupreisregel) Wählen Sie aus, wann Sie Ihren Amazon-Listingpreis basierend auf Ihrem Konkurrenten-Feedback und Ihren Varianzparametern an den  [niedrigsten ](./lowest-competitor-pricing.md) Wettbewerbspreis anpassen möchten. Wenn ausgewählt, werden die Felder _Apply_ und _Adjustment Amount_ entfernt. |
| [!UICONTROL Apply] | Optionen:<br>**[!UICONTROL Apply as percentage]**- Wählen Sie aus, wann der definierte _[!UICONTROL Magento Price Source]_in Ihrem [Listing Price](./listing-price.md) um einen Prozentwert angepasst werden soll.<br>**[!UICONTROL Apply as fixed amount]**- Wählen Sie aus, wann die in Ihrem_[!UICONTROL Magento Price Source]_ Listing- [ ](./listing-price.md) Preis definierte Variable um einen festen Betrag angepasst werden soll. |
| [!UICONTROL Adjustment Amount] | Erforderlich.<br>Wenn Sie  `Apply as percentage` für  **[!UICONTROL Apply]** wählen, geben Sie den Prozentwert ein (Beispiel: 25 %  `25` für eine Anpassung).<br>Wenn Sie  `Apply as fixed amount` für  **[!UICONTROL Apply]** wählen, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: für  `25` eine feste Anpassung von 25 USD). |
