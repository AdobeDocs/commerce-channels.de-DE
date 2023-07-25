---
title: Amazon-Vertriebskanal - [!UICONTROL Listing Price]
description: Verwenden Sie die Einstellungen für den Listenpreis , um die Preisquelle und den Basiswert (Standard) für Ihre Amazon-Auflistungen zu bestimmen.
feature: Sales Channels, Products, Price Rules
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# [!UICONTROL Listing Price]

[!UICONTROL Listing Price] -Einstellungen sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über die [Store-Dashboard](./amazon-store-dashboard.md).

Diese Einstellungen bestimmen, welche [!DNL Commerce] Preisattribut, das als Ihre Preisquelle verwendet wird, das der (standardmäßige) Basispreiswert für Ihre Amazon-Auflistungen ist. Diese Einstellungen werden von Ihrem [Preisregeln](./pricing-rule-general-settings.md) , um Ihren Amazon-Listenpreis automatisch an den festgelegten Wert anzupassen. _[!UICONTROL Magento Price Source]_.

Sie können Ihre [Preisgestaltung](./price-scope.md) als globale oder Website. Wenn Ihr Preisbereich auf `Global`, gibt es eine einzige Preisquelle für alle Ihre Geschäfte/Websites. Wenn Ihr Preisbereich auf `Website`verwendet die Preisquelle die Ausweichlogik des Website-Preises (sofern verfügbar) gefolgt vom standardmäßigen (globalen) Preis.

Wenn eine Listening-Regel auf mehr als eine Website angewendet werden soll, wird die Reihenfolge, in der der Website-Preis verwendet wird, durch die in der Variablen [Auflistungsregel](./listing-rules.md). Mit diesen Regeln können Sie die Produktpreise in Ihrem Katalog definieren. Informationen dazu, ob Sie den Umfang der Website-Preise verwenden, finden Sie unter [Katalogpreisumfang](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html).

Die unter _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_ und _[!UICONTROL Strike Through Price (MSRP)]_enthalten Ihre konfigurierten Preisattribute. Preisattribute sind [!DNL Commerce] Produktattribute, bei denen der Katalogeingabetyp für den Wert &quot;Store Owner&quot;auf `Price`. Siehe [Attributeingabetypen](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/attributes-input-types.html).

## Einstellungen für den Listenpreis konfigurieren {#configure-listing-price-settings}

1. Klicken **[!UICONTROL Listing Settings]** im Dashboard speichern.

1. Erweitern Sie die _[!UICONTROL Listing Price]_Abschnitt.

1. Für **[!UICONTROL Magento Price Source]** (erforderlich), wählen Sie eine Option aus.

   Der Standardwert ist `Price`. Diese Einstellung bestimmt die Preisquelle, die für Ihre Amazon-Auflistungen verwendet wird. Wenn Sie [Preisregeln](./pricing-products.md), werden die Regeln auf den Wert angewendet, der für das hier ausgewählte Attribut definiert ist. Sie können jedes konfigurierte Preisattribut auswählen. Wenn das ausgewählte Attribut jedoch nicht für ein Produkt ausgefüllt wird, wird die Preisquelle für das Produkt standardmäßig auf `Price` wenn Preisregeln zur Bestimmung des veröffentlichten Amazon-Listenpreises angewendet werden.

1. Für **[!UICONTROL Minimum Advertised Price (MAP)**], wählen Sie eine Option aus.

   Die Standardeinstellung ist keine Auswahl. Diese Einstellung ermöglicht einen mindestens beworbenen Preis (MAP) für ein Produkt. Wenn Sie ein Preisattribut definieren und Ihr Börsennotierungspreis für ein Produkt unter den festgelegten Mindestpreis fällt (basierend auf Ihrer Preisquelle und Ihren Regeln), wird dieser Wert zum MAP für die Auflistung. Mit dieser Einstellung können Sie [Preisregeln](./pricing-products.md), während Sie gleichzeitig Ihren Mindestpreis für ein Produkt kontrollieren. Wählen Sie ein Preisattribut, das als MAP verwendet werden soll, um zu verhindern, dass der Listenpreis zu niedrig ist. Wenn das ausgewählte Preisfeld jedoch nicht für ein Produkt definiert ist, wird das MAP nicht verwendet.

1. Für **[!UICONTROL Strike Through Price (MSRP)]**, wählen Sie eine Option aus.

   Die Standardeinstellung ist keine Auswahl. Diese Einstellung bestimmt, welches Preisattribut als empfohlener Einzelhandelspreis (MSRP) des Herstellers für ein Produkt verwendet wird. Wenn Ihr Listingpreis unter dem definierten MSRP liegt, wird Ihre Amazon-Liste mit einer Durchsage des MSRP-Preises mit dem niedrigeren Listenpreis sowie dem berechneten Betrag und Prozentsatz &quot;Sie speichern&quot;angezeigt. Wenn das ausgewählte Preisfeld jedoch nicht für ein Produkt definiert ist, wird der MSRP nicht berechnet.

   >[!NOTE]
   >
   >Diese Einstellung gilt nur für Auflistungen, die die [Buy Box](./buy-box-competitor-pricing.md) Position. Die Buy Box wird von Amazon an den Verkäufer verliehen, der das Produkt in der Regel zum besten Preis anbietet, sowie an andere Faktoren wie FBA/Prime-Versand, Verfügbarkeit und Leistung des Verkäufers.

1. Für **Anwendung der Mehrwertsteuer (MwSt.)**, wählen Sie eine Option aus:

   - `Disabled` - (Standard) Wählen Sie aus, wann Sie keine Mehrwertsteuer auf Ihren Listenpreis anwenden möchten.

   - `Enabled` - Wählen Sie aus, wann Sie die Mehrwertsteuer auf Ihren Listenpreis anwenden möchten. Die MwSt wird in der Regel als Umsatzsteuer in europäischen Ländern verwendet und zu Ihrem endgültigen börsennotierten Preis in Amazon hinzugefügt. Die Mehrwertsteuer gilt nicht für den Endpreis von Auflistungen, die im Rahmen einer intelligenten Preisregel verwendet werden, es sei denn, die [Grundpreis](./floor-price.md) wird getroffen.

   >[!NOTE]
   >
   >Die Unternehmen in der Europäischen Union (EU) müssen den kaufenden Unternehmen Rechnungen zuschicken, damit der Kunde die Steuer umsetzen kann. Sie können diese Rechnungen entweder selbst erstellen und die Steuern berechnen oder einen Steuerrechnungs-Service wie den MwSt-Berechnungsdienst von Amazon nutzen. Amazon empfiehlt, sich für die [Amazon - MwSt-Berechnungsservice](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;). Wenn Sie eine andere Methode wählen, sind Sie für die Einhaltung der Mehrwertsteuer verantwortlich.>
   >
   >Es kann 10-14 Tage dauern, bis Amazon Ihr Konto für den MwSt-Berechnungsdienst überprüft und aktiviert.

1. Für **[!UICONTROL VAT Percentage]** Geben Sie den Wert für Ihren Mehrwertsteuersatz ein.

   Der Standardwert ist `0.00`. Dieser Wert wird verwendet, um den Mehrwertsteuerbetrag zu berechnen, der dem Börsennotierungspreis hinzugefügt werden soll. Wenn `10.2` angegeben ist, wird eine 10,20% MwSt auf Ihren Listenpreis erhoben. Dieses Feld ist deaktiviert, wenn das Feld Mehrwertsteuer (MwSt.) auf `Disabled`.

1. **(Nur UK Stores)** Für **[!UICONTROL Amazon Product Tax Code (PTC)]**, wählen Sie eine Option aus:

   - `Do Not Manage PTC` - (Standard) Wählen Sie aus, ob Sie einen Steuerberechnungsdienst eines Drittanbieters verwenden oder bereits alle Ihre Steuerberechnungen in Ihrem [!DNL Amazon Seller Central] -Konto. Wenn ausgewählt, sendet der Amazon-Verkaufskanal keine Informationen zum Produktsteuercode an Ihre [!DNL Amazon Seller Central] -Konto.

   - `Set Default PTC` - Entscheiden Sie, ob Sie einen universellen Produktsteuercode (PTC) haben, den Sie für alle Ihre Produkte verwenden möchten. Wenn diese Option ausgewählt ist, müssen Sie _[!UICONTROL Default PTC]_.

      - Für **[!UICONTROL Default PTC]**, geben Sie den Standard-PTC an, der für alle zulässigen Amazon-Listen verwendet werden soll. Wenn Ihr standardmäßiger PTC in Ihrer [!DNL Amazon Seller Central] -Konto verwenden, lassen Sie dieses Feld leer. Änderungen an diesem Feld wirken sich nicht auf bestehende Amazon-Listen aus. Um den Standard-PTC für eine vorhandene Liste zu ändern, muss die Liste [ended](./end-listings-manually.md) und eine neue Liste erstellt.

   >[!NOTE]
   >
   >Wenn Sie den MwSt-Berechnungsdienst von Amazon verwenden, müssen Sie die Steuerkategorie für Ihre Produkte kennen. Ein PTC ist der Steuerkategorie-ID-Code von Amazon für B2B-Käufe in der EU. Siehe [Amazon-Produktsteuercodes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}.

1. Für **[!UICONTROL Currency Conversion]**, wählen Sie eine Option aus.

   Der Standardwert ist `Disabled`. Diese Optionen hängen von Ihrer [!DNL Commerce] [currency](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) -Einstellungen. Wenn keine Optionen verfügbar sind, richten Sie Ihre Währungseinstellungen ein.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save listing settings]**.

![Listenpreis](assets/amazon-listing-price.png){width="500" zoomable="yes"}

| Feld | Beschreibung |
|---------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Magento Price Source] | Bestimmt die Preisquelle, die bei der Erstellung Ihrer Amazon-Auflistungen verwendet wird. Der Standardwert ist `Price`. Wenn Sie ein anderes Attribut auswählen, z. B. `Amazon Price` oder `Special Price`festgelegt ist, wird der definierte Wert für das Attribut für Ihre Amazon-Auflistung verwendet. Wenn das ausgewählte Attribut jedoch nicht definiert ist, `Price` verwendet. |
| [!UICONTROL Minimum Advertised Price (MAP)] | Die [!DNL Commerce] -Attribut für MAP-Preise. Wenn Sie die MAP-Option auswählen, wird Ihre Amazon-Auflistung automatisch auf den MAP-Preis gesetzt, wenn der Listenpreis unter dem MAP-Preis liegt. |
| [!UICONTROL Strike Through Price (MSRP)] | Die [!DNL Commerce] -Attribut, das die MSRP-Preise darstellt. Wenn Ihr Amazon-Listingpreis unter dem MSRP liegt, wird eine Durchsicht des MSRP-Preises und des Börsennotierungspreises angezeigt. Diese Einstellung wird auch verwendet, um den Betrag und den Prozentsatz für &quot;Sie speichern&quot;zu berechnen. Diese Funktion gilt jedoch nur für Auflistungen, die die [Buy Box](./buy-box-competitor-pricing.md) Position. |
| [!UICONTROL Apply Value Added Tax (VAT)] | Die Mehrwertsteuer wird von Verkäufern in der Europäischen Union verwendet.<br><br>Auswählen `Disabled` wenn Sie nicht möchten, dass die MwSt zu den Preisen hinzugefügt wird.<br><br>Auswählen `Enabled` Geben Sie dann den MwSt.-Prozentsatz für die Anwendung der MwSt. auf Ihre Listenpreise ein. |
| [!UICONTROL VAT Percentage] | Definieren Sie den Prozentsatz, der zur Berechnung des Mehrwertsteuerbetrags verwendet werden soll, der zum Listenpreis für Ihre Amazon-Auflistungen hinzugefügt werden soll. <br><br>Wenn Sie `5`auf den endgültigen Börsennotierungspreis wird eine Mehrwertsteuer von 5 % erhoben, nachdem alle Preisregeln angewandt wurden. Die MwSt.-Steuer gilt nicht für den Endpreis von Auflistungen, die im Rahmen einer intelligenten Preisregel verwendet werden, es sei denn, die [floor](./floor-price.md) oder [ceiling](./optional-ceiling-price.md) wird getroffen. |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Nur für UK Stores angezeigt) Bestimmt, ob der Amazon-Vertriebskanal Produktsteuercode-Informationen an Ihre [!DNL Amazon Seller Central] -Konto. <br><br>Auswählen **PTC nicht verwalten** wenn Sie einen Steuerberechnungsdienst eines Drittanbieters verwenden oder bereits alle Ihre Steuerberechnungen in Ihrem [!DNL Amazon Seller Central] -Konto. Wenn diese Option aktiviert ist, sendet der Amazon-Verkaufskanal keine Informationen zum Produktsteuercode an Ihre [!DNL Amazon Seller Central] -Konto.<br><br>Auswählen **Standard-PTC festlegen** Wenn Sie einen universellen Produktsteuercode haben, den Sie für alle Ihre Produkte verwenden möchten.<br><br>Siehe [Amazon-Produktsteuercodes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}. |
| [!UICONTROL Default PTC] | Nur angezeigt, wenn **Amazon Product Tax Code (PTC)** auf `Set Default PTC`. Geben Sie den Standard-PTC an, der für alle zulässigen Amazon-Listen verwendet werden soll. Wenn Ihr standardmäßiger PTC in Ihrer [!DNL Amazon Seller Central] -Konto verwenden, lassen Sie dieses Feld leer. <br><br>Änderungen an diesem Feld wirken sich nicht auf bestehende Listen aus. Die Auflistung muss [ended](./end-listings-manually.md) und eine neue Liste erstellt, damit die Änderung wirksam wird. |
| [!UICONTROL Currency Conversion] | Ermöglicht Ihnen die [!DNL Commerce] storefront die Standardwährung, um eine genaue Konversion in Ihre Amazon-Standardwährung vorzunehmen und Ihre Listenpreise in der entsprechenden Währung zu veröffentlichen. Die Währungsumrechnung basiert immer auf Ihrer [!DNL Commerce] Standardwährung.<br><br>Sie können Ihre Standardeinstellung weiterhin anzeigen [!DNL Commerce] und Amazon-Währungen, wenn andere Währungen verfügbar sind. Wenn die Standardeinstellung [!DNL Commerce] Die Währung entspricht der Amazon-Standardwährung, lassen Sie die Währungsumrechnung deaktiviert.<br><br>Wenn beispielsweise Ihre [!DNL Commerce] Standardwährung ist CAD (kanadischer Dollar) und Ihre Amazon-Standardwährung ist USD. Sie müssen die Währungsumrechnung aktivieren und die Konversionsrate CAD auf USD wählen. Die angezeigten Optionen basieren auf dem integrierten [!DNL Commerce] Währungsumrechnungen. Wenn die gewünschte Option nicht angezeigt wird, [die Währung in [!DNL Commerce]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html). |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
