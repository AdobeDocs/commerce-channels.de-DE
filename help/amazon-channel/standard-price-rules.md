---
title: Standardmäßige Preisregelaktionen
description: Verwenden Sie standardmäßige Preisregelaktionen, um einen Amazon-Listingpreis im Verhältnis zum Commerce-Katalogpreis (oder zur Preisquelle) zu erhöhen oder zu senken.
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Standardmäßige Preisregelaktionen

Mit einer standardmäßigen Preisregel-Aktion können Sie einen Amazon-Listingpreis um einen bestimmten Prozentwert oder festen Dollarbetrag im Verhältnis zum [!DNL Commerce] Katalogpreis (oder Preisquelle).

Zu den Abschnitten einer Standardaktion für Preisregeln gehören:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Aktionen für Preisregeln konfigurieren

1. Für **[!UICONTROL Rule Type]** auswählen `Standard price rule`.

   Diese Option deaktiviert die anderen Felder im _[!UICONTROL Select Rule Type]_Abschnitt.

1. Erweitern Sie die _[!UICONTROL Price Adjustment]_bei Bedarf.

1. Für **[!UICONTROL Price Action]**, wählen Sie eine Option, um festzulegen, wie Sie die *[!UICONTROL Magento Price Source]* (definiert in [Listenpreis](./listing-price.md)).

   - `Decrease By` - Legen Sie fest, wann der Wert reduziert werden soll, bevor Sie ihn in Amazon auflisten.

   - `Increase By` - Wählen Sie aus, wann der Wert erhöht werden soll, bevor Sie Amazon auflisten.

1. Für **[!UICONTROL Apply]**, wählen Sie eine Option und eine Option, um festzulegen, wie Sie die Definition *[!UICONTROL Magento Price Source]* definiert in [Listenpreis](./listing-price.md) Wert, der angepasst werden soll:

   - `Apply as percentage` - Legen Sie fest, wann die Definition erfolgen soll *[!UICONTROL Magento Price Source]* definiert in [Listenpreis](./listing-price.md) um einen Prozentsatz berichtigter Wert

   - `Apply as fixed amount` - Legen Sie fest, wann die Definition erfolgen soll *[!UICONTROL Magento Price Source]* definiert in [Listenpreis](./listing-price.md) um einen Festbetrag berichtigten Wert.

1. Für **[!UICONTROL Adjustment Amount]** (erforderlich), geben Sie den numerischen Wert für die Preisanpassung an.

   - Wann *[!UICONTROL Apply]* auf `Apply as percentage`, geben Sie den Prozentwert ein (Beispiel: enter `25` 25 % Preisanpassung).

   - Wann *[!UICONTROL Apply]* auf `Apply as fixed amount`Geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: enter `25` für eine Preisanpassung in Höhe von 25 USD).

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save pricing rule]**.

![Standardpreisregel](assets/ob-price-rule-action-standard-example.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Rule Type] | Auswählen `Standard price rule`. |
| [!UICONTROL Price Action] | Optionen:<ul><li>**[!UICONTROL Decrease By]** - Legen Sie fest, wann die Definition erfolgen soll [!DNL Commerce] Preisquellenwert vor der Aufnahme in Amazon zu reduzieren.</li><li>**[!UICONTROL Increase By]** - Legen Sie fest, wann die Definition erfolgen soll [!DNL Commerce] Preisquellenwert, der vor der Auflistung in Amazon erhöht werden soll.</li></ul> |
| [!UICONTROL Apply] | Optionen:<ul><li>**[!UICONTROL Apply as percentage]** - Legen Sie fest, wann die Definition erfolgen soll [!DNL Commerce] Preisquellenwert, um einen Prozentsatz berichtigt.</li><li>**[!UICONTROL Apply as fixed amount]** - Legen Sie fest, wann die Definition erfolgen soll [!DNL Commerce] Preisquellenwert, berichtigt um einen festen Betrag.</li></ul> |
| [!UICONTROL Adjustment Amount] | Erforderlich.<br><br>Wenn Sie `Apply as percentage` für *[!UICONTROL Apply]*, geben Sie den Prozentwert ein (Beispiel: enter `25` 25 %).<br><br>Wenn Sie `Apply as fixed amount` für *[!UICONTROL Apply]* Geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: enter `25` für eine feste Anpassung in Höhe von 25 USD). |
