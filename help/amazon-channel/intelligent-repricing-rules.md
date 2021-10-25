---
title: '"Intelligente Preisanpassungsregel: Regeltyp auswählen'''
description: Ermitteln Sie Ihren Listenpreis für Amazon anhand des Konkurrent-Preises und schaffen Sie eine intelligente Preisanpassungsregel.
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Intelligente Preisanpassungsregel: Regeltyp auswählen

>[!IMPORTANT]
>
>Intelligente Preisanpassungsregeln funktionieren nicht ordnungsgemäß, wenn die Amazon-Region auf `Inactive` Status, wie es während des Einbodens ist. Ihre Preisberechnungen hängen von Ihren Versandkosten ab. Ihre Region muss sich in `Active` Status für Ihre Versandtarife, die von Amazon aus synchronisiert werden sollen.<br><br>
>
>Um den Regionsstatus in Ihrem Amazon-Konto zu aktualisieren, navigieren Sie zu Einstellungen > Kontoinformationen > Urlaubseinstellungen. Siehe [Amazon: Listungsstatus für Urlaube](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

Eine intelligente Neupreisregel verwendet die Preise der Amazon Konkurrent, um Ihren Börsenpreis zu bestimmen. Konkurrent sind andere Verkäufer, die die gleichen Produkte wie Ihre auf Amazon Liste.

Zu den Abschnitten einer intelligenten Neubewertungsregel gehören:

- Regeltyp auswählen
- [Bedingte Abweichungen des Konkurrenten](./competitor-conditional-variances.md)
- [Preisanpassung](./price-adjustment.md)
- [Floor-Preis](./floor-price.md)
- [Optionaler Höchstpreis](./optional-ceiling-price.md)

## Regeltyp konfigurieren

Regeltyp definieren im _[!UICONTROL Select Rule Type]_Abschnitt.

1. für **[!UICONTROL Rule Type]**, wählen `Intelligent repricing rule`.

   Diese Einstellung aktiviert die _[!UICONTROL Competitor Price Source]_und [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md)und [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) Abschnitte.

1. für **[!UICONTROL Competitor Price Source]**, wählen Sie eine Option aus:

   - **[!UICONTROL Use "Buy Box" Price]** - Legen Sie fest, wann Sie die Amazon-Preise auf der Grundlage des Amazon anpassen möchten [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Verkaufspreis. A [!DNL Buy Box] Der Preis ist vorhanden, wenn mehrere Verkäufer auf Amazon Angebot dasselbe Produkt. Amazon definiert [!DNL Buy Box] Verkäufer auf der Grundlage von Leistungsanforderungen. Händler versuchen, die [!DNL Buy Box] Vertriebsstatus und Angebot maximale Sichtbarkeit ihrer Produktauflistungen.

   - **[!UICONTROL Use Lowest Competitor Price]** - Wählen Sie aus, wann Sie den Listenpreis mit dem Konkurrent-Preis für dasselbe Produkt vergleichen und anpassen möchten. Bei Auswahl der _[!UICONTROL Minimum Positive Feedback]_und_[!UICONTROL Minimum Feedback Count]_ Felder sind aktiviert.

1. Wenn aktiviert, wählen Sie eine Option für **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - Wählen Sie aus, wann Sie Ihre Preise auf der Grundlage aller Konkurrent für ein und dasselbe Produkt vergleichen und anpassen möchten.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Wählen Sie aus, wann Sie die Konkurrent begrenzen möchten, mit denen der Preis für dasselbe Produkt verglichen wird. Durch diese Einstellung werden die Konkurrent weiter eingeschränkt, da sie in ihrer Auflistung vor Anwendung der niedrigsten Preisregel einen Mindestprozentsatz an positivem Feedback angeben müssen.

1. Wenn aktiviert, geben Sie einen numerischen Wert ein für **[!UICONTROL Minimum Feedback Count]**.

   Dieser optionale numerische Wert senkt die Wettbewerbspreise weiter. Wenn ein Händler beispielsweise eine positive Rückmeldung von 95 % hat, aber nur eine Rückmeldung von `20`, ist es möglicherweise kein Konkurrent, an dem Sie Ihre Preise ändern möchten. Wenn Sie jedoch einen Wert von `1000`, würde es erforderlich sein, dass der Händler 95 % positive Rückmeldungen und mindestens 1000 Handelsüberprüfungen erhält.

>[!NOTE]
>
>Sie können diese Konkurrent-Preise und Feedback-Optionen verwenden, um Ihre Preisgestaltung nicht auf einen Konkurrent zu stützen, der über schlechtes Feedback verfügt und ein Produkt von geringerer Qualität verkauft.

![Intelligente Neupreisregel - Regeltyp auswählen](assets/ob-intelligent-price-rule-type.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Rule Type] | Wählen Sie einen Regeltyp aus. Optionen:<ul><li>**[!UICONTROL Standard price rule]** - Dieser Regeltyp ermöglicht es Ihnen, den Amazon-Börsennotierungspreis um einen bestimmten Prozentsatz oder festen Dollarbetrag im Verhältnis zum _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - Dieser Regeltyp ermöglicht es Ihnen, Ihren Amazon-Listingpreis auf Basis der Preise des Konkurrenten anzupassen. Bei Auswahl der _[!UICONTROL Minimum Positive Feedback]_und_[!UICONTROL Minimum Feedback Count]_ Felder sind aktiviert.</li></ul> |
| [!UICONTROL Competitor Price Source] | Wählen Sie die gewünschte Preisquelle aus. Optionen:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Wählen Sie diese Option, wenn Sie die Amazon-Preise auf Basis des Amazon anpassen möchten [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Verkaufspreis. A [!DNL Buy Box] Der Preis ist vorhanden, wenn mehrere Verkäufer auf Amazon Angebot dasselbe Produkt. Amazon definiert [!DNL Buy Box] Verkäufer auf der Grundlage von Leistungsanforderungen. Händler versuchen, die [!DNL Buy Box] Vertriebsstatus und Angebot maximale Sichtbarkeit ihrer Produktauflistungen.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - Wählen Sie diese Option, wenn Sie Ihren Listenpreis vergleichen und anpassen möchten auf [niedrigste Konkurrent-Preise](./lowest-competitor-pricing.md) für dasselbe Produkt. Bei Auswahl der _[!UICONTROL Minimum Positive Feedback]_und_[!UICONTROL Minimum Feedback Count]_ Felder sind aktiviert.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | Nur aktiv, wenn `Use Lowest Competitor Price` ausgewählt. Optionen:<ul><li>**[!UICONTROL All Competitor's Prices]** - Wählen Sie aus, wann Sie Ihre Preise auf der Grundlage aller Konkurrent für ein und dasselbe Produkt vergleichen und anpassen möchten.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Wählen Sie aus, wann Sie die Konkurrent, mit denen Sie vergleichen, begrenzen und die Preise anpassen möchten. Mit dieser Einstellung werden Ihre Konkurrent weiter eingeschränkt, da in der Liste ein Mindestprozentsatz an positivem Feedback angegeben werden muss und dann der niedrigste Preis für diese Teilmenge von Konkurrenten verwendet wird.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | Nur aktiv, wenn `Use Lowest Competitor Price` ausgewählt. Dieser optionale numerische Wert verringert den Preisvergleich weiter. Wenn ein Händler beispielsweise eine positive Rückmeldung von 95 % hat, aber nur eine Rückmeldung von `20`, ist es möglicherweise kein Konkurrent, an dem Sie Ihre Preise ändern möchten. Wenn Sie jedoch einen Wert von `1000`, würde es erforderlich sein, dass der Händler 95 % positive Rückmeldungen und mindestens 1000 Handelsüberprüfungen erhält. |
