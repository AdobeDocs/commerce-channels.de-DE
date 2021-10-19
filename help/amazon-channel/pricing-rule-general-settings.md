---
title: Allgemeine Preisregel - Einstellungen
description: Verwenden Sie die allgemeinen Preisregeleinstellungen, um die primären Eigenschaften einer Preisregel für die Auflistung zu definieren.
redirect_from: /sales-channels/asc/ob-pricing-rules-general-settings.html
exl-id: 915b3eed-997e-4f94-a23f-0553a9dfe30c
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# Allgemeine Preisregel - Einstellungen

Definieren Sie den Namen, die Beschreibung, die aktiven Daten und die Priorität der Regel.

## Vervollständigen Sie den Abschnitt mit den allgemeinen Preisregel-Einstellungen.

1. für **[!UICONTROL Rule Name]** (erforderlich), geben Sie den Namen für die Regel ein.

   Dieser Name dient nur zu Ihrer internen Identifizierung. Je beschreibender der Regelname, desto besser.

1. für **[!UICONTROL Description]**, geben Sie eine detaillierte Beschreibung Ihrer Regel ein.

   Diese Beschreibung kann Informationen zu den Produkten enthalten, die die Kriterien erfüllen, zu den aktiven Daten, zur Formel zur Berechnung des angepassten Preises oder zu anderen Informationen, die Sie für nützlich halten, wenn Sie die Regel ändern möchten.

1. für **[!UICONTROL Status]**, wählen Sie eine Option aus:

   - `Active` - Wählen Sie diese Option aus, wenn die Preisregel auf die in Frage kommenden Produkte angewendet und die Listenpreise vor der Veröffentlichung auf Amazon angepasst werden sollen.

   - `Inactive` - Wählen Sie diese Option aus, wenn die Preisregel nicht auf Ihre förderfähigen Produkte angewendet werden soll. Diese Option wird höchstwahrscheinlich verwendet, wenn eine Preisregel geändert oder nach einer begrenzten Promotion deaktiviert wird.

1. für **[!UICONTROL From]** und **[!UICONTROL To]**, geben Sie ein Start- und Enddatum für die Preisregel ein.

   Sie können auch auf das Kalendersymbol klicken, um ein Datum aus dem dynamischen Kalender auszuwählen. Diese automatische Beginn- und Stoppoption ist nützlich, wenn zeitlich begrenzte oder saisonale Promotions mit bestimmten Start- und Enddaten eingerichtet werden.

1. für **[!UICONTROL Priority]**, geben Sie einen numerischen Wert für die Regelpriorität ein.

   Prioritätswert gleich `1` hat höchste Priorität. Wenn Sie mehrere aktive Preisregeln haben, können Sie diesen Prioritätswert verwenden, um zu bestimmen, welche Regel zuerst angewendet wird. Dieses Feld ist erforderlich, um _[!UICONTROL Discard Subsequent Rules]_Funktion.

1. für **[!UICONTROL Discard Subsequent Rules]**, wählen Sie eine Option aus:

   - `Yes` - Wählen Sie diese Option, wenn keine anderen Preisregeln für ein Produkt angewendet werden sollen. Wenn mehrere Preisregeln für ein und dasselbe Produkt gelten, bedeutet das Verwerfen nachfolgender Regeln, dass nur die Preisregel mit dem höchsten definierten Prioritätswert auf das Produkt angewendet wird. Diese Option verhindert, dass mehrere Preisregeln stapelbar sind und unbeabsichtigte zusätzliche Rabatte bieten.

   - `No` - Wählen Sie diese Option, wenn mehrere Preisregeln auf dasselbe Produkt angewendet werden sollen. Diese Option kann zu einer Stapelung und mehreren Rabatten führen.

>[!NOTE]
>
>Um nachfolgende Regeln zu verwerfen, muss eine Preisregel eine **Priorität** Wert.

![Allgemeine Preisregel - Einstellungen](assets/amazon-pricing-rule-general.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Rule Name] | (Erforderlich) Geben Sie einen Namen für die Regel ein, der für interne Identifizierungszwecke verwendet wird. Je beschreibender der Regelname, desto besser. Zum Beispiel &quot;25% Rabatt auf den Buchverkauf am Jahresende&quot;. |
| [!UICONTROL Description] | Geben Sie eine detaillierte Beschreibung ein, die die Regel erklärt (auch für interne Zwecke verwendet). Zum Beispiel &quot;Jahresende, 25 % aller Artikel in der Kategorie der Bücher&quot;. |
| [!UICONTROL Status] | Optionen:<ul><li>**[!UICONTROL Inactive]** - Die Preisregel gilt nicht für Ihre Auflistungen. Diese Option kann verwendet werden, wenn eine Preisregel geändert oder nach einer begrenzten Promotion deaktiviert wird.</li><li>**[!UICONTROL Active]** - Die Preisregel gilt für Ihre Auflistungen und passt Ihre Listenpreise vor der Veröffentlichung auf Amazon an.</li></ul> |
| [!UICONTROL From] | Geben Sie das Datum des Beginns ein, an dem die Preisregel beginnt. Wenn Sie z. B. im letzten Monat des Jahres einen Verkauf durchführen möchten, setzen Sie die `From` -Datum bis 1. Dezember, damit die Preisregel ab dem 1. Dezember automatisch auf Ihre Amazon-Listen Anwendung findet. |
| [!UICONTROL To] | Geben Sie das Enddatum ein, an dem die Preisregel endet. Wenn Sie das vorherige Beispiel fortsetzen und den Verkauf auf den letzten Monat des Jahres beschränken möchten, setzen Sie die `To` Dezember 31, sodass die Preisregel am 31. Dezember endet. |
| [!UICONTROL Priority] | Geben Sie einen Wert für die Priorität der Preisregel ein. Ein Prioritätswert gleich `1` hat höchste Priorität. Wenn Sie mehrere Preisregeln haben, können Sie den Prioritätswert verwenden, um zu bestimmen, welche Regel zuerst angewendet wird. Dieses Feld ist erforderlich, um **Nachfolgende Regeln verwerfen** Funktion. |
| [!UICONTROL Discard Subsequent Rules] | Wird verwendet, um mehrere Preisregeln stapelbar zu machen oder zu verhindern und zusätzliche Rabatte zu gewähren. Um nachfolgende Regeln zu verwerfen, muss für eine Preisregel ein Wert definiert sein für **[!UICONTROL Priority]**. Optionen:<ul><li>**[!UICONTROL Yes]** - Wählen Sie aus, ob andere Preisregeln, die auf ein Produkt zutreffen können, angewendet werden sollen. Wenn mehrere Preisregeln für ein und dasselbe Produkt gelten, bedeutet das Verwerfen nachfolgender Regeln, dass nur die Preisregel mit dem höchsten definierten Prioritätswert angewendet wird.</li><li>**[!UICONTROL No]** - Wählen Sie aus, wann mehrere Preisregeln auf dasselbe Produkt angewendet werden sollen. Diese Option kann zu Stapelung und mehreren Rabatten führen, die auf Ihren Listenpreis angewendet werden.</li></ul> |
