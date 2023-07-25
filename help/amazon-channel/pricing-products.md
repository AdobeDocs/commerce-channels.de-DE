---
title: Amazon-Preise verwalten
description: Sie können die Preise für Ihre Amazon-Auflistungen mithilfe der Preisregeln von Ihrem COCommerce-Store unterscheiden.
feature: Sales Channels, Price Rules
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 0%

---

# Amazon-Preise verwalten

Mit dem Amazon-Vertriebskanal können Sie Preisregeln festlegen, mit denen Sie Ihren Amazon-Listenpreis von der definierten **[!UICONTROL Magento Price Source]** in [Listenpreis](./listing-price.md). Sie können auch mehrere Regeln stapeln und sogar die intelligente Preisgestaltung verwenden, um Ihren Amazon-Listingpreis auf Grundlage der [[!DNL Buy Box]](./buy-box-competitor-pricing.md) oder [niedrigster Wettbewerbspreis](./lowest-competitor-pricing.md).

Es gibt zwei Arten von Preisregeln:

- [Standardmäßige Preisregel](./standard-price-rules.md)
- [Intelligente Neupreisregel](./intelligent-repricing-rules.md)

  >[!IMPORTANT]
  >
  >Intelligente Regeln für die Neuberechnung funktionieren nicht ordnungsgemäß, wenn der Amazon-Bereich auf `Inactive` -Status, wie es beim Onboarding der Fall ist. Ihre Preisberechnungen hängen von Ihren Versandkosten ab und Ihre Region muss sich in `Active` Status für Ihre Versandraten, die von Amazon synchronisiert werden.
  >
  >Um den Status Ihrer Region in Ihrem Amazon-Konto zu aktualisieren, gehen Sie zu Einstellungen > Kontoinformationen > Urlaubseinstellungen. Siehe [Amazon: Listening-Status für Urlaub](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620) (Anmeldung bei Seller Central erforderlich).

Mit dieser Funktion können Sie Ihre Amazon-Preise so anpassen, dass sie der [!DNL Commerce] [Katalogpreisregeln](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html). Sie können komplexe Regeln erstellen, mit denen Sie die Preise für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder auch mit bestimmten Attributen ändern können.

Sie können Preisregeln für Ihre Amazon-Listen hinzufügen. Mit Preisregeln können Sie Ihre Listenpreise anhand einer Reihe definierter Bedingungen automatisch anpassen. Preisregeln werden ausgelöst und berechnen Ihren angepassten Preis, bevor Ihr Produkt in Amazon aufgeführt wird.

>[!NOTE]
>
>Die Preisquelle für Ihre Amazon-Listen wird für **[!UICONTROL Magento Price Source]** in [Listenpreis](./listing-price.md) -Einstellungen. Alle in der Preisregel definierten Anpassungsberechnungen verwenden die Preisquelle als Startwert.

Mit den Preisregeln können Sie Ihren Amazon-Listenpreis von Ihrem **[!UICONTROL Magento Price Source]** in [Listenpreis](./listing-price.md) -Einstellungen. Sie können auch mehrere Regeln stapeln, die zusammenarbeiten, um Ihren Preis anzupassen.

Eine Preis-/Preisänderungsregel erfordert während der Einrichtung drei Informationssätze:

- [Allgemeine Einstellungen](./pricing-rule-general-settings.md): Definiert den Namen, die Beschreibung, das aktive Datum und die Priorität für eine Regel und legt das Verhalten nachfolgender Regeln basierend auf ihrer Prioritätseinstellung fest.
- [Bedingungen](./pricing-rule-conditions.md): Bestimmen Sie, welche Produkte für die Preisregel infrage kommen.
- [Aktionen](./pricing-rule-actions.md): Definieren Sie die auf die Preisquelle angewendeten Anpassungsberechnungen zur Bestimmung des Börsenkurses.

Sie können [Standardpreisregeln](./standard-price-rules.md) , mit dem Ihr Amazon-Listingpreis automatisch im Verhältnis zur ausgewählten angepasst wird **[!UICONTROL Magento Price Source]** in [Listenpreis](./listing-price.md) -Einstellungen. Mit dieser Funktion können Sie Ihre Amazon-Preise so anpassen, dass sie der [!DNL Commerce] [Katalogpreisregeln](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html). Sie können komplexe Regeln erstellen, die die Preise für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder Produkte mit bestimmten Attributen automatisch ändern. Sie können traditionelle Einstellungen vornehmen und Ihre Produkte neu berechnen, um sie basierend auf einem festen Betrag oder Prozentsatz zu erhöhen oder zu verringern.

Ein weiteres leistungsfähiges Werkzeug ist die [Intelligente Neuberechnung](./intelligent-repricing-rules.md) Funktion, die Ihren Amazon-Listingpreis auf Grundlage des Konkurrenten anpasst [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Preis oder [Niedrigster Wettbewerbspreis](./lowest-competitor-pricing.md). Ähnlich wie bei [!DNL Commerce] [Katalogpreisregeln](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html)bietet Ihnen diese erweiterte Funktion die Möglichkeit, Ihre Amazon-Preise durch Erstellung komplexer Regeln zu ändern. Regeln können den Umfang einer Preisänderung für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder auch mit bestimmten Produktattributen definieren.

Die intelligente Neuberechnung zur Anpassung Ihrer Amazon-Listenpreise auf der Grundlage der Preise des Konkurrenten. Amazon Sales Channel verfügt über integrierte Schutzmechanismen, mit denen Sie die Spannen schützen oder verhindern können, dass die Preise eines Händlers mit geringem Feedback abgeglichen werden. Verwenden [intelligente Neubewertungsregeln](./intelligent-repricing-rules.md), können die Amazon-Listenpreise automatisch als fester oder prozentualer Betrag (nach oben oder unten) oder sogar mit der [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Preis oder [Niedrigster Wettbewerbspreis](./lowest-competitor-pricing.md) auf Artikelbasis. Regeln können sogar gestapelt werden, um eine unbegrenzte Flexibilität zu bieten.

Sie können wichtige Aspekte von Regeln steuern, z. B. den aktiven/inaktiven Status, die Website-Eignung, optionale Datumsbereiche und optionale Prioritätsstufen (für die Regelstapelung verwendet).

Sie können beispielsweise die Bedingungen für eine Preisregel definieren und festlegen, die, wenn die Bedingungen erfüllt sind, automatisch Ihren Listenpreis ändert, bevor er an Amazon gesendet wird.

Eine weitere Preisoption ist [Preisüberschreibung](./overrides.md), der auf der Ebene der einzelnen Listen festgelegt wird. A [Preisüberschreibung](./overrides.md) kann festgelegt werden. Bei einer Außerkraftsetzung werden alle anderen Standardeinstellungen, Einstellungen und Regeln ignoriert/überschrieben. Ein [override](./overrides.md) kann für Preis, Bearbeitungszeit, Bedingung und Verkaufshinweise (mit einigen Ausnahmen) festgelegt werden.

![Preisregeln](assets/amazon-pricing-rules.png){width="600" zoomable="yes"}

## Standardspalten

| Spalte | Beschreibung |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Name] | Der Name der Preisregel, wie in [Allgemeine Preisregeleinstellungen](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | Der Regeltyp, wie in [Preisregelaktionen](./pricing-rule-actions.md) (entweder Standardpreisregel oder intelligente Neupreisregel) |
| [!UICONTROL Is Active] | Gibt an, ob die Regel aktiv ist, wie in [Allgemeine Preisregeleinstellungen](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | Die Priorität gegenüber anderen Preisbedingungen gemäß [Allgemeine Preisregeleinstellungen](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Gibt an, ob weitere Preisregeln für die unter diese Regel fallenden Erzeugnisse verarbeitet werden, wie in [Allgemeine Einstellungen der Preisregel](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | Der Anfang des Zeitraums, in dem die Regel aktiv ist |
| [!UICONTROL To Date] | Das Ende des Zeitraums, in dem die Regel aktiv ist |
| [!UICONTROL Action] | Listet alle Aktionen auf, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie auf **[!UICONTROL Select]** im _[!UICONTROL Action]_Spalte. Optionen: `Edit Price Rule` / `Delete Price Rule` |
