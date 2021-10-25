---
title: Listingpreis
description: Verwenden Sie die Listenpreiseinstellungen, um die Preisquelle und den Basiswert (Standard) für Ihre Amazon-Auflistungen zu bestimmen.
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# Listingpreis

[!UICONTROL Listing Price] -Einstellungen Teil Ihrer Einstellungen für die Ladenliste sind. Auf die Listseinstellungen kann über folgende Optionen zugegriffen werden: [Dashboard speichern](./amazon-store-dashboard.md).

Diese Einstellungen definieren [!DNL Commerce] das Preisattribut, das als Ihre Preisquelle verwendet wird, der Grundpreis (Standard) für Ihre Amazon-Auflistungen. Diese Einstellungen werden von Ihren [Preisregeln](./pricing-rule-general-settings.md) um den Amazon-Listingpreis automatisch an den festgelegten Wert anzupassen für _[!UICONTROL Magento Price Source]_.

Sie können [Preisgestaltung](./price-scope.md) als global oder website. Wenn Ihr Preisbereich auf `Global`, gibt es eine einzige Preisquelle für alle Ihre Läden/Websites. Wenn Ihr Preisbereich auf `Website`verwendet die Preisquelle die Fallback-Logik des Website-Preises (falls verfügbar) gefolgt vom Standard-Preis (Global).

Wenn eine Listungsregel für mehr als eine Website gilt, wird die Reihenfolge, in der der Websitepreis verwendet wird, durch die Prioritätseinstellung der Website bestimmt, die in der [Listungsregel](./listing-rules.md). Diese Regeln ermöglichen es Ihnen, die Produktpreise im gesamten Katalog zu definieren. Informationen dazu, ob Sie den Websitepreisbereich verwenden, finden Sie unter [Katalogpreisumfang](https://docs.magento.com/user-guide/catalog/catalog-price-scope.html){Zielgruppe=&quot;_blank&quot;}.

Die in _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_ und _[!UICONTROL Strike Through Price (MSRP)]_enthalten die konfigurierten Preisattribute. Preisattribute sind [!DNL Commerce] Produktattribute, bei denen der Katalogeingabetyp für den Store-Eigentümer auf `Price`. Siehe [Attributeingabetypen](https://docs.magento.com/user-guide/stores/attributes-input-types.html){Zielgruppe=&quot;_blank&quot;}.

## Listungspreiseinstellungen konfigurieren {#configure-listing-price-settings}

1. Klick **[!UICONTROL Listing Settings]** auf dem Dashboard.

1. Erweitern der _[!UICONTROL Listing Price]_Abschnitt.

1. für **[!UICONTROL Magento Price Source]** (erforderlich), wählen Sie eine Option aus.

   Der Standardwert ist `Price`. Diese Einstellung bestimmt die Preisquelle für Ihre Amazon-Auflistungen. Wenn Sie [Preisregeln](./pricing-products.md), werden die Regeln auf den Wert angewendet, der für das hier ausgewählte Attribut definiert ist. Sie können jedes konfigurierte Preisattribut auswählen. Wenn das ausgewählte Attribut jedoch nicht für ein Produkt ausgefüllt wird, wird die Preisquelle für das Produkt standardmäßig auf `Price` bei Anwendung der Preisregeln zur Bestimmung des veröffentlichten Amazon-Notierungspreises.

1. für **[!UICONTROL Minimum Advertised Price (MAP)**], wählen Sie eine Option aus.

   Der Standardwert ist keine Auswahl. Diese Einstellung ermöglicht einen Mindestpreis (MAP) für ein Produkt. Wenn Sie ein Preisattribut definieren und Ihr Börsennotierungspreis für ein Produkt unter den festgelegten Mindestpreis fällt (basierend auf Ihrer Preisquelle und Ihren Regeln), wird dieser Wert zum MAP für die Auflistung. Mit dieser Einstellung können Sie Folgendes implementieren: [Preisregeln](./pricing-products.md), während Sie Ihren Mindestpreis für ein Produkt steuern. Um zu verhindern, dass ein Listenpreis zu niedrig ist, wählen Sie ein Preisattribut, das als MAP verwendet werden soll. Wenn das ausgewählte Preisfeld jedoch nicht für ein Produkt definiert ist, wird das MAP nicht verwendet.

1. für **[!UICONTROL Strike Through Price (MSRP)]**, wählen Sie eine Option aus.

   Der Standardwert ist keine Auswahl. Mit dieser Einstellung wird festgelegt, welches Preisattribut als vom Hersteller vorgeschlagener Einzelhandelspreis (MSRP) für ein Produkt verwendet wird. Wenn Ihr Börsennotierungspreis unter dem festgelegten MSRP liegt, wird Ihre Amazon-Auflistung mit einem Durchstreichen des MSRP-Preises mit dem niedrigeren Listenpreis sowie dem errechneten Betrag und Prozentsatz angezeigt. Wenn jedoch das ausgewählte Preisfeld für ein Produkt nicht definiert ist, wird der MSRP nicht berechnet.

   >[!NOTE]
   >
   >Diese Einstellung gilt nur für Auflistungen, die die [Buy Box](./buy-box-competitor-pricing.md) Position. Die Buy Box wird von Amazon an den Verkäufer verliehen, der das Produkt üblicherweise zum günstigsten Preis anbietet, sowie an andere Faktoren wie die angebotene FBA/Prime-Lieferung, die Verfügbarkeit und die Leistung des Verkäufers.

1. für **Mehrwertsteuer (MwSt) anwenden**, wählen Sie eine Option aus:

   - `Disabled` - (Standard) Wählen Sie aus, wenn Sie keine Mehrwertsteuer auf Ihren Börsenkurs anwenden möchten.

   - `Enabled` - Wählen Sie aus, wann Sie die MwSt auf Ihren Listenpreis anwenden möchten. Die MwSt wird in der Regel als Verkaufssteuer in europäischen Ländern verwendet und wird zu Ihrem endgültigen, börsennotierten Preis in Amazon addiert. Die Mehrwertsteuer gilt nicht für den Endpreis von Auflistungen, die innerhalb einer intelligenten Preisregel verwendet werden, es sei denn, die [Tiefstpreis](./floor-price.md) ist getroffen.
   >[!NOTE]
   >
   >Die Unternehmen in der Europäischen Vereinigung (EU) müssen den Käufern Rechnungen zukommen lassen, damit der Kunde die Steuer abgeben kann. Sie können diese Rechnungen entweder selbst erstellen und die Steuern selbst berechnen oder einen Steuerberechnungsdienst wie den Mehrwertsteuerberechnungsdienst von Amazon nutzen. Amazon empfiehlt, sich für die [MwSt-Berechnungsservice Amazon](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;){Zielgruppe=&quot;_blank&quot;}. Wenn Sie eine andere Methode wählen, sind Sie für die Einhaltung der Mehrwertsteuer verantwortlich.>
   >
   >Es kann 10-14 Tage dauern, bis Amazon Ihr MwSt.-Berechnungsservice-Konto überprüft und aktiviert.

1. für **[!UICONTROL VAT Percentage]**, geben Sie den Wert für Ihren Mehrwertsteuersatz ein.

   Der Standardwert ist `0.00`. Dieser Wert wird verwendet, um den MwSt.-Betrag zu berechnen, der dem Börsenkurs hinzuzufügen ist. Falls `10.2` wird eine 10,20% MwSt auf Ihren Börsenpreis erhoben. Dieses Feld ist deaktiviert, wenn das Feld Mehrwertsteuer (MwSt.) auf `Disabled`.

1. **(Nur britische Geschäfte)** für **[!UICONTROL Amazon Product Tax Code (PTC)]**, wählen Sie eine Option aus:

   - `Do Not Manage PTC` - (Standard) Wählen Sie aus, ob Sie einen Steuerberechnungsdienst eines Drittanbieters verwenden oder bereits alle Ihre Steuerberechnungen in Ihren [!DNL Amazon Seller Central] Konto. Wenn Sie diese Option wählen, sendet Amazon Sales Kanal keine Produktsteuercode-Informationen an Ihre [!DNL Amazon Seller Central] Konto.

   - `Set Default PTC` - Wählen Sie aus, ob Sie einen universellen Produktsteuercode (PTC) für all Ihre Produkte verwenden möchten. Wenn ausgewählt, müssen Sie _[!UICONTROL Default PTC]_.

      - für **[!UICONTROL Default PTC]**, geben Sie den Standard-PTC ein, der für alle zugelassenen Amazon-Listen verwendet werden soll. Wenn Ihr Standard-PTC in Ihrem [!DNL Amazon Seller Central] Konto, lassen Sie dieses Feld leer. Änderungen in diesem Feld haben keine Auswirkungen auf bestehende Amazon-Listen. Um die Standard-PTC für eine vorhandene Auflistung zu ändern, muss die Liste [beendet](./end-listings-manually.md) und eine neue Liste erstellt.
   >[!NOTE]
   >
   >Wenn Sie den MwSt.-Berechnungsservice von Amazon nutzen, müssen Sie die Kategorie für Ihre Produkte kennen. Ein PTC ist der Amazon-Code für Kategorien-ID für B2B-Einkäufe in der EU. Siehe [Amazon-Produktsteuercodes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){Zielgruppe=&quot;_blank&quot;}.

1. für **[!UICONTROL Currency Conversion]**, wählen Sie eine Option aus.

   Der Standardwert ist `Disabled`. Diese Optionen hängen von Ihren [!DNL Commerce] [Währung](https://docs.magento.com/user-guide/configuration/general/currency-setup.html)Einstellungen für {Zielgruppe=&quot;_blank&quot;}. Wenn keine Optionen verfügbar sind, legen Sie Ihre Währungseinstellungen fest.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Listingpreis](assets/amazon-listing-price.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Magento Price Source] | Bestimmt die Preisquelle, die bei der Erstellung Ihrer Amazon-Auflistungen verwendet wird. Der Standardwert ist `Price`. Wenn Sie ein anderes Attribut auswählen, z. B. `Amazon Price` oder `Special Price`, wird der definierte Wert für das Attribut für Ihre Amazon-Auflistung verwendet. Wenn das ausgewählte Attribut jedoch nicht definiert ist, `Price` wird verwendet. |
| [!UICONTROL Minimum Advertised Price (MAP)] | Die [!DNL Commerce] Attribut für MAP-Preise. Wenn Sie die MAP-Option wählen, wird Ihre Amazon-Auflistung automatisch auf den MAP-Preis gesetzt, wenn der Listenpreis unter dem MAP-Preis liegt. |
| [!UICONTROL Strike Through Price (MSRP)] | Die [!DNL Commerce] Attribut, das die MSRP-Preise darstellt. Wenn Ihr Amazon-Börsennotierungspreis unter dem MSRP liegt, wird ein Durchstreichen des MSRP-Preises und des Börsennotierungspreises angezeigt. Diese Einstellung wird auch verwendet, um den Betrag und den Prozentsatz für &quot;Speichern&quot;zu berechnen. Diese Funktion gilt jedoch nur für Auflistungen, die die [Buy Box](./buy-box-competitor-pricing.md) Position. |
| [!UICONTROL Apply Value Added Tax (VAT)] | Die Mehrwertsteuer wird von Verkäufern in der Europäischen Vereinigung verwendet.<br><br>Auswählen `Disabled` wenn Sie nicht möchten, dass die MwSt. zu den Preisen addiert wird.<br><br>Auswählen `Enabled` und geben Sie dann den MwSt-Prozentsatz für die Anwendung der MwSt auf Ihre Notierungspreise ein. |
| [!UICONTROL VAT Percentage] | Geben Sie den Prozentsatz an, der zur Berechnung des MwSt.-Betrags verwendet werden soll, der dem Börsennotierungspreis für Ihre Amazon-Auflistungen hinzuzufügen ist. <br><br>Wenn Sie `5`, wird eine Mehrwertsteuer von 5 % auf den endgültigen Notierungspreis erhoben, nachdem alle Preisregeln angewandt wurden. Die Mehrwertsteuer gilt nicht für den Endpreis von Auflistungen, die innerhalb einer intelligenten Preisregel verwendet werden, es sei denn, die [Fußboden](./floor-price.md) oder [Obergrenze](./optional-ceiling-price.md) ist getroffen. |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (Nur für britische Geschäfte angezeigt) Bestimmt, ob der Amazon-Kanal Produktsteuercodeninformationen an Ihre [!DNL Amazon Seller Central] Konto. <br><br>Auswählen **PTC nicht verwalten** wenn Sie einen Steuerberechnungsdienst eines Drittanbieters verwenden oder bereits alle Ihre Steuerberechnungen in Ihren [!DNL Amazon Seller Central] Konto. Wenn diese Option aktiviert ist, sendet Amazon Sales Kanal keine Produktemodellinformationen an Ihre [!DNL Amazon Seller Central] Konto.<br><br>Auswählen **Standard-PTC festlegen** wenn Sie einen universellen Produktsteuercode haben, den Sie für all Ihre Produkte verwenden möchten.<br><br>Siehe [Amazon-Produktsteuercodes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){Zielgruppe=&quot;_blank&quot;}. |
| [!UICONTROL Default PTC] | Wird nur angezeigt, wenn **Amazon Product Tax Code (PTC)** ist eingestellt auf `Set Default PTC`. Geben Sie den Standard-PTC ein, der für alle zulässigen Amazon-Auflistungen verwendet werden soll. Wenn Ihr Standard-PTC in Ihrem [!DNL Amazon Seller Central] Konto, lassen Sie dieses Feld leer. <br><br>Änderungen in diesem Feld haben keine Auswirkungen auf vorhandene Listen. Die Auflistung muss [beendet](./end-listings-manually.md) und eine neue Liste erstellt, damit die Änderung wirksam wird. |
| [!UICONTROL Currency Conversion] | Ermöglicht es Ihrem [!DNL Commerce] speichern Sie die Standardwährung, um Ihre Listenpreise in der richtigen Währung in Ihre Amazon-Standardwährung zu konvertieren. Die Währungsumrechnung basiert immer auf Ihrer [!DNL Commerce] Standardwährung.<br><br>Sie können Ihre Standardeinstellung weiterhin Ansicht [!DNL Commerce] und Amazon-Währungen, wenn andere Währungen verfügbar sind. Wenn Ihre Standardeinstellung [!DNL Commerce] Die Währung stimmt mit Ihrer Amazon-Standardwährung überein, lassen Sie die Währungsumrechnung deaktiviert.<br><br>Wenn z. B. [!DNL Commerce] Die Standardwährung ist CAD (Kanadische Dollar) und Ihre Amazon Standardwährung ist USD. Sie müssen die Währungsumrechnung aktivieren und die Konversionsrat-CAD-Option auf USD auswählen. Die angebotenen Optionen basieren auf dem integrierten [!DNL Commerce] Währungsumrechnungen. Wenn Sie die von Ihnen gesuchte Option nicht sehen, [die Währung in [!DNL Commerce]](https://docs.magento.com/user-guide/stores/currency-configuration.html){Zielgruppe=&quot;_blank&quot;}. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
