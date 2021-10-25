---
title: Amazon-Preise verwalten
description: Sie können die Preise für Ihre Amazon-Auflistungen anhand der Preisregeln von Ihrem COmmerce-Store abweichen.
redirect_from: /sales-channels/asc/ob-pricing-rules.html
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# Amazon-Preise verwalten

Mit Amazon Sales Kanal können Sie Preisregeln festlegen, mit denen Sie Ihren Amazon-Listingpreis auf einen anderen als den definierten einstellen können. **[!UICONTROL Magento Price Source]** in [Börsenkurs](./listing-price.md). Sie können auch mehrere Regeln stapeln und sogar intelligente Preise verwenden, um Ihren Amazon-Listenpreis auf Grundlage der Konkurrent anzupassen. [[!DNL Buy Box]](./buy-box-competitor-pricing.md) dem Preis oder [niedrigster Konkurrent](./lowest-competitor-pricing.md).

Es gibt zwei Arten von Preisregeln:

- [Standardpreisregel](./standard-price-rules.md)
- [Intelligente Preisanpassungsregel](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >Intelligente Preisanpassungsregeln funktionieren nicht ordnungsgemäß, wenn die Amazon-Region auf `Inactive` Status, wie es während des Einbodens ist. Ihre Preisberechnungen hängen von Ihren Versandkosten ab. Ihre Region muss sich in `Active` Status für Ihre Versandtarife, die von Amazon aus synchronisiert werden sollen.
   >
   >Um den Regionsstatus in Ihrem Amazon-Konto zu aktualisieren, navigieren Sie zu Einstellungen > Kontoinformationen > Urlaubseinstellungen. Siehe [Amazon: Listungsstatus für Urlaube](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620){Zielgruppe=&quot;_blank&quot;} (Anmeldung bei Verkäuferzentrale erforderlich).

Mit dieser Funktion können Sie Ihre Amazon-Preise auf eine Art und Weise manipulieren, die dem [!DNL Commerce] [Katalogpreisregeln](https://docs.magento.com/user-guide/catalog/pricing.html){Zielgruppe=&quot;_blank&quot;}. Sie können komplexe Regeln erstellen, mit denen Sie die Preise für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder auch mit bestimmten Eigenschaften ändern können.

Sie können Preisregeln für Ihre Amazon-Auflistungen hinzufügen. Preisregeln können verwendet werden, um Ihre Notierungspreise auf Basis bestimmter Bedingungen automatisch anzupassen. Preisregeln werden ausgelöst und berechnen den angepassten Preis, bevor Ihr Produkt auf Amazon aufgeführt wird.

>[!NOTE]
>
>Die Preisquelle für Ihre Amazon-Auflistungen ist definiert für **[!UICONTROL Magento Price Source]** in [Börsenkurs](./listing-price.md) Einstellungen. Bei allen in der Preisregel definierten Anpassungsberechnungen wird die Preisquelle als Ausgangswert verwendet.

Preisregeln ermöglichen es Ihnen, einen anderen Amazon-Listenpreis als Ihren **[!UICONTROL Magento Price Source]** in [Börsenkurs](./listing-price.md) Einstellungen. Sie können auch mehrere Regeln stapeln, die zusammenarbeiten, um Ihren Preis anzupassen.

Eine Preis-/Verpreisungs-Regel erfordert während der Einrichtung drei Informationssätze:

- [Allgemeine Einstellungen](./pricing-rule-general-settings.md): Definiert den Namen, die Beschreibung, die aktiven Daten und die Priorität einer Regel und legt das Verhalten nachfolgender Regeln auf der Grundlage ihrer Prioritätseinstellung fest.
- [Bedingungen](./pricing-rule-conditions.md): zu bestimmen, welche Produkte für die Preisregel infrage kommen.
- [Aktionen](./pricing-rule-actions.md): Definieren Sie die Anpassungsberechnungen, die zur Bestimmung des Börsenkurses auf die Kursquelle angewendet werden.

Sie können [Standardpreisregeln](./standard-price-rules.md) , die Ihren Amazon-Listingpreis automatisch in Relation zu den ausgewählten ändern **[!UICONTROL Magento Price Source]** in [Börsenkurs](./listing-price.md) Einstellungen. Mit dieser Funktion können Sie Ihre Amazon-Preise auf eine Art und Weise manipulieren, die dem [!DNL Commerce] [Katalogpreisregeln](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){Zielgruppe=&quot;_blank&quot;}. Sie können komplexe Regeln erstellen, die die Preise für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder Produkte mit bestimmten Eigenschaften automatisch ändern. Sie können traditionelle Einstellungen vornehmen und Ihre Produkte neu berechnen, um sie zu erhöhen oder zu reduzieren, basierend auf einem festen Betrag oder einem bestimmten Prozentsatz.

Ein weiteres mächtiges Werkzeug ist [Intelligente Preisgestaltung](./intelligent-repricing-rules.md) Funktion, mit der Sie Ihren Amazon-Börsennotierungspreis auf Grundlage des Konkurrenten anpassen können [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Preis oder [Niedrigster Konkurrent](./lowest-competitor-pricing.md). Ähnlich der [!DNL Commerce] [Katalogpreisregeln](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){Zielgruppe=&quot;_blank&quot;}, mit dieser erweiterten Funktion können Sie Ihre Amazon-Preise durch Erstellung komplexer Regeln ändern. Die Regeln können den Spielraum für eine Preisänderung für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder sogar mit bestimmten Produktmerkmalen festlegen.

Intelligente Neupreisgestaltung zur Anpassung der Listenpreise in Amazon, basierend auf den Preisen von Konkurrent. Amazon Sales Kanal hat Sicherheitsvorkehrungen für Sie eingebaut, um Margen zu schützen oder die Preise eines Händlers nicht mit einem geringen Rückkopplungsverhältnis abzugleichen. Verwenden [Intelligente Preisanpassungsregeln](./intelligent-repricing-rules.md), können die Listenpreise in Amazon automatisch als fester oder prozentualer Betrag (nach oben oder unten) manipuliert oder sogar mit dem [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Preis oder [Niedrigster Konkurrent](./lowest-competitor-pricing.md) auf der Grundlage von Einzelposten. Regeln können sogar so gestapelt werden, dass sie unbegrenzte Flexibilität bieten.

Sie können wichtige Aspekte von Regeln steuern, wie z. B. aktiven/inaktiven Status, Website-Berechtigung, optionale Datumsbereiche und optionale Prioritätsstufen (für Regelstapelung verwendet).

Sie können beispielsweise die Bedingungen für eine Preisregel festlegen und festlegen, die, wenn die Bedingungen erfüllt sind, den Börsennotierungspreis automatisch anpassen kann, bevor er an Amazon gesendet wird.

Eine weitere Preisoption ist [Preisüberschreibung](./overrides.md), die auf der einzelnen Listenniveau festgelegt ist. A [Preisüberschreibung](./overrides.md) kann eingestellt werden, und eine Außerkraftsetzung ignoriert/hat Vorrang vor allen anderen Standardeinstellungen, Einstellungen und Regeln. An [überschreiben](./overrides.md) kann für Preis, Bearbeitungszeit, Zustand und Händlernotizen (mit wenigen Ausnahmen) festgelegt werden.

![Preisregeln](assets/amazon-pricing-rules.png)

## Standardspalten

| Spalte | Beschreibung |
|---|---|
| [!UICONTROL Name] | Der Name der Preisregel, wie in [Allgemeine Preisregel - Einstellungen](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | Der Regeltyp, wie in [Preisregelaktionen](./pricing-rule-actions.md) (entweder Standardpreisregel oder Intelligente Neupreisregelung) |
| [!UICONTROL Is Active] | Gibt an, ob die Regel aktiv ist, wie in [Allgemeine Preisregel - Einstellungen](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | Die Priorität gegenüber anderen Preisbedingungen gemäß [Allgemeine Preisregel - Einstellungen](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Gibt an, ob weitere Preisregeln für die unter diese Regel fallenden Erzeugnisse gemäß [Allgemeine Preisregel](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | Der Beginn des Zeitraums, in dem die Regel aktiv ist |
| [!UICONTROL To Date] | Das Ende des Zeitraums, in dem die Regel aktiv ist |
| [!UICONTROL Action] | Liste aller Aktionen, die auf eine bestimmte Auflistung angewendet werden können. Klicken Sie zum Anwenden einer Aktion auf **[!UICONTROL Select]** in _[!UICONTROL Action]_Spalte. Optionen: `Edit Price Rule` / `Delete Price Rule` |
