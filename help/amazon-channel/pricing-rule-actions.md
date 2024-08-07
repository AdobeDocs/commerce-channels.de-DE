---
title: Amazon-Vertriebskanal - Aktionen für Preisregeln
description: Verwenden Sie die Preisregelaktionen, um die auf die Preisquelle angewendeten Anpassungsberechnungen zur Bestimmung des Amazon-Börsennotierungspreises zu definieren.
feature: Sales Channels, Price Rules
exl-id: c46bd5c2-7994-45b4-ae0c-9e473372c73a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Aktionen für Preisregeln

Preisregelaktionen definieren die Anpassungsberechnungen, die auf die Preisquelle angewendet werden, um den Börsennotierungspreis zu bestimmen.

## Standardpreisregel

Eine [Standardpreisregel](./standard-price-rules.md) ermöglicht es Ihnen, einen Amazon-Börsennotierungspreis um einen bestimmten Prozentwert oder festen Dollarbetrag im Verhältnis zum [!DNL Commerce] -Katalogpreis (oder zur Preisquelle) zu erhöhen oder zu senken.

| Abschnitt | Beschreibung |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Select Rule Type]](./standard-price-rules.md) | Legen Sie den Regeltyp auf `Standard price rule` fest. |
| [[!UICONTROL Price Adjustment]](./standard-price-rules.md) | Definieren Sie die auf die Preisquelle angewendeten Anpassungsberechnungen zur Bestimmung des Börsenkurses. |

## Intelligente Neupreisregel

Eine [intelligente Neupreisregel](./intelligent-repricing-rules.md) verwendet die Preise von Amazon-Konkurrenten, um Ihren Listenpreis zu bestimmen. Wettbewerber sind andere Verkäufer, die dieselben Produkte auflisten, die Sie in Amazon auflisten.

| Abschnitt | Beschreibung |
|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md) | Legen Sie den Regeltyp zusammen mit Ihren Anforderungen an Konkurrentenpreise, Source und Feedback auf `Intelligent repricing rule` fest. |
| [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md) | Definieren Sie Abweichungen für Bedingungen des gleichen Produkts, das von Wettbewerbern verkauft wird. |
| [[!UICONTROL Price Adjustment]](./price-adjustment.md) | Definieren Sie die auf die Preisquelle angewendeten Anpassungsberechnungen zur Bestimmung des Börsenkurses. |
| [[!UICONTROL Floor Price]](./floor-price.md) | Definieren Sie den niedrigsten Preis für ein Produkt, um zu verhindern, dass durch mehrere Preisregeln ein Listentarif zu niedrig festgelegt wird. |
| [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md) | Definieren Sie Ihren höchsten Preis für ein Produkt, um sicherzustellen, dass Ihre Preise wettbewerbsfähig bleiben. |
