---
title: Standardmäßige Preisregelaktionen
description: Verwenden Sie standardmäßige Preisregelaktionen, um einen Börsennotierungspreis der Amazon im Verhältnis zum Commerce-Katalogpreis (oder der Preisquelle) zu erhöhen oder zu senken.
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Standardpreisregelaktionen

Mit einer standardmäßigen Preisregel-Aktion können Sie einen Amazon-Börsennotierungspreis um einen bestimmten Prozentsatz oder festen Dollarbetrag im Verhältnis zum [!DNL Commerce] Katalogpreis (oder Preisquelle).

Zu den Abschnitten einer standardmäßigen Preisregelaktion gehören:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Preisregelaktionen konfigurieren

1. für **[!UICONTROL Rule Type]**, wählen `Standard price rule`.

   Mit dieser Option werden die anderen Felder in der _[!UICONTROL Select Rule Type]_Abschnitt.

1. Erweitern der _[!UICONTROL Price Adjustment]_Abschnitt, falls erforderlich.

1. für **[!UICONTROL Price Action]**, wählen Sie eine Option, um zu bestimmen, wie Sie die Änderung *[!UICONTROL Magento Price Source]* (definiert in [Listingpreis](./listing-price.md)).

   - `Decrease By` - Wählen Sie aus, wann der Wert vor dem Auflisten auf Amazon reduziert werden soll.

   - `Increase By` - Wählen Sie aus, wann der Wert erhöht werden soll, bevor Sie Amazon auflisten.

1. für **[!UICONTROL Apply]**, wählen Sie eine Option und eine Option, um zu bestimmen, wie Sie die Definition *[!UICONTROL Magento Price Source]* definiert in [Listingpreis](./listing-price.md) anzupassender Wert:

   - `Apply as percentage` - Wählen Sie aus, wann die *[!UICONTROL Magento Price Source]* definiert in [Listingpreis](./listing-price.md) um einen Prozentsatz bereinigter Wert

   - `Apply as fixed amount` - Wählen Sie aus, wann die *[!UICONTROL Magento Price Source]* definiert in [Listingpreis](./listing-price.md) um einen festen Betrag bereinigt.

1. für **[!UICONTROL Adjustment Amount]** (erforderlich), geben Sie den numerischen Wert für die Preisanpassung ein.

   - Wann *[!UICONTROL Apply]* ist eingestellt auf `Apply as percentage`, geben Sie den Prozentwert ein (Beispiel: Eingabe `25` für eine Preisanpassung von 25 %).

   - Wann *[!UICONTROL Apply]* ist eingestellt auf `Apply as fixed amount`, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: Eingabe `25` für eine Preisanpassung von 25 Dollar).

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save pricing rule]**.

![Standardpreisregel](assets/ob-price-rule-action-standard-example.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Rule Type] | Auswählen `Standard price rule`. |
| [!UICONTROL Price Action] | Optionen:<ul><li>**[!UICONTROL Decrease By]** - Wählen Sie aus, wann die [!DNL Commerce] Wert der Kursquelle, der vor der Aufnahme in Amazon herabgesetzt werden muss.</li><li>**[!UICONTROL Increase By]** - Wählen Sie aus, wann die [!DNL Commerce] vor der Aufnahme in Amazon zu erhöhen.</li></ul> |
| [!UICONTROL Apply] | Optionen:<ul><li>**[!UICONTROL Apply as percentage]** - Wählen Sie aus, wann die [!DNL Commerce] um einen Prozentsatz bereinigter Preis-Quellenwert.</li><li>**[!UICONTROL Apply as fixed amount]** - Wählen Sie aus, wann die [!DNL Commerce] Preisquellenwert um einen festen Betrag berichtigt.</li></ul> |
| [!UICONTROL Adjustment Amount] | Erforderlich.<br><br>Wählen Sie `Apply as percentage` für *[!UICONTROL Apply]*, geben Sie den Prozentwert ein (Beispiel: Eingabe `25` 25 % Anpassung).<br><br>Wenn Sie möchten `Apply as fixed amount` für *[!UICONTROL Apply]*, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: Eingabe `25` für eine feste Anpassung um 25 Dollar). |
