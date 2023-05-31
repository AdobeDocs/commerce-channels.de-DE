---
title: Amazon-Vertriebskanal - Allgemeine Preisregeleinstellungen
description: Verwenden Sie die allgemeinen Preisregeleinstellungen, um die Hauptmerkmale einer Regel für den Börsennotierungspreis zu definieren.
exl-id: 915b3eed-997e-4f94-a23f-0553a9dfe30c
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Allgemeine Preisregeleinstellungen

Definieren Sie den Namen, die Beschreibung, das aktive Datum und die Priorität für die Regel.

## Füllen Sie den Abschnitt Allgemeine Preisregeln aus.

1. Für **[!UICONTROL Rule Name]** (erforderlich), geben Sie den Namen für die Regel ein.

   Dieser Name dient nur Ihrer internen Identifizierung. Je beschreibender der Regelname ist, desto besser.

1. Für **[!UICONTROL Description]** Geben Sie eine detaillierte Beschreibung Ihrer Regel ein.

   Diese Beschreibung kann Informationen zu den qualifizierenden Produkten, den aktiven Daten, der Formel zur Berechnung Ihres angepassten Preises oder andere Informationen enthalten, die Sie für nützlich halten, wenn Sie die Regel ändern möchten.

1. Für **[!UICONTROL Status]**, wählen Sie eine Option aus:

   - `Active` - Wählen Sie diese Option aus, wenn die Preisregel auf Ihre geeigneten Produkte angewendet werden soll, und passen Sie Ihre Listenpreise vor der Veröffentlichung in Amazon an.

   - `Inactive` - Wählen Sie diese Option aus, wenn die Preisregel nicht für Ihre förderfähigen Produkte gelten soll. Diese Option wird höchstwahrscheinlich verwendet, wenn eine Preisregel geändert oder nach einer begrenzten Promotion deaktiviert wird.

1. Für **[!UICONTROL From]** und **[!UICONTROL To]** ein Start- und ein Enddatum für die Preisregel eingeben.

   Sie können auch auf das Kalendersymbol klicken, um ein Datum aus dem dynamischen Kalender auszuwählen. Diese automatische Start- und Stopp-Option ist nützlich, wenn Sie zeitlich begrenzte oder saisonale Promotions mit bestimmten Start- und Enddaten einrichten.

1. Für **[!UICONTROL Priority]**, geben Sie einen numerischen Wert für die Regelpriorität ein.

   Prioritätswert gleich `1` hat höchste Priorität. Wenn Sie mehrere Regeln für aktive Preise haben, können Sie diesen Prioritätswert verwenden, um zu bestimmen, welche Regel zuerst angewendet wird. Dieses Feld ist erforderlich, um die _[!UICONTROL Discard Subsequent Rules]_Funktion.

1. Für **[!UICONTROL Discard Subsequent Rules]**, wählen Sie eine Option aus:

   - `Yes` - Wählen Sie diese Option, wenn Sie keine anderen Preisregeln anwenden möchten, die für ein Produkt gelten können. Das Verwerfen nachfolgender Regeln bedeutet, dass, wenn mehrere Preisregeln für dasselbe Produkt gelten, nur die Preisregel mit dem höchsten definierten Prioritätswert auf das Produkt angewendet wird. Diese Option verhindert, dass mehrere Preisregeln stapeln und unbeabsichtigte zusätzliche Rabatte bieten.

   - `No` - Wählen Sie diese Option, wenn Sie zulassen möchten, dass mehrere Preisregeln auf dasselbe Produkt angewendet werden. Diese Option könnte zu Stapelung und mehreren Rabatten führen, die angewendet werden sollen.

>[!NOTE]
>
>Um nachfolgende Regeln verwerfen zu können, muss eine Preisregel über eine **Priorität** -Wert.

![Allgemeine Preisregeleinstellungen](assets/amazon-pricing-rule-general.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Rule Name] | (Erforderlich) Geben Sie einen Namen für die Regel ein, der für interne Identifizierungszwecke verwendet wird. Je beschreibender der Regelname ist, desto besser. Beispiel: &quot;25 % Rabatt auf den Jahresbuchverkauf.&quot; |
| [!UICONTROL Description] | Geben Sie eine detaillierte Beschreibung ein, in der die Regel erläutert wird (auch für interne Zwecke verwendet). Beispiel: &quot;Verkauf Ende des Jahres, 25 % aller Artikel in der Kategorie &quot;Bücher&quot;. |
| [!UICONTROL Status] | Optionen:<ul><li>**[!UICONTROL Inactive]** - Die Preisregel gilt nicht für Ihre Auflistungen. Diese Option kann verwendet werden, wenn eine Preisregel geändert oder nach einer begrenzten Promotion deaktiviert wird.</li><li>**[!UICONTROL Active]** - Die Preisregel gilt für Ihre Auflistungen und passt Ihre Auflistungspreise vor der Veröffentlichung in Amazon an.</li></ul> |
| [!UICONTROL From] | Geben Sie das Startdatum an, an dem die Preisregel beginnt. Wenn Sie beispielsweise einen Verkauf im letzten Monat des Jahres durchführen möchten, legen Sie die Variable `From` -Datum auf den 1. Dezember zu setzen, damit die Preisregel ab dem 1. Dezember automatisch auf Ihre Amazon-Listen angewendet wird. |
| [!UICONTROL To] | Geben Sie das Enddatum an, an dem die Preisregel endet. Um den Verkauf im vorherigen Beispiel auf den letzten Monat des Jahres zu beschränken, würden Sie die Variable `To` Datum auf den 31. Dezember gesetzt, sodass die Preisregel am 31. Dezember abläuft. |
| [!UICONTROL Priority] | Geben Sie einen Wert für die Priorität der Preisregel ein. Ein Prioritätswert von `1` hat höchste Priorität. Wenn Sie mehrere Preisregeln haben, können Sie den Prioritätswert verwenden, um zu bestimmen, welche Regel zuerst angewendet wird. Dieses Feld ist erforderlich, um die **Nachfolgende Regeln verwerfen** Funktion. |
| [!UICONTROL Discard Subsequent Rules] | Wird verwendet, um die Stapelung mehrerer Preisregeln und die Bereitstellung zusätzlicher Rabatte zu ermöglichen oder zu verhindern. Um nachfolgende Regeln verwerfen zu können, muss für eine Preisregel ein Wert definiert sein für **[!UICONTROL Priority]**. Optionen:<ul><li>**[!UICONTROL Yes]** - Wählen Sie aus, wann keine anderen Preisregeln angewendet werden sollen, die für ein Produkt gelten. Das Verwerfen nachfolgender Regeln bedeutet, dass bei mehreren Preisregeln für dasselbe Produkt nur die Preisregel mit dem höchsten definierten Prioritätswert angewendet wird.</li><li>**[!UICONTROL No]** - Wählen Sie aus, wann mehrere Preisregeln auf dasselbe Produkt angewendet werden sollen. Diese Option kann zu Stapelung und mehreren Rabatten führen, die auf Ihren Listenpreis angewendet werden.</li></ul> |
