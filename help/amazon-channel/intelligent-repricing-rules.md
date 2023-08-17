---
title: "Intelligente Neupreisregel: Regeltyp auswählen"
description: Bestimmen Sie anhand einer intelligenten Neupreisregel den Listenpreis für Amazon anhand der Preise für Wettbewerber.
feature: Sales Channels, Products, Price Rules
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Intelligente Neupreisregel: Regeltyp auswählen

>[!IMPORTANT]
>
>Intelligente Regeln für die Neuberechnung funktionieren nicht ordnungsgemäß, wenn der Amazon-Bereich auf `Inactive` -Status, wie es beim Onboarding der Fall ist. Ihre Preisberechnungen hängen von Ihren Versandkosten ab und Ihre Region muss sich in `Active` Status für Ihre Versandraten, die von Amazon synchronisiert werden.<br><br>
>
>Um den Status Ihrer Region in Ihrem Amazon-Konto zu aktualisieren, gehen Sie zu Einstellungen > Kontoinformationen > Urlaubseinstellungen. Siehe Abschnitt [Amazon: Auflistungsstatus für Urlaub](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

Eine intelligente Neupreisregel nutzt die Preise von Amazon-Konkurrenten, um Ihren Börsennotierungspreis zu bestimmen. Wettbewerber sind andere Verkäufer, die dieselben Produkte wie Ihre in Amazon auflisten.

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- Regeltyp auswählen
- [Bedingte Unterschiede zwischen Wettbewerbern](./competitor-conditional-variances.md)
- [Preisanpassung](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- [Optionaler Höchstpreis](./optional-ceiling-price.md)

## Regeltyp konfigurieren

Definieren Sie den Regeltyp im _[!UICONTROL Select Rule Type]_Abschnitt.

1. Für **[!UICONTROL Rule Type]** auswählen `Intelligent repricing rule`.

   Diese Einstellung ermöglicht die _[!UICONTROL Competitor Price Source]_und [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md), und [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) Abschnitte.

1. Für **[!UICONTROL Competitor Price Source]** eine Option auswählen:

   - **[!UICONTROL Use "Buy Box" Price]** - Legen Sie fest, wann Sie Ihre Amazon-Preise auf der Grundlage der Amazon anpassen möchten [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Verkaufspreis. A [!DNL Buy Box] Der Preis ist vorhanden, wenn mehrere Verkäufer in Amazon dasselbe Produkt anbieten. Amazon definiert die [!DNL Buy Box] Verkäufer auf der Grundlage von Leistungsanforderungen. Händler versuchen, die [!DNL Buy Box] Verkaufsstatus und maximale Sichtbarkeit der Produktlisten.

   - **[!UICONTROL Use Lowest Competitor Price]** - Wählen Sie aus, wann Sie Ihren Listenpreis vergleichen und an die Preise von Konkurrenten für dasselbe Produkt anpassen möchten. Wenn ausgewählt, wird die _[!UICONTROL Minimum Positive Feedback]_und_[!UICONTROL Minimum Feedback Count]_ -Felder aktiviert sind.

1. Wählen Sie, falls aktiviert, eine Option für **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - Entscheiden Sie, wann Sie Ihre Preise auf der Grundlage aller Preise von Konkurrenten für dasselbe Produkt vergleichen und anpassen möchten.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Wählen Sie aus, wann Sie die Konkurrenten einschränken möchten, mit denen der Preis für dasselbe Produkt verglichen wird. Diese Einstellung schränkt die Konkurrenten weiter ein, indem sie von ihrer Auflistung verlangen, dass sie mindestens über den gewählten Prozentsatz an positivem Feedback verfügen, bevor sie die Regel des niedrigsten Preises anwenden.

1. Geben Sie bei Aktivierung einen numerischen Wert für **[!UICONTROL Minimum Feedback Count]**.

   Dieser optionale numerische Wert schränkt die Wettbewerbspreise weiter ein. Wenn beispielsweise ein Händler eine positive Feedback-Bewertung von 95 % hat, aber nur eine Feedback-Anzahl von `20`ist es möglicherweise kein Konkurrent, an dem Sie Ihre Preise ändern möchten. Wenn Sie jedoch den Wert `1000`würde es erforderlich sein, dass der Händler 95 % positives Feedback und mindestens 1000 Handelsüberprüfungen erhält.

>[!NOTE]
>
>Sie können diese Preisgestaltung und Feedback-Optionen von Konkurrenten verwenden, um zu vermeiden, dass Sie Ihre Preise auf einen Konkurrenten stützen, der über schlechtes Feedback verfügt und ein Produkt mit geringerer Qualität verkauft.

![Intelligente Neupreisregel - Regeltyp auswählen](assets/ob-intelligent-price-rule-type.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | Wählen Sie einen Regeltyp aus. Optionen:<ul><li>**[!UICONTROL Standard price rule]** - Mit diesem Regeltyp können Sie den Amazon-Listingpreis um einen bestimmten Prozentwert oder festen Dollarbetrag im Verhältnis zum _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - Mit diesem Regeltyp können Sie Ihren Listenpreis für Amazon auf der Grundlage der Preise des Konkurrenten anpassen. Wenn ausgewählt, wird die _[!UICONTROL Minimum Positive Feedback]_und_[!UICONTROL Minimum Feedback Count]_ -Felder aktiviert sind.</li></ul> |
| [!UICONTROL Competitor Price Source] | Wählen Sie die gewünschte Preisquelle aus. Optionen:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Wählen Sie diese Option, wenn Sie Ihre Amazon-Preise auf der Grundlage der Amazon anpassen möchten. [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Verkaufspreis. A [!DNL Buy Box] Der Preis ist vorhanden, wenn mehrere Verkäufer in Amazon dasselbe Produkt anbieten. Amazon definiert die [!DNL Buy Box] Verkäufer auf der Grundlage von Leistungsanforderungen. Händler versuchen, die [!DNL Buy Box] Verkaufsstatus und maximale Sichtbarkeit der Produktlisten.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - Wählen Sie diese Option aus, wenn Sie Ihren Listenpreis vergleichen und an die [niedrigste Preise für Wettbewerber](./lowest-competitor-pricing.md) für dasselbe Produkt. Wenn ausgewählt, wird die _[!UICONTROL Minimum Positive Feedback]_und_[!UICONTROL Minimum Feedback Count]_ -Felder aktiviert sind.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | Nur aktiv, wenn `Use Lowest Competitor Price` ausgewählt ist. Optionen:<ul><li>**[!UICONTROL All Competitor's Prices]** - Entscheiden Sie, wann Sie Ihre Preise auf der Grundlage aller Preise von Konkurrenten für dasselbe Produkt vergleichen und anpassen möchten.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Wählen Sie aus, wann Sie die Konkurrenten einschränken möchten, mit denen Sie Ihre Preise vergleichen, und passen Sie sie an. Diese Einstellung schränkt Ihre Konkurrenten weiter ein, indem sie von ihrer Auflistung verlangen, dass sie mindestens über den ausgewählten Prozentsatz an positivem Feedback verfügen und dann den niedrigsten Preis dieser Untergruppe von Wettbewerbern verwenden.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | Nur aktiv, wenn `Use Lowest Competitor Price` ausgewählt ist. Dieser optionale numerische Wert schränkt den Vergleich der Wettbewerbspreise weiter ein. Wenn beispielsweise ein Händler eine positive Feedback-Bewertung von 95 % hat, aber nur eine Feedback-Zählung von `20`ist es möglicherweise kein Konkurrent, an dem Sie Ihre Preise ändern möchten. Wenn Sie jedoch den Wert `1000`würde es erforderlich sein, dass der Händler 95 % positives Feedback und mindestens 1000 Handelsüberprüfungen erhält. |
