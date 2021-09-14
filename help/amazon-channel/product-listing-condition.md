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

Die Bedingungseinstellungen für die Produktliste sind Teil Ihrer Einstellungen für die Store-Auflistung. Sie können auf die Listeneinstellungen im [Dashboard speichern](./amazon-store-dashboard.md) zugreifen.

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
>Wenn Sie erneuerte (renovierte) Produkte verkaufen, müssen Sie sich bei [!DNL Amazon Renewed Program] anmelden. Siehe [Erneute Produkte](./renewed-products.md).

Wenn Ihr Katalog jedoch Produkte mit unterschiedlichen Bedingungen enthält (z. B. Neu, Verwendet und renoviert), müssen Sie **[!UICONTROL Assign Condition Using Product Attribute]** auswählen. Mit dieser Einstellung können Sie Ihr [!DNL Commerce]-Bedingungsattribut und Ihre Werte den Bedingungen Ihrer Amazon-Auflistung zuordnen.

Bei [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md) sollten Sie ein [!DNL Commerce]-Produktattribut für die Bedingung eines Produkts erstellen. Wenn Sie Produkte unter verschiedenen Bedingungen anbieten und kein Bedingungsattribut erstellt haben, finden Sie weitere Informationen unter [Erstellen eines Produktattributs in [!DNL Commerce]](./ob-creating-magento-attributes.md). Nachdem das Bedingungsattribut erstellt wurde, können Sie jedem Ihrer Produkte in Ihrem [!DNL Commerce] -Katalog einen Bedingungswert zuweisen.

## Einstellungen konfigurieren

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt **[!UICONTROL Product Listing Condition]** .

1. Wählen Sie für **[!UICONTROL Listing Product Condition]** eine Option aus.

   Wählen Sie eine der standardmäßigen Amazon-Bedingungen für Ihren globalen Bedingungswert für alle Ihre Auflistungen aus. Die Standardeinstellung ist `New`.

   Wenn Sie über Produkte/Listen mit unterschiedlichen Bedingungen verfügen, wählen Sie `Assign Condition Using Product Attribute` aus, um die Einstellungen für Ihre Produktbedingungen in den zusätzlichen angezeigten Feldern zu definieren.

1. Wählen Sie für **Bedingungsattribut** das Attribut [!DNL Commerce] aus, um Werte für die einzelnen standardmäßigen Amazon-Bedingungsattribute zuzuordnen.

   Wenn Sie Produkte in der Bedingung `Used` oder `Collectible` haben, aber nicht weiter unterscheiden, können Sie eine einzelne Bedingung `Used` oder `Collectible` Amazon zuordnen und die anderen leer lassen. Diese Methode ordnet alle `Used` - oder `Collectible` -Bedingungen der einzelnen verwendeten oder kollektiven Amazon-Bedingung zu.

   Sie haben beispielsweise eine einzelne `Used` -Bedingung für Ihre Produkte. Bei der Zuordnung wählen Sie aus, ob Sie der Amazon-Bedingung `Used; Like New`, `Used; Very Good`, `Used; Good` oder `Used; Acceptable` zuordnen möchten. Füllen Sie nur das Feld für die gewünschte Amazon-Bedingung aus, wobei die anderen `Used`-Optionen auf `--Select Option--` gesetzt bleiben. Im Beispielbild werden alle [!DNL Commerce] -Produkte in der Bedingung `Used` der Bedingung Amazon `Used; Very Good` zugeordnet.

   Sie können auch beschreibenden Text für Ihre Bedingungen eingeben, mit Ausnahme von `New`.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Bedingung für die Produktliste](assets/amazon-product-listing-condition.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Listing Product Condition] | Die Bedingung Ihrer Produktlisten. Optionen: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>Wenn Sie eine einzige Produktbedingung verkaufen, wählen Sie eine der Amazon-Standardbedingungen. Wenn Ihr [!DNL Commerce] -Katalog Produkte in verschiedenen Bedingungen enthält, wählen Sie `Assign Condition Using Product Attribute` aus. |
| [!UICONTROL Condition Attribute] | Das [!DNL Commerce]-Attribut, das die Bedingung für Ihre Produkte definiert. Wählen Sie das von Ihnen erstellte Attribut Magneto aus, um es dem Amazon-Bedingungsattribut zuzuordnen. Im Beispiel [Vorsetup-Aufgaben](./ob-creating-magento-attributes.md) empfiehlt die Benennung als `Amazon Condition`. Wenn diese Option ausgewählt ist, werden zusätzliche Felder für die Zuordnung der standardmäßigen Amazon-Bedingungen angezeigt. |
| [!UICONTROL Additional Condition fields] | Wählen Sie für jede der standardmäßigen Amazon-Bedingungen die entsprechende Bedingung aus. Die Optionen sind die Bedingungsbezeichnungen, die Sie hinzugefügt haben, als Sie [Ihr Amazon-Bedingungsattribut](./ob-creating-magento-attributes.md) erstellt haben.<br><br>Wenn Sie Produkte in der  `Used` -  `Collectible` Bedingung haben, aber nicht weiter unterscheiden, können Sie eine einzelne  `Used` oder  `Collectible` Amazon-Bedingung zuordnen und die anderen leer lassen. Diese Methode ordnet alle `Used` - oder `Collectible` -Bedingungen der einzelnen verwendeten Amazon- oder Sammelbedingung zu. |

**Schnellzugriff**  -  [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
