---
title: Amazon-Vertriebskanal - Aktionen im Rahmen von Standardpreisregeln
description: Verwenden Sie Aktionen, die mit Standardpreisregeln durchgeführt werden, um einen Amazon-Listingpreis im Verhältnis zum Commerce-Katalogpreis (oder zur Preisquelle) zu erhöhen oder zu senken.
feature: Sales Channels, Price Rules
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '340'
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

1. Erweitern Sie bei Bedarf den Abschnitt &quot;_[!UICONTROL Price Adjustment]_&quot;.

1. Wählen Sie für **[!UICONTROL Price Action]** eine Option, um festzulegen, wie Sie den (in Ihrem [Listing Price](./listing-price.md) -Wert definierten) *[!UICONTROL Magento Price Source]* ändern möchten.

   - `Decrease By` - Legen Sie fest, wann der Wert reduziert werden soll, bevor Sie ihn in Amazon auflisten.

   - `Increase By` - Legen Sie fest, wann der Wert erhöht werden soll, bevor Sie Amazon auflisten.

1. Wählen Sie für **[!UICONTROL Apply]** eine Option aus, um zu bestimmen, wie der definierte *[!UICONTROL Magento Price Source]*, der im [Listenpreis](./listing-price.md) -Wert definiert ist, angepasst werden soll:

   - `Apply as percentage` - Legen Sie fest, wann der definierte *[!UICONTROL Magento Price Source]* in Ihrem [Listing Price](./listing-price.md) -Wert um einen Prozentsatz angepasst werden soll

   - `Apply as fixed amount` - Wählen Sie aus, wann der definierte *[!UICONTROL Magento Price Source]*-Wert in Ihrem [Listing Price](./listing-price.md)-Wert um einen festen Betrag angepasst werden soll.

1. Geben Sie für &quot;**[!UICONTROL Adjustment Amount]**&quot;(erforderlich) den numerischen Wert für die Preisanpassung ein.

   - Wenn *[!UICONTROL Apply]* auf `Apply as percentage` gesetzt ist, geben Sie den Prozentwert ein (Beispiel: geben Sie `25` für eine Preisanpassung von 25 % ein).

   - Wenn *[!UICONTROL Apply]* auf `Apply as fixed amount` gesetzt ist, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: geben Sie `25` für eine Anpassung des Festpreises um 25 USD ein).

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save pricing rule]**.

![Standardpreisregel](assets/ob-price-rule-action-standard-example.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|--------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | Wählen Sie `Standard price rule` aus. |
| [!UICONTROL Price Action] | Optionen:<ul><li>**[!UICONTROL Decrease By]** - Legen Sie fest, wann der definierte [!DNL Commerce] Preisquellenwert reduziert werden soll, bevor er in Amazon aufgelistet wird.</li><li>**[!UICONTROL Increase By]** - Legen Sie fest, wann der definierte [!DNL Commerce] Preisquellenwert erhöht werden soll, bevor Sie Amazon auflisten.</li></ul> |
| [!UICONTROL Apply] | Optionen:<ul><li>**[!UICONTROL Apply as percentage]** - Wählen Sie aus, wann der definierte [!DNL Commerce] Preisquellenwert um einen Prozentsatz angepasst werden soll.</li><li>**[!UICONTROL Apply as fixed amount]** - Wählen Sie aus, wann der definierte [!DNL Commerce] Preisquellenwert um einen festen Betrag angepasst werden soll.</li></ul> |
| [!UICONTROL Adjustment Amount] | Erforderlich.<br><br>Wenn Sie `Apply as percentage` für *[!UICONTROL Apply]* auswählen, geben Sie den Prozentwert ein (Beispiel: geben Sie `25` für eine 25%-ige Einstellung ein).<br><br>Wenn Sie `Apply as fixed amount` für *[!UICONTROL Apply]* auswählen, geben Sie den numerischen Wert für den Festbetrag ein (Beispiel: Geben Sie `25` für eine feste Anpassung von 25 USD ein). |
