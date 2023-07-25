---
title: Amazon-Vertriebskanal - [!UICONTROL Price Adjustment]
description: Konfigurieren Sie Preisanpassungen, um die Preisberechnung zu definieren, wenn Sie die Preisquelle des Amazon-Konkurrenten ermittelt haben.
feature: Sales Channels, Price Rules
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# [!UICONTROL Price Adjustment]

>[!NOTE]
>
>Der Abschnitt &quot;Preisanpassung&quot;unterscheidet sich geringfügig für Standard- und intelligente Neupreisregeln. **[!UICONTROL Match Competitor Price]** ist nur verfügbar unter _[!UICONTROL Price Action]_when **[!UICONTROL Rule Type]**auf `Intelligent repricing rule`.

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- [Regeltyp auswählen](./intelligent-repricing-rules.md)
- [Bedingte Unterschiede zwischen Wettbewerbern](./competitor-conditional-variances.md)
- Preisanpassung
- [Floor Price](./floor-price.md)
- [Optionaler Höchstpreis](./optional-ceiling-price.md)

Die Preisanpassung definiert die Preisberechnung, wenn Sie die Preisquelle des Konkurrenten ermittelt haben.

## Preisanpassung konfigurieren

Definieren Sie Ihre Preisanpassung im _[!UICONTROL Price Adjustment]_Abschnitt.

1. Für **[!UICONTROL Price Action]**, wählen Sie eine Option aus:

   - `Decrease By` - Wählen Sie aus, wann der definierte Preis-Quellwert angepasst werden soll, um einen niedrigeren Preis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.

   - `Increase By` - Wählen Sie aus, wann der definierte Preisquellenwert angepasst werden soll, um einen höheren Preis für die Regel zu erzielen, bevor Sie sie in Amazon auflisten.

   - `Match Competitor Price` - (Nur intelligente Neupreisregel) Wählen Sie aus, wann Sie Ihren Amazon-Listingpreis so ändern möchten, dass er mit dem [kleinster Konkurrent](./lowest-competitor-pricing.md) Preis, basierend auf Ihrem Feedback und Varianzparametern Ihrer Konkurrenten. Wenn auf `Match Competitor Price`, die _[!UICONTROL Apply]_und_[!UICONTROL Adjustment Amount]_ -Felder entfernt werden.

1. Für **[!UICONTROL Apply]**, wählen Sie eine Option aus:

   - `Apply as percentage` - Legen Sie fest, wann die Definition erfolgen soll **[!UICONTROL Magento Price Source]** definiert in [Listenpreis](./listing-price.md) um einen Prozentsatz bereinigt.

   - `Apply as fixed amount` - Legen Sie fest, wann die Definition erfolgen soll **[!UICONTROL Magento Price Source]** definiert in [Listenpreis](./listing-price.md) angepasst um einen festen Betrag.

1. Für **[!UICONTROL Adjustment Amount]** (erforderlich), geben Sie den numerischen Wert für die Preisanpassung an.

   - Wann **[!UICONTROL Apply]** auf `Apply as percentage`, geben Sie den Prozentwert ein (Beispiel: enter `25` 25 %).

   - Wann **[!UICONTROL Apply]** auf `Apply as fixed amount`Geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: enter `25` für eine feste Anpassung in Höhe von 25 USD).

![Intelligente Neupreisregelung - Preisanpassung](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | Wählen Sie eine Preisanpassungsaktion. Optionen:<br>**[!UICONTROL Decrease By]**- Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Magento Price Source]_definiert in [Listenpreis](./listing-price.md) , um einen niedrigeren Preis für die Regel zu erzielen, bevor sie in Amazon aufgenommen wird.<br>**[!UICONTROL Increase By]**- Legen Sie fest, wann die Definition erfolgen soll_[!UICONTROL Magento Price Source]_ definiert in [Listenpreis](./listing-price.md) , um einen höheren Preis für die Regel zu erzielen, bevor sie in Amazon aufgenommen wird.<br>**[!UICONTROL Match Competitor Price]**- (Nur intelligente Neupreisregel) Wählen Sie aus, wann Sie Ihren Amazon-Listingpreis so ändern möchten, dass er mit dem [kleinster Konkurrent](./lowest-competitor-pricing.md) Preis, basierend auf Ihrem Feedback und Varianzparametern Ihrer Konkurrenten. Wenn ausgewählt, wird die _Anwenden_ und _Anpassungsbetrag_ -Felder entfernt werden. |
| [!UICONTROL Apply] | Optionen:<br>**[!UICONTROL Apply as percentage]**- Legen Sie fest, wann die Definition erfolgen soll _[!UICONTROL Magento Price Source]_definiert in [Listenpreis](./listing-price.md) um einen Prozentsatz bereinigt.<br>**[!UICONTROL Apply as fixed amount]**- Legen Sie fest, wann die Definition erfolgen soll_[!UICONTROL Magento Price Source]_ definiert in [Listenpreis](./listing-price.md) angepasst um einen festen Betrag. |
| [!UICONTROL Adjustment Amount] | Erforderlich.<br>Wenn Sie `Apply as percentage` für **[!UICONTROL Apply]**, geben Sie den Prozentwert ein (Beispiel: enter `25` 25 %).<br>Wenn Sie `Apply as fixed amount` für **[!UICONTROL Apply]** Geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: enter `25` für eine feste Anpassung in Höhe von 25 USD). |
