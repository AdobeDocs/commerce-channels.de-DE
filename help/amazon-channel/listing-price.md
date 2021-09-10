---
title: Listenpreis
description: 'Verwenden Sie die Einstellungen für den Listenpreis , um die Preisquelle und den Basiswert (Standard) für Ihre Amazon-Auflistungen zu bestimmen.'
redirect_from: /sales-channels/asc/ob-listing-price.html: 
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 1509
ht-degree: 0%

---

# Listenpreis

[!UICONTROL Listing Price] -Einstellungen sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über das [Store-Dashboard](./amazon-store-dashboard.md) zugegriffen werden.

Diese Einstellungen definieren, welches [!DNL Commerce] Preisattribut als Ihre Preisquelle verwendet werden soll, was der (standardmäßige) Basispreiswert für Ihre Amazon-Auflistungen ist. Diese Einstellungen werden von Ihren [Preisregeln](./pricing-rule-general-settings.md) verwendet, um Ihren Amazon-Listenpreis automatisch an den für _[!UICONTROL Magento Price Source]_festgelegten Wert anzupassen.

Sie können Ihren [Preisbereich](./price-scope.md) als globale oder Website konfigurieren. Wenn Ihr Preisbereich auf `Global` festgelegt ist, gibt es eine einzige Preisquelle für alle Ihre Geschäfte/Websites. Wenn Ihr Preisbereich auf `Website` festgelegt ist, verwendet die Preisquelle die Ausweichlogik des Website-Preises (sofern verfügbar) gefolgt vom standardmäßigen (globalen) Preis.

Wenn eine Listening-Regel auf mehr als eine Website angewendet wird, wird die Reihenfolge, in der der Website-Preis verwendet wird, durch die in der [Listening-Regel](./listing-rules.md) definierte Website-Priorität bestimmt. Mit diesen Regeln können Sie die Produktpreise in Ihrem Katalog definieren. Informationen dazu, ob Sie den Umfang des Website-Preises verwenden, finden Sie unter [Catalog Price Scope](https://docs.magento.com/user-guide/catalog/catalog-price-scope.html){target=&quot;_blank&quot;}.

Die unter _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_ und _[!UICONTROL Strike Through Price (MSRP)]_aufgeführten Optionen enthalten Ihre konfigurierten Preisattribute. Preisattribute sind [!DNL Commerce] -Produktattribute, bei denen der Wert für &quot;Catalog Input Type for Store Owner&quot;auf `Price` gesetzt ist. Siehe [Attributeingabetypen](https://docs.magento.com/user-guide/stores/attributes-input-types.html){target=&quot;_blank&quot;}.

## Einstellungen für den Listenpreis konfigurieren {#configure-listing-price-settings}

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt _[!UICONTROL Listing Price]_.

1. Wählen Sie für **[!UICONTROL Magento Price Source]** (erforderlich) eine Option aus.

   Der Standardwert ist `Price`. Diese Einstellung bestimmt die Preisquelle, die für Ihre Amazon-Auflistungen verwendet wird. Wenn Sie [Preisregeln](./pricing-products.md) erstellen, werden die Regeln auf den Wert angewendet, der für das hier ausgewählte Attribut definiert ist. Sie können jedes konfigurierte Preisattribut auswählen. Wenn das ausgewählte Attribut jedoch nicht für ein Produkt ausgefüllt wird, wird als Preisquelle für das Produkt bei Anwendung der Preisregeln zur Bestimmung des veröffentlichten Amazon-Listenpreises standardmäßig `Price` verwendet.

1. Wählen Sie für **[!UICONTROL Minimum Advertised Price (MAP)**] eine Option aus.

   Die Standardeinstellung ist keine Auswahl. Diese Einstellung ermöglicht einen mindestens beworbenen Preis (MAP) für ein Produkt. Wenn Sie ein Preisattribut definieren und Ihr Börsennotierungspreis für ein Produkt unter den festgelegten Mindestpreis fällt (basierend auf Ihrer Preisquelle und Ihren Regeln), wird dieser Wert zum MAP für die Auflistung. Mit dieser Einstellung können Sie [Preisregeln](./pricing-products.md) implementieren und gleichzeitig Ihren Mindestpreis für ein Produkt steuern. Wählen Sie ein Preisattribut, das als MAP verwendet werden soll, um zu verhindern, dass der Listenpreis zu niedrig ist. Wenn das ausgewählte Preisfeld jedoch nicht für ein Produkt definiert ist, wird das MAP nicht verwendet.

1. Wählen Sie für **[!UICONTROL Strike Through Price (MSRP)]** eine Option aus.

   Die Standardeinstellung ist keine Auswahl. Diese Einstellung bestimmt, welches Preisattribut als empfohlener Einzelhandelspreis (MSRP) des Herstellers für ein Produkt verwendet wird. Wenn Ihr Listingpreis unter dem definierten MSRP liegt, wird Ihre Amazon-Liste mit einer Durchsage des MSRP-Preises mit dem niedrigeren Listenpreis sowie dem berechneten Betrag und Prozentsatz &quot;Sie speichern&quot;angezeigt. Wenn das ausgewählte Preisfeld jedoch nicht für ein Produkt definiert ist, wird der MSRP nicht berechnet.

   >[!NOTE]
   >
   >Diese Einstellung gilt nur für Auflistungen, die die Position [Buy Box](./buy-box-competitor-pricing.md) gewonnen haben. Die Buy Box wird von Amazon an den Verkäufer verliehen, der das Produkt in der Regel zum besten Preis anbietet, sowie an andere Faktoren wie FBA/Prime-Versand, Verfügbarkeit und Leistung des Verkäufers.

1. Wählen Sie für **Mehrwertsteuer (MwSt)** anwenden eine Option:

   - `Disabled` - (Standard) Wählen Sie aus, wann Sie keine Mehrwertsteuer auf Ihren Listenpreis anwenden möchten.

   - `Enabled` - Wählen Sie aus, wann Sie die Mehrwertsteuer auf Ihren Listenpreis anwenden möchten. Die MwSt wird in der Regel als Umsatzsteuer in europäischen Ländern verwendet und zu Ihrem endgültigen börsennotierten Preis in Amazon hinzugefügt. Die Mehrwertsteuer gilt nicht für den Endpreis von Auflistungen, die innerhalb einer intelligenten Preisregel verwendet werden, es sei denn, der [Grundpreis](./floor-price.md) wird erreicht.
   >[!NOTE]
   >
   >Die Unternehmen in der Europäischen Union (EU) müssen den kaufenden Unternehmen Rechnungen zuschicken, damit der Kunde die Steuer umsetzen kann. Sie können diese Rechnungen entweder selbst erstellen und die Steuern berechnen oder einen Steuerrechnungs-Service wie den MwSt-Berechnungsdienst von Amazon nutzen. Amazon empfiehlt, sich für den [Amazon-Mehrwertsteuerberechnungsdienst](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;){target=&quot;_blank&quot;} anzumelden. Wenn Sie eine andere Methode wählen, sind Sie für die Einhaltung der Mehrwertsteuer verantwortlich.>
   >
   >Es kann 10-14 Tage dauern, bis Amazon Ihr Konto für den MwSt-Berechnungsdienst überprüft und aktiviert.

1. Geben Sie für **[!UICONTROL VAT Percentage]** den Wert für Ihren Mehrwertsteuersatz ein.

   Der Standardwert ist `0.00`. Dieser Wert wird verwendet, um den Mehrwertsteuerbetrag zu berechnen, der dem Börsennotierungspreis hinzugefügt werden soll. Wenn `10.2` eingegeben wird, wird eine 10,20% Mehrwertsteuer auf Ihren Börsennotierungspreis erhoben. Dieses Feld ist deaktiviert, wenn das Feld Mehrwertsteuer (MwSt.) auf `Disabled` gesetzt ist.

1. **(Nur UK Stores)** Wählen Sie  **[!UICONTROL Amazon Product Tax Code (PTC)]** eine Option:

   - `Do Not Manage PTC` - (Standard) Wählen Sie aus, ob Sie einen Steuerberechnungsdienst eines Drittanbieters verwenden oder bereits alle Ihre Steuerberechnungen in Ihrem  [!DNL Amazon Seller Central] Konto eingerichtet haben. Wenn diese Option aktiviert ist, sendet der Amazon-Verkaufskanal keine Informationen zum Produktsteuercode an Ihr [!DNL Amazon Seller Central]-Konto.

   - `Set Default PTC` - Entscheiden Sie, ob Sie einen universellen Produktsteuercode (PTC) haben, den Sie für alle Ihre Produkte verwenden möchten. Wenn ausgewählt, müssen Sie _[!UICONTROL Default PTC]_ausfüllen.

      - Geben Sie für **[!UICONTROL Default PTC]** den Standard-PTC ein, der für alle zulässigen Amazon-Listen verwendet werden soll. Wenn Ihr Standard-PTC in Ihrem [!DNL Amazon Seller Central]-Konto festgelegt ist, lassen Sie dieses Feld leer. Änderungen an diesem Feld wirken sich nicht auf bestehende Amazon-Listen aus. Um die Standard-PTC für eine bestehende Liste zu ändern, muss die Auflistung [ended](./end-listings-manually.md) lauten und eine neue Liste erstellt werden.
   >[!NOTE]
   >
   >Wenn Sie den MwSt-Berechnungsdienst von Amazon verwenden, müssen Sie die Steuerkategorie für Ihre Produkte kennen. Ein PTC ist der Steuerkategorie-ID-Code von Amazon für B2B-Käufe in der EU. Siehe [Amazons Produktsteuercodes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}.

1. Wählen Sie für **[!UICONTROL Currency Conversion]** eine Option aus.

   Der Standardwert ist `Disabled`. Diese Optionen hängen von Ihren [!DNL Commerce] [Währung](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;} Einstellungen ab. Wenn keine Optionen verfügbar sind, richten Sie Ihre Währungseinstellungen ein.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Listenpreis](assets/amazon-listing-price.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Magento Price Source] | Bestimmt die Preisquelle, die bei der Erstellung Ihrer Amazon-Auflistungen verwendet wird. Der Standardwert ist `Price`. Wenn Sie ein anderes Attribut auswählen, z. B. `Amazon Price` oder `Special Price`, wird der definierte Wert für das Attribut für Ihre Amazon-Auflistung verwendet. Wenn das ausgewählte Attribut jedoch nicht definiert ist, wird `Price` verwendet. |
| [!UICONTROL Minimum Advertised Price (MAP)] | Das [!DNL Commerce]-Attribut für MAP-Preise. Wenn Sie die MAP-Option auswählen, wird Ihre Amazon-Auflistung automatisch auf den MAP-Preis gesetzt, wenn der Listenpreis unter dem MAP-Preis liegt. |
| [!UICONTROL Strike Through Price (MSRP)] | Das [!DNL Commerce]-Attribut, das die MSRP-Preise darstellt. Wenn Ihr Amazon-Listingpreis unter dem MSRP liegt, wird eine Durchsicht des MSRP-Preises und des Börsennotierungspreises angezeigt. Diese Einstellung wird auch verwendet, um die Menge und den Prozentsatz &quot;Sie speichern&quot;zu berechnen. Diese Funktion gilt jedoch nur für Auflistungen, die die Position [Buy Box](./buy-box-competitor-pricing.md) gewonnen haben. |
| [!UICONTROL Apply Value Added Tax (VAT)] | Die Mehrwertsteuer wird von Verkäufern in der Europäischen Union verwendet.<br><br>Entscheiden Sie,  `Disabled` ob Sie keine Mehrwertsteuer auf die Preisliste hinzufügen möchten.<br><br>Wählen Sie  `Enabled` und geben Sie dann den MwSt.-Prozentsatz für Ihre Listenpreise an. |
| [!UICONTROL VAT Percentage] | Definieren Sie den Prozentsatz, der zur Berechnung des Mehrwertsteuerbetrags verwendet werden soll, der zum Listenpreis für Ihre Amazon-Auflistungen hinzugefügt werden soll. <br><br>Wenn Sie eintragen,  `5`wird eine 5% MwSt auf den endgültigen Börsennotierungspreis angewendet, nachdem alle Preisregeln angewendet wurden. Die MwSt.-Steuer gilt nicht für den Endpreis von Auflistungen, die im Rahmen einer intelligenten Preisregel verwendet werden, es sei denn, der Wert [floor](./floor-price.md) oder [ceiling](./optional-ceiling-price.md) wird erreicht. |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Wird nur für UK Stores angezeigt) Bestimmt, ob der Amazon-Verkaufskanal Produktsteuercode-Informationen an Ihr [!DNL Amazon Seller Central]-Konto sendet. <br><br>Wählen Sie  **Nicht** PTC verwalten aus, wenn Sie einen Steuerberechnungsdienst eines Drittanbieters verwenden oder bereits alle Ihre Steuerberechnungen in Ihrem  [!DNL Amazon Seller Central] Konto eingerichtet haben. Wenn diese Option aktiviert ist, sendet der Amazon-Verkaufskanal keine Informationen zum Produktsteuercode an Ihr [!DNL Amazon Seller Central]-Konto.<br><br>Wählen Sie  **Standard-** PTC festlegen aus, wenn Sie einen universellen Produktsteuercode haben, den Sie für alle Ihre Produkte verwenden möchten.<br><br>Siehe  [Amazon-Produktsteuercodes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}. |
| [!UICONTROL Default PTC] | Wird nur angezeigt, wenn **Amazon Product Tax Code (PTC)** auf `Set Default PTC` gesetzt ist. Geben Sie den Standard-PTC an, der für alle zulässigen Amazon-Listen verwendet werden soll. Wenn Ihr Standard-PTC in Ihrem [!DNL Amazon Seller Central]-Konto festgelegt ist, lassen Sie dieses Feld leer. <br><br>Änderungen an diesem Feld wirken sich nicht auf bestehende Listen aus. Die Liste muss [ended](./end-listings-manually.md) lauten und eine neue Liste erstellt werden, damit die Änderung wirksam wird. |
| [!UICONTROL Currency Conversion] | Ermöglicht es Ihrer Standardwährung [!DNL Commerce], Ihre Listenpreise in der richtigen Währung in Ihre Amazon-Standardwährung umzurechnen. Die Währungsumrechnung basiert immer auf Ihrer [!DNL Commerce] Standardwährung.<br><br>Sie können Ihre Standard-  [!DNL Commerce] und Amazon-Währungen weiterhin anzeigen, wenn andere Währungen verfügbar sind. Wenn Ihre Standardwährung [!DNL Commerce] mit Ihrer Standardwährung in Amazon übereinstimmt, lassen Sie die Währungsumrechnung deaktiviert.<br><br>Wenn Ihre  [!DNL Commerce] Standardwährung beispielsweise CAD (Kanadischer Dollar) ist und Ihre Amazon-Standardwährung USD ist, müssen Sie die Währungsumrechnung aktivieren und die Konversionsrate CAD auf USD festlegen. Die angezeigten Optionen basieren auf den integrierten [!DNL Commerce] Währungsumrechnungen. Wenn die gewünschte Option nicht angezeigt wird, richten Sie die Währung in [a [!DNL Commerce]](https://docs.magento.com/user-guide/stores/currency-configuration.html){target=&quot;_blank&quot;} ein. |

**Schnellzugriff**  -  [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
