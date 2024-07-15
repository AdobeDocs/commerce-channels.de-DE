---
title: Amazon-Verkaufskanal - [!UICONTROL Price Adjustment]
description: Konfigurieren Sie Preisanpassungen, um die Preisberechnung zu definieren, wenn Sie die Preisquelle des Amazon-Konkurrenten ermittelt haben.
feature: Sales Channels, Price Rules
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# [!UICONTROL Price Adjustment]

>[!NOTE]
>
>Der Abschnitt &quot;Preisanpassung&quot;unterscheidet sich geringfügig für Standard- und intelligente Neupreisregeln. **[!UICONTROL Match Competitor Price]** ist nur unter _[!UICONTROL Price Action]_verfügbar, wenn **[!UICONTROL Rule Type]**auf `Intelligent repricing rule` gesetzt ist.

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

   - `Decrease By` - Wählen Sie aus, wann der definierte Preisquellenwert angepasst werden soll, um einen niedrigeren Preis für die Regel zu erzielen, bevor Sie sie an Amazon auflisten.

   - `Increase By` - Wählen Sie aus, wann der definierte Preisquellenwert angepasst werden soll, um einen höheren Preis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.

   - `Match Competitor Price` - (Nur intelligente Neupreisregel) Wählen Sie aus, wann Sie Ihren Amazon-Listingpreis entsprechend dem Preis [kleinster Konkurrent](./lowest-competitor-pricing.md) ändern möchten, basierend auf Ihrem Feedback des Konkurrenten und den Varianzparametern. Wenn der Wert auf `Match Competitor Price` gesetzt ist, werden die Felder _[!UICONTROL Apply]_und_[!UICONTROL Adjustment Amount]_ entfernt.

1. Wählen Sie für **[!UICONTROL Apply]** eine Option:

   - `Apply as percentage` - Legen Sie fest, wann der definierte **[!UICONTROL Magento Price Source]** in Ihrem [Listing Price](./listing-price.md) um einen Prozentsatz angepasst werden soll.

   - `Apply as fixed amount` - Legen Sie fest, wann der definierte **[!UICONTROL Magento Price Source]** in Ihrem [Listing Price](./listing-price.md) um einen festen Betrag angepasst werden soll.

1. Geben Sie für &quot;**[!UICONTROL Adjustment Amount]**&quot;(erforderlich) den numerischen Wert für die Preisanpassung ein.

   - Wenn **[!UICONTROL Apply]** auf `Apply as percentage` gesetzt ist, geben Sie den Prozentwert ein (Beispiel: geben Sie `25` für eine 25-%-Einstellung ein).

   - Wenn **[!UICONTROL Apply]** auf `Apply as fixed amount` gesetzt ist, geben Sie den numerischen Wert für den festen Betrag ein (Beispiel: geben Sie `25` für eine feste Anpassung von 25 USD ein).

![Intelligente Neupreisregel - Preisanpassung](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | Wählen Sie eine Preisanpassungsaktion. Optionen:<br>**[!UICONTROL Decrease By]**- Wählen Sie aus, wann der in Ihrem [Listing Price](./listing-price.md) definierte definierte _[!UICONTROL Magento Price Source]_angepasst werden soll, um einen niedrigeren Preis für die Regel zu erzielen, bevor Sie Amazon auflisten.<br>**[!UICONTROL Increase By]**- Legen Sie fest, wann der in Ihrem [Listing Price](./listing-price.md) definierte definierte_[!UICONTROL Magento Price Source]_ angepasst werden soll, um einen höheren Preis für die Regel zu erzielen, bevor Sie Amazon auflisten.<br>**[!UICONTROL Match Competitor Price]**- (Nur intelligente Neupreisregel) Wählen Sie aus, wann Sie Ihren Amazon-Listingpreis entsprechend dem Preis [kleinster Konkurrent](./lowest-competitor-pricing.md) ändern möchten, basierend auf Ihrem Feedback des Konkurrenten und den Varianzparametern. Wenn ausgewählt, werden die Felder _Apply_ und _Adjustment Amount_ entfernt. |
| [!UICONTROL Apply] | Optionen:<br>**[!UICONTROL Apply as percentage]**- Wählen Sie aus, wann der definierte _[!UICONTROL Magento Price Source]_in Ihrem [Listing Price](./listing-price.md) um einen Prozentsatz angepasst werden soll.<br>**[!UICONTROL Apply as fixed amount]**- Legen Sie fest, wann der definierte_[!UICONTROL Magento Price Source]_ in Ihrem [Listing Price](./listing-price.md) um einen festen Betrag angepasst werden soll. |
| [!UICONTROL Adjustment Amount] | Erforderlich.<br>Wenn Sie `Apply as percentage` für **[!UICONTROL Apply]** auswählen, geben Sie den Prozentwert ein (Beispiel: geben Sie `25` für eine 25%ige Anpassung ein).<br>Wenn Sie `Apply as fixed amount` für **[!UICONTROL Apply]** auswählen, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: Geben Sie `25` für eine feste Anpassung von 25 USD ein). |
