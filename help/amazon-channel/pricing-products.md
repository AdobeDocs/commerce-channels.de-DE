---
title: Amazon-Preise verwalten
description: Sie können die Preise für Ihre Amazon-Auflistungen mithilfe der Preisregeln von Ihrem Commerce-Store unterscheiden.
feature: Sales Channels, Price Rules
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# Amazon-Preise verwalten

Mit dem Amazon-Vertriebskanal können Sie Preisregeln festlegen, mit denen Sie Ihren Amazon-Listenpreis festlegen können, der vom definierten **[!UICONTROL Magento Price Source]** in Ihrem [Listenpreis](./listing-price.md) abweicht. Sie können auch mehrere Regeln stapeln und sogar die intelligente Preisgestaltung verwenden, um Ihren Amazon-Listenpreis auf Grundlage des [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Preises der Konkurrenten oder des [niedrigsten Konkurrenzpreises](./lowest-competitor-pricing.md) anzupassen.

Es gibt zwei Arten von Preisregeln:

- [Standardmäßige Preisregel](./standard-price-rules.md)
- [Intelligente Neupreisregel](./intelligent-repricing-rules.md)

  >[!IMPORTANT]
  >
  >Intelligente Regeln für die Neuberechnung funktionieren nicht ordnungsgemäß, wenn der Amazon-Bereich auf den Status &quot;`Inactive`&quot;gesetzt ist, wie dies beim Onboarding der Fall ist. Ihre Preisberechnungen hängen von Ihren Versandtarifen ab und Ihre Region muss den Status `Active` aufweisen, damit Ihre Versandraten mit Amazon synchronisiert werden.
  >
  >Um den Status Ihrer Region in Ihrem Amazon-Konto zu aktualisieren, gehen Sie zu Einstellungen > Kontoinformationen > Urlaubseinstellungen. Siehe [Amazon: Listing Status for Vacations](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620) (Anmeldung von Seller Central erforderlich).

Mit dieser Funktion können Sie Ihre Amazon-Preise auf eine Weise bearbeiten, die den [!DNL Commerce] [Katalogpreisregeln](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html) ähnelt. Sie können komplexe Regeln erstellen, mit denen Sie die Preise für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder auch mit bestimmten Attributen ändern können.

Sie können Preisregeln für Ihre Amazon-Listen hinzufügen. Mit Preisregeln können Sie Ihre Listenpreise anhand einer Reihe definierter Bedingungen automatisch anpassen. Preisregeln werden ausgelöst und berechnen Ihren angepassten Preis, bevor Ihr Produkt in Amazon aufgeführt wird.

>[!NOTE]
>
>Die Preisquelle für Ihre Amazon-Auflistungen wird für **[!UICONTROL Magento Price Source]** in Ihren Einstellungen für [Auflistungspreis](./listing-price.md) definiert. Alle in der Preisregel definierten Anpassungsberechnungen verwenden die Preisquelle als Startwert.

Mit den Preisregeln können Sie Ihren Amazon-Listenpreis in Ihren Einstellungen für [Listenpreis](./listing-price.md) von Ihrem **[!UICONTROL Magento Price Source]** unterscheiden. Sie können auch mehrere Regeln stapeln, die zusammenarbeiten, um Ihren Preis anzupassen.

Eine Preis-/Preisänderungsregel erfordert während der Einrichtung drei Informationssätze:

- [Allgemeine Einstellungen](./pricing-rule-general-settings.md): Definiert den Namen, die Beschreibung, das aktive Datum und die Priorität für eine Regel und legt das Verhalten nachfolgender Regeln basierend auf ihrer Prioritätseinstellung fest.
- [Bedingungen](./pricing-rule-conditions.md): Bestimmen Sie, welche Produkte für die Preisregel infrage kommen.
- [Aktionen](./pricing-rule-actions.md): Definieren Sie die Anpassungsberechnungen, die auf die Preisquelle angewendet werden, um den Börsennotierungspreis zu bestimmen.

Sie können [Standardpreisregeln](./standard-price-rules.md) erstellen, mit denen Sie Ihren Amazon-Listenpreis in Ihren Einstellungen für [Listenpreis](./listing-price.md) automatisch an den ausgewählten **[!UICONTROL Magento Price Source]** anpassen. Mit dieser Funktion können Sie Ihre Amazon-Preise auf eine Weise bearbeiten, die den [!DNL Commerce] [Katalogpreisregeln](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) ähnelt. Sie können komplexe Regeln erstellen, die die Preise für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder Produkte mit bestimmten Attributen automatisch ändern. Sie können traditionelle Einstellungen vornehmen und Ihre Produkte neu berechnen, um sie basierend auf einem festen Betrag oder Prozentsatz zu erhöhen oder zu verringern.

Ein weiteres leistungsstarkes Tool ist die Funktion [Intelligent Reprice](./intelligent-repricing-rules.md) , mit der Sie Ihren Amazon-Listenpreis anhand des Preises von Konkurrenten [[!DNL Buy Box]](./buy-box-competitor-pricing.md) oder des Preises von Konkurrenten mit dem niedrigsten Preis anpassen können [4}. ](./lowest-competitor-pricing.md) Ähnlich wie bei den [!DNL Commerce] [Katalogpreisregeln](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) können Sie mit dieser erweiterten Funktion Ihre Amazon-Preise durch Erstellung komplexer Regeln ändern. Regeln können den Umfang einer Preisänderung für bestimmte Produkte, Produkte innerhalb bestimmter Kategorien oder auch mit bestimmten Produktattributen definieren.

Die intelligente Neuberechnung zur Anpassung Ihrer Amazon-Listenpreise auf der Grundlage der Preise des Konkurrenten. Amazon Sales Channel verfügt über integrierte Schutzmechanismen, mit denen Sie die Spannen schützen oder verhindern können, dass die Preise eines Händlers mit geringem Feedback abgeglichen werden. Mithilfe von [intelligenten Neupreisregeln](./intelligent-repricing-rules.md) können die Listenpreise in Amazon automatisch als fester oder prozentualer Betrag (nach oben oder unten) manipuliert oder auf Artikelbasis sogar mit dem [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Preis oder dem [niedrigsten Konkurrenzpreis](./lowest-competitor-pricing.md) synchronisiert werden. Regeln können sogar gestapelt werden, um eine unbegrenzte Flexibilität zu bieten.

Sie können wichtige Aspekte von Regeln steuern, z. B. den aktiven/inaktiven Status, die Website-Eignung, optionale Datumsbereiche und optionale Prioritätsstufen (für die Regelstapelung verwendet).

Sie können beispielsweise die Bedingungen für eine Preisregel definieren und festlegen, die, wenn die Bedingungen erfüllt sind, automatisch Ihren Listenpreis ändert, bevor er an Amazon gesendet wird.

Eine weitere Preisoption ist eine [Preisüberschreibung](./overrides.md), die auf der Ebene der einzelnen Listen festgelegt wird. Es kann eine [Preisüberschreibung](./overrides.md) festgelegt werden, und eine Überschreibung ignoriert/hat Vorrang vor allen anderen Standardeinstellungen, Einstellungen und Regeln. Eine [override](./overrides.md) kann für Preis, Bearbeitungszeit, Bedingung und Verkaufshinweise festgelegt werden (mit einigen wenigen Ausnahmen).

![Preisregeln](assets/amazon-pricing-rules.png){width="600" zoomable="yes"}

## Standardspalten

| Spalte | Beschreibung |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Name] | Der Name der Preisregel, wie in den allgemeinen Einstellungen der [Preisregel](./pricing-rule-general-settings.md) festgelegt. |
| [!UICONTROL Rule Type] | Der Regeltyp, wie in [Preisregelaktionen](./pricing-rule-actions.md) festgelegt (entweder Standardpreisregel oder intelligente Neupreisregel) |
| [!UICONTROL Is Active] | Gibt an, ob die Regel aktiv ist, wie in den allgemeinen Einstellungen der Preisregel [festgelegt.](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | Die Priorität gegenüber anderen Preisbedingungen, wie in den Allgemeinen Einstellungen der Preisregel [festgelegt.](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | Gibt an, ob weitere Preisregeln für Produkte verarbeitet werden, die für diese Regel infrage kommen, wie in den allgemeinen Einstellungen der [Preisregel](./pricing-rule-general-settings.md) festgelegt |
| [!UICONTROL From Date] | Der Anfang des Zeitraums, in dem die Regel aktiv ist |
| [!UICONTROL To Date] | Das Ende des Zeitraums, in dem die Regel aktiv ist |
| [!UICONTROL Action] | Listet alle Aktionen auf, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**. Optionen: `Edit Price Rule` / `Delete Price Rule` |
