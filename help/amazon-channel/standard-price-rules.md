---
title: Standardmäßige Preisregelaktionen
description: Verwenden Sie Aktionen, die mit Standardpreisregeln durchgeführt werden, um einen Amazon-Listingpreis im Verhältnis zum Commerce-Katalogpreis (oder zur Preisquelle) zu erhöhen oder zu senken.
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Standardmäßige Preisregelaktionen

Mit einer standardmäßigen Preisregel-Aktion können Sie einen Amazon-Börsennotierungspreis um einen bestimmten Prozentwert oder festen Dollarbetrag im Verhältnis zum [!DNL Commerce] -Katalogpreis (oder zur Preisquelle) erhöhen oder verringern.

Zu den Abschnitten einer Standardaktion für Preisregeln gehören:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Aktionen für Preisregeln konfigurieren

1. Wählen Sie für **[!UICONTROL Rule Type]** `Standard price rule` aus.

   Diese Option deaktiviert die anderen Felder im Abschnitt _[!UICONTROL Select Rule Type]_.

1. Erweitern Sie bei Bedarf den Abschnitt _[!UICONTROL Price Adjustment]_.

1. Wählen Sie für **[!UICONTROL Price Action]** eine Option, um festzulegen, wie Sie den *[!UICONTROL Magento Price Source]* (definiert in Ihrem [Listing Price](./listing-price.md))-Wert ändern möchten.

   - `Decrease By` - Legen Sie fest, wann der Wert reduziert werden soll, bevor Sie ihn in Amazon auflisten.

   - `Increase By` - Wählen Sie aus, wann der Wert erhöht werden soll, bevor Sie Amazon auflisten.

1. Wählen Sie für **[!UICONTROL Apply]** eine Option und legen Sie fest, wie der definierte *[!UICONTROL Magento Price Source]*-Wert, der in Ihrem [Listenpreis](./listing-price.md) definiert ist, angepasst werden soll:

   - `Apply as percentage` - Wählen Sie aus, wann der in Ihrem  *[!UICONTROL Magento Price Source]* Listing- [ ](./listing-price.md) Preiswert definierte Wert um einen Prozentsatz angepasst werden soll.

   - `Apply as fixed amount` - Wählen Sie aus, wann der in Ihrem  *[!UICONTROL Magento Price Source]* Listing- [ ](./listing-price.md) Preis definierte Wert um einen festen Betrag angepasst werden soll.

1. Geben Sie für **[!UICONTROL Adjustment Amount]** (erforderlich) den numerischen Wert für die Preisanpassung ein.

   - Wenn *[!UICONTROL Apply]* auf `Apply as percentage` gesetzt ist, geben Sie den Prozentwert ein (Beispiel: `25` für eine Preisanpassung von 25 % eingeben).

   - Wenn *[!UICONTROL Apply]* auf `Apply as fixed amount` gesetzt ist, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: `25` für eine Anpassung des Festpreises von 25 USD eingeben).

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save pricing rule]**.

![Standardpreisregel](assets/ob-price-rule-action-standard-example.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Rule Type] | Wählen Sie `Standard price rule` aus. |
| [!UICONTROL Price Action] | Optionen:<ul><li>**[!UICONTROL Decrease By]** - Wählen Sie aus, wann der definierte  [!DNL Commerce] Preisquellenwert vor der Auflistung mit Amazon reduziert werden soll.</li><li>**[!UICONTROL Increase By]** - Wählen Sie aus, wann der definierte  [!DNL Commerce] Preisquellenwert erhöht werden soll, bevor Sie Amazon auflisten.</li></ul> |
| [!UICONTROL Apply] | Optionen:<ul><li>**[!UICONTROL Apply as percentage]** - Wählen Sie aus, wann der definierte  [!DNL Commerce] Preisquellwert um einen Prozentwert angepasst werden soll.</li><li>**[!UICONTROL Apply as fixed amount]** - Wählen Sie aus, wann der definierte  [!DNL Commerce] Preisquellenwert um einen festen Betrag angepasst werden soll.</li></ul> |
| [!UICONTROL Adjustment Amount] | Erforderlich.<br><br>Wenn Sie  `Apply as percentage` für  *[!UICONTROL Apply]* wählen, geben Sie den Prozentwert ein (Beispiel: 25 %  `25` für eine Anpassung).<br><br>Wenn Sie  `Apply as fixed amount` für  *[!UICONTROL Apply]* wählen, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: für  `25` eine feste Anpassung von 25 USD). |
