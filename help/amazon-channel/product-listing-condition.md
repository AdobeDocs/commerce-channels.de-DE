---
title: Produktlistenbedingung
description: Verwenden Sie die Einstellungen für die Produktlisten-Bedingung, um Ihre Commerce-Produkte einer Amazon-Produktbedingung zuzuordnen, z. B. "Neu"oder "Neu"oder "Raffiniert".
redirect_from: /sales-channels/asc/ob-product-listing-condition.html
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Bedingung für die Produktliste

Die Bedingungseinstellungen für die Produktliste sind Teil Ihrer Einstellungen für die Store-Auflistung. Sie können auf die Listeneinstellungen im [Store-Dashboard](./amazon-store-dashboard.md).

Amazon erfordert eine Produktliste, die eine definierte Bedingung aufweist. Wenn alle Ihre Produkte dieselbe Bedingung aufweisen, können Sie eine der Amazon-Bedingungsoptionen auswählen, um alle Ihre Produkte als Ihren globalen Bedingungswert darzustellen. Zu den standardmäßigen Amazon-Bedingungen gehören:

- `New`
- `Refurbished`
- `Used; Like New`
- `Used; Very Good`
- `Used; Good`
- `Used; Acceptable`
- `Collectible; Like New`
- `Collectible; Very Good`
- `Collectible; Good`
- `Collectible; Acceptable`

>[!IMPORTANT]
>
>Wenn Sie erneuerte (renovierte) Produkte verkaufen, müssen Sie sich bei der [!DNL Amazon Renewed Program]. Siehe [Erneuerte Produkte](./renewed-products.md).

Wenn Ihr Katalog jedoch Produkte mit unterschiedlichen Bedingungen enthält (z. B. Neu, Verwendet und Überarbeitet), müssen Sie zwischen **[!UICONTROL Assign Condition Using Product Attribute]**. Mit dieser Einstellung können Sie Ihre [!DNL Commerce] Bedingungsattribut und -werte zu den Bedingungen in Ihrer Amazon-Auflistung hinzufügen.

Während [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md)wird empfohlen, eine [!DNL Commerce] Produktattribut für die Bedingung eines Produkts. Wenn Sie Produkte unter verschiedenen Bedingungen anbieten und kein Bedingungsattribut erstellt haben, lesen Sie [Erstellen Sie ein Produktattribut in [!DNL Commerce]](./ob-creating-magento-attributes.md). Nachdem das Bedingungsattribut erstellt wurde, können Sie jedem Ihrer Produkte in Ihrer [!DNL Commerce] Katalog.

## Einstellungen konfigurieren

1. Klicken **[!UICONTROL Listing Settings]** im Dashboard speichern.

1. Erweitern Sie die **[!UICONTROL Product Listing Condition]** Abschnitt.

1. Für **[!UICONTROL Listing Product Condition]**, wählen Sie eine Option aus.

   Wählen Sie eine der standardmäßigen Amazon-Bedingungen für Ihren globalen Bedingungswert für alle Ihre Auflistungen aus. Die Standardeinstellung ist `New`.

   Wenn Sie Produkte/Listen mit unterschiedlichen Bedingungen haben, wählen Sie `Assign Condition Using Product Attribute` , um die Einstellungen für die Produktbedingungen in den zusätzlichen angezeigten Feldern zu definieren.

1. Für **Bedingungsattribut**, wählen Sie die [!DNL Commerce] -Attribut, um Werte für die einzelnen standardmäßigen Amazon-Bedingungsattribute zuzuordnen.

   Wenn Sie Produkte im `Used` oder `Collectible` -Bedingung, Sie unterscheiden jedoch nicht weiter, können Sie einer einzelnen `Used` oder `Collectible` Amazon-Bedingung verwenden und die anderen leer lassen. Diese Methode ordnet alle Ihre `Used` oder `Collectible` Bedingungen für die einzelne verwendete oder kollektive Amazon-Bedingung.

   Sie haben beispielsweise eine `Used` für Ihre Produkte. Bei der Zuordnung wählen Sie aus, ob Sie der Amazon-Bedingung zuordnen möchten `Used; Like New`, `Used; Very Good`, `Used; Good`oder `Used; Acceptable`. Füllen Sie nur das Feld für die gewünschte Amazon-Bedingung aus, wobei die andere `Used` Optionen festgelegt auf `--Select Option--`. Im Beispielbild werden alle [!DNL Commerce] in `Used` -Bedingung der Amazon zugeordnet werden. `Used; Very Good` Bedingung.

   Sie können auch beschreibenden Text für Ihre Bedingungen eingeben, außer `New`.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save listing settings]**.

![Bedingung für die Produktliste](assets/amazon-product-listing-condition.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Listing Product Condition] | Die Bedingung Ihrer Produktlisten. Optionen: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Wenn Sie eine einzige Produktbedingung verkaufen, wählen Sie eine der standardmäßigen Amazon-Bedingungen. Wenn [!DNL Commerce] Der Katalog enthält Produkte unter verschiedenen Bedingungen, wählen Sie `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | Die [!DNL Commerce] -Attribut, das die Bedingung für Ihre Produkte definiert. Wählen Sie das von Ihnen erstellte Attribut Magneto aus, um es dem Amazon-Bedingungsattribut zuzuordnen. Im [Beispiel für Aufgaben vor der Einrichtung](./ob-creating-magento-attributes.md) empfiehlt die Benennung als `Amazon Condition`. Wenn diese Option ausgewählt ist, werden zusätzliche Felder für die Zuordnung der standardmäßigen Amazon-Bedingungen angezeigt. |
| [!UICONTROL Additional Condition fields] | Wählen Sie für jede der standardmäßigen Amazon-Bedingungen die entsprechende Bedingung aus. Die Optionen sind die Bedingungsbeschriftungen, die Sie bei der [Amazon-Bedingungsattribut erstellt haben](./ob-creating-magento-attributes.md).<br><br>Wenn Sie Produkte im `Used` oder `Collectible` -Bedingung, Sie unterscheiden jedoch nicht weiter, können Sie einer einzelnen `Used` oder `Collectible` Amazon-Bedingung verwenden und die anderen leer lassen. Diese Methode ordnet alle `Used` oder `Collectible` Bedingungen für die einzelne verwendete oder kollektive Amazon-Bedingung. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
