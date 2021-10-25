---
title: Produktauflistungsbedingung
description: Verwenden Sie die Einstellungen für die Produktauflistungsbedingung, um Ihre Commerce-Produkte einer Amazon-Produktbedingung zuzuordnen, z. B. "Neu" oder "Neu".
redirect_from: /sales-channels/asc/ob-product-listing-condition.html
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Produktlistungsbedingung

Die Einstellungen für die Produktlistungsbedingung sind Teil Ihrer Einstellungen für die Ladenliste. Sie können auf die Listeneinstellungen auf der [Dashboard speichern](./amazon-store-dashboard.md).

Amazon benötigt eine Produktliste, um eine definierte Bedingung zu haben. Wenn alle Ihre Produkte gleich sind, können Sie eine der Amazon-Bedingungsoptionen auswählen, um alle Ihre Produkte als Ihren globalen Bedingungswert darzustellen. Die Amazon-Standardbedingungen umfassen:

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
>Wenn Sie erneuerte (renovierte) Produkte verkaufen, müssen Sie sich anmelden bei [!DNL Amazon Renewed Program]. Siehe [Erneuerte Produkte](./renewed-products.md).

Wenn Ihr Katalog jedoch Produkte unter verschiedenen Bedingungen enthält (z. B. Neu, Gebraucht und renoviert), müssen Sie zwischen **[!UICONTROL Assign Condition Using Product Attribute]**. Mit dieser Einstellung können Sie Ihre [!DNL Commerce] Bedingungsattribut und -werte zu den Bedingungen in Ihrer Amazon-Auflistung.

Während [Aufgaben vor dem Setup](./amazon-pre-setup-tasks.md), sollten Sie eine [!DNL Commerce] Produktattribut für die Bedingung eines Produkts. Wenn Sie Produkte unter verschiedenen Bedingungen Angebot haben und kein Bedingungsattribut erstellt haben, lesen Sie die Informationen unter [Produkt-Attribut erstellen in [!DNL Commerce]](./ob-creating-magento-attributes.md). Nachdem das Bedingungsattribut erstellt wurde, können Sie jedem Ihrer Produkte in Ihrem [!DNL Commerce] Katalog.

## Einstellungen konfigurieren

1. Klick **[!UICONTROL Listing Settings]** auf dem Dashboard.

1. Erweitern der **[!UICONTROL Product Listing Condition]** Abschnitt.

1. für **[!UICONTROL Listing Product Condition]**, wählen Sie eine Option aus.

   Wählen Sie eine der standardmäßigen Amazon-Bedingungen für Ihren globalen Bedingungswert für alle Ihre Auflistungen. Standardeinstellung ist `New`.

   Wenn Sie Produkte/Listen mit unterschiedlichen Bedingungen haben, wählen Sie `Assign Condition Using Product Attribute` , um Ihre Produktzustandseinstellungen in den zusätzlichen Feldern zu definieren, die angezeigt werden.

1. für **Bedingungsattribut**, wählen Sie [!DNL Commerce] -Attribut, um Werte für die einzelnen Amazon-Bedingungsattribute zuzuordnen.

   Wenn Sie Produkte im Bereich `Used` oder `Collectible` -Bedingung, aber Sie unterscheiden nicht weiter, können Sie einer einzelnen `Used` oder `Collectible` Amazon-Zustand und lassen Sie die anderen leer. Diese Methode ordnet alle Ihre `Used` oder `Collectible` Bedingungen für die einzelne Amazon-Gebraucht- oder Sammelbedingung.

   Sie haben z. B. eine einzige `Used` für Ihre Produkte. Bei der Zuordnung wählen Sie, ob Sie der Amazon-Bedingung zuordnen möchten `Used; Like New`, `Used; Very Good`, `Used; Good`oder `Used; Acceptable`. Füllen Sie das Feld für die gewünschte Amazon-Bedingung aus, wobei die andere verbleibt `Used` Optionen eingestellt auf `--Select Option--`. Im Beispielbild werden alle [!DNL Commerce] Produkte in `Used` Bedingung ist dem Amazon zugeordnet `Used; Very Good` Bedingung.

   Sie können für Ihre Bedingungen auch beschreibenden Text eingeben, außer `New`.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Produktlistungsbedingung](assets/amazon-product-listing-condition.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Listing Product Condition] | Der Zustand Ihrer Produktliste. Optionen: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Wenn Sie eine einzige Produktbedingung verkaufen, wählen Sie eine der Amazon-Standardbedingungen. Wenn [!DNL Commerce] Katalog enthält Produkte unter verschiedenen Bedingungen. Wählen Sie `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | Die [!DNL Commerce] Attribut, das die Bedingung für Ihre Produkte definiert. Wählen Sie das von Ihnen erstellte Magneto-Attribut aus, um es dem Amazon-Bedingungsattribut zuzuordnen. In [Beispiel für Aufgaben vor dem Setup](./ob-creating-magento-attributes.md) empfiehlt die Benennung als `Amazon Condition`. Bei Auswahl dieser Option werden zusätzliche Felder für die Zuordnung der Amazon-Standardbedingungen angezeigt. |
| [!UICONTROL Additional Condition fields] | Wählen Sie für jede der Standardbedingungen Amazon die entsprechende Bedingung aus. Die Optionen sind die Bedingungsbeschriftungen, die Sie beim Hinzufügen hinzugefügt haben [Amazon-Bedingungsattribut erstellt](./ob-creating-magento-attributes.md).<br><br>Wenn Sie Produkte im Bereich `Used` oder `Collectible` -Bedingung, aber Sie unterscheiden nicht weiter, können Sie einer einzelnen `Used` oder `Collectible` Amazon-Zustand und lassen Sie die anderen leer. Diese Methode ordnet alle `Used` oder `Collectible` Bedingungen für die einzelne Amazon-Gebraucht- oder Sammelbedingung. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
