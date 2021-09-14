---
title: Allgemeine Preisregeleinstellungen
description: Verwenden Sie die allgemeinen Preisregeleinstellungen, um die Hauptmerkmale einer Regel für den Börsennotierungspreis zu definieren.
redirect_from: /sales-channels/asc/ob-pricing-rules-general-settings.html
exl-id: 915b3eed-997e-4f94-a23f-0553a9dfe30c
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# Allgemeine Preisregeleinstellungen

Definieren Sie den Namen, die Beschreibung, das aktive Datum und die Priorität für die Regel.

## Füllen Sie den Abschnitt Allgemeine Preisregeln aus.

1. Geben Sie für **[!UICONTROL Rule Name]** (erforderlich) den Namen für die Regel ein.

   Dieser Name dient nur Ihrer internen Identifizierung. Je beschreibender der Regelname ist, desto besser.

1. Geben Sie für **[!UICONTROL Description]** eine detaillierte Beschreibung Ihrer Regel ein.

   Diese Beschreibung kann Informationen zu den qualifizierenden Produkten, den aktiven Daten, der Formel zur Berechnung Ihres angepassten Preises oder andere Informationen enthalten, die Sie für nützlich halten, wenn Sie die Regel ändern möchten.

1. Wählen Sie für **[!UICONTROL Status]** eine Option:

   - `Active` - Wählen Sie diese Option aus, wenn die Preisregel auf Ihre geeigneten Produkte angewendet werden soll, und passen Sie Ihre Listenpreise vor der Veröffentlichung in Amazon an.

   - `Inactive` - Wählen Sie diese Option aus, wenn die Preisregel nicht für Ihre förderfähigen Produkte gelten soll. Diese Option wird höchstwahrscheinlich verwendet, wenn eine Preisregel geändert oder nach einer begrenzten Promotion deaktiviert wird.

1. Geben Sie für **[!UICONTROL From]** und **[!UICONTROL To]** ein Start- und Enddatum für die Preisregel ein.

   Sie können auch auf das Kalendersymbol klicken, um ein Datum aus dem dynamischen Kalender auszuwählen. Diese automatische Start- und Stopp-Option ist nützlich, wenn Sie zeitlich begrenzte oder saisonale Promotions mit bestimmten Start- und Enddaten einrichten.

1. Geben Sie für **[!UICONTROL Priority]** einen numerischen Wert für die Regelpriorität ein.

   Der Prioritätswert von `1` ist die höchste Priorität. Wenn Sie mehrere Regeln für aktive Preise haben, können Sie diesen Prioritätswert verwenden, um zu bestimmen, welche Regel zuerst angewendet wird. Dieses Feld ist erforderlich, um die Funktion _[!UICONTROL Discard Subsequent Rules]_zu verwenden.

1. Wählen Sie für **[!UICONTROL Discard Subsequent Rules]** eine Option:

   - `Yes` - Wählen Sie diese Option, wenn Sie keine anderen Preisregeln anwenden möchten, die für ein Produkt gelten können. Das Verwerfen nachfolgender Regeln bedeutet, dass, wenn mehrere Preisregeln für dasselbe Produkt gelten, nur die Preisregel mit dem höchsten definierten Prioritätswert auf das Produkt angewendet wird. Diese Option verhindert, dass mehrere Preisregeln stapeln und unbeabsichtigte zusätzliche Rabatte bieten.

   - `No` - Wählen Sie diese Option, wenn Sie zulassen möchten, dass mehrere Preisregeln auf dasselbe Produkt angewendet werden. Diese Option könnte zu Stapelung und mehreren Rabatten führen, die angewendet werden sollen.

>[!NOTE]
>
>Um nachfolgende Regeln zu verwerfen, muss eine Preisregel einen definierten Wert (**Priorität** ) haben.

![Allgemeine Preisregeleinstellungen](assets/amazon-pricing-rule-general.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Rule Name] | (Erforderlich) Geben Sie einen Namen für die Regel ein, der für interne Identifizierungszwecke verwendet wird. Je beschreibender der Regelname ist, desto besser. Beispiel: &quot;25 % Rabatt auf den Jahresbuchverkauf.&quot; |
| [!UICONTROL Description] | Geben Sie eine detaillierte Beschreibung ein, in der die Regel erläutert wird (auch für interne Zwecke verwendet). Beispiel: &quot;Verkauf Ende des Jahres, 25 % aller Artikel in der Kategorie &quot;Bücher&quot;. |
| [!UICONTROL Status] | Optionen:<ul><li>**[!UICONTROL Inactive]** - Die Preisregel gilt nicht für Ihre Auflistungen. Diese Option kann verwendet werden, wenn eine Preisregel geändert oder nach einer begrenzten Promotion deaktiviert wird.</li><li>**[!UICONTROL Active]** - Die Preisregel gilt für Ihre Auflistungen und passt Ihre Auflistungspreise vor der Veröffentlichung in Amazon an.</li></ul> |
| [!UICONTROL From] | Geben Sie das Startdatum an, an dem die Preisregel beginnt. Um beispielsweise einen Verkauf im letzten Monat des Jahres durchzuführen, würden Sie das `From`-Datum auf den 1. Dezember setzen, sodass die Preisregel ab dem 1. Dezember automatisch auf Ihre Amazon-Listen angewendet wird. |
| [!UICONTROL To] | Geben Sie das Enddatum an, an dem die Preisregel endet. Um den Verkauf im vorherigen Beispiel auf den letzten Monat des Jahres zu beschränken, würden Sie das `To`-Datum auf den 31. Dezember festlegen, sodass die Preisregel am 31. Dezember abläuft. |
| [!UICONTROL Priority] | Geben Sie einen Wert für die Priorität der Preisregel ein. Ein Prioritätswert von `1` ist die höchste Priorität. Wenn Sie mehrere Preisregeln haben, können Sie den Prioritätswert verwenden, um zu bestimmen, welche Regel zuerst angewendet wird. Dieses Feld ist erforderlich, um die Funktion **Nachfolgende Regeln verwerfen** zu verwenden. |
| [!UICONTROL Discard Subsequent Rules] | Wird verwendet, um die Stapelung mehrerer Preisregeln und die Bereitstellung zusätzlicher Rabatte zu ermöglichen oder zu verhindern. Um nachfolgende Regeln zu verwerfen, muss für eine Preisregel ein Wert definiert sein, der für **[!UICONTROL Priority]** definiert ist. Optionen:<ul><li>**[!UICONTROL Yes]** - Wählen Sie aus, wann keine anderen Preisregeln angewendet werden sollen, die für ein Produkt gelten. Das Verwerfen nachfolgender Regeln bedeutet, dass bei mehreren Preisregeln für dasselbe Produkt nur die Preisregel mit dem höchsten definierten Prioritätswert angewendet wird.</li><li>**[!UICONTROL No]** - Wählen Sie aus, wann mehrere Preisregeln auf dasselbe Produkt angewendet werden sollen. Diese Option kann zu Stapelung und mehreren Rabatten führen, die auf Ihren Listenpreis angewendet werden.</li></ul> |
