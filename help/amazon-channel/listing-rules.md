---
title: Listening-Regeln
description: Mit Listening-Regeln werden die Commerce-Katalogprodukte bestimmt, die als Amazon Marketplace-Listen veröffentlicht werden.
redirect_from: /sales-channels/asc/ob-listing-rules.html/sales-channels/asc/ob-listing-preview.html/sales-channels/asc/listing-rule-preview.html
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Listening-Regeln

Sie können auf die Listenregeln für den Store im [Store-Dashboard](./amazon-store-dashboard.md).

Listening-Regeln definieren die Regeln, um zu bestimmen, welche Produkte der Amazon-Vertriebskanal in Amazon veröffentlicht. Diese Regeln bieten viele Optionen zum Erstellen einfacher bis komplexer Regeln zum Ein- oder Ausschließen von Produkten als Listen. Jede Regel besteht aus Bedingungen, die die Voraussetzungen für die Produktlisten-Eignung festlegen.

Ihre Listening-Regeln werden kontinuierlich mit Ihrer [!DNL Commerce] Katalog. Wenn Sie neue [!DNL Commerce] Produkte, die die in Ihren Zulassungsregeln festgelegten Eignungsanforderungen erfüllen, werden die Produkte automatisch für die Aufnahme in Amazon verarbeitet.

- Wenn Sie möchten, dass alle Ihre Produkte in einer Amazon-Liste veröffentlicht werden, legen Sie keine Bedingungen für Ihre Listening-Regeln fest.

- Wenn Sie begrenzen möchten, welche Ihrer Katalogprodukte in Amazon veröffentlicht werden, definieren Sie Ihre Bedingungen für die Listenregel. Das Definieren der Bedingungen für Ihre Amazon-Listening-Regeln folgt derselben Logik und demselben Prozess wie das Definieren der Bedingungen für [Warenkorbpreisregeln](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}.

- Wenn Ihre Listening-Regeln ein Produkt ausschließen, ändert sich der Berechtigungsstatus für dieses Produkt in `Ineligible`. Nicht infrage kommende Produkte werden nicht in Amazon veröffentlicht.

- Wenn ein nicht infrage kommendes Produkt bereits in Amazon aufgeführt ist und Sie die Amazon-Liste mit Ihrer [!DNL Commerce] Katalogprodukt, die Menge für die Amazon, in der Änderungen an `0` um den Verkauf des Erzeugnisses zu verhindern. Amazon-Listen können [manuell entfernt](./end-listings-manually.md).

Änderungen an Menge und Berechtigungsstatus wirken sich auf alle Auflistungen aus, die die Amazon Seller-SKU auf Marktplätzen teilen, die für Geschäfte bestehen, die in derselben Region verkauft werden (wie definiert in _[!UICONTROL Amazon Marketplace Country]_during [Store-Integration](./store-integration.md)). Änderungen an freigegebenen [!DNL Amazon Seller SKU] in einer Region die Amazon-Listen des Produkts in einem anderen Land nicht beeinflusst.

![Listening-Regeln](assets/ob-listing-rules.png)

## Einstellungen für Listening-Regeln konfigurieren

1. Klicken **[!UICONTROL Listing Rules]** im Dashboard speichern.

1. Legen Sie die gewünschten Bedingungen für die Berechtigung von Produkten fest, die in Amazon aufgeführt werden sollen.

Siehe [Beispiel: Definieren einer Bedingung](./ob-define-condition-example.md).

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Websites] | Die verfügbaren Optionen hängen von der [Websites](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}, die Sie in Ihrem [!DNL Commerce] Konfiguration. Wählen Sie die Website für die in Amazon aufgeführten Produkte aus. Es kann nur eine Website ausgewählt werden, da für jede Website ein eindeutiger Amazon Store erforderlich ist, der im Amazon-Vertriebskanal erstellt wurde. |
| [!UICONTROL Conditions] | Wird verwendet, um die [!DNL Commerce] -Attribute für die Produkteignung in Ihrer Amazon-Region. Siehe [Beispiel: Definieren einer Bedingung](./ob-define-condition-example.md). |

## Bedingungsarbeitsbereich

Auf alle Bereiche in den fett gedruckten Bedingungen kann geklickt werden, um die verschiedenen Optionen anzuzeigen.

- Fügen Sie keine Bedingungen hinzu, wenn alle Produkte auf den ausgewählten Websites infrage kommen.
- Es gibt eine komplexe Reihe von Back-End-Prozessen, die direkt mit den Systemen von Amazon kommunizieren. Je nachdem, wie viele Elemente Sie auflisten möchten und wie beschäftigt die Amazon-Systeme sein könnten (z. B. Black Friday), kann es einige Zeit dauern, bis Ihre Artikel in Amazon aufgelistet werden.

Weitere Informationen zu Bedingungen finden Sie unter [Beschreibung der Bedingungen](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}.

## Vorschau der Listening-Regel

Wenn Sie Ihre Bedingungsdefinitionen für Ihre Listenregeln ändern, können Sie auf **[!UICONTROL Preview Changes]** , um Ihre Regeländerungen anzuwenden und zu sehen, wie sich Ihre Listen auswirken. Überprüfen Sie Ihre Auflistungen in dieser Listenvorschau-Funktion, bevor Sie Ihre Änderungen an den Listening-Regeln speichern.

Ihre Amazon-Listen werden mit Ihren Regeln und definierten Bedingungen verglichen. Anschließend können Sie Folgendes überprüfen:

- Welche Produkte wechseln basierend auf Ihrem aktuellen Status zu einem nicht förderfähigen Produkt [!DNL Amazon Seller Central] account
- Welche Erzeugnisse werden aus nicht förderfähigen Ländern wieder in den förderfähigen Status versetzt?
- Welche Produkte sind neue Amazon-Listen und wurden aus Ihrer Liste in Amazon hinzugefügt? [!DNL Commerce] products

Die Listenvorschau ermöglicht es Ihnen, eine Vorschau Ihrer potenziellen Amazon-Auflistungen anzuzeigen und die erforderlichen Anpassungen an Ihren Listenregeln vorzunehmen.

Ihre potenziellen Amazon-Auflistungen werden im _[!UICONTROL Listing Preview]_Seite in einem der drei Registerkarten:

- **[!UICONTROL Ineligible Listings]** - Die aufgelisteten Produkte können aufgrund Ihrer aktuellen Listenregeln und -bedingungen nicht in die Amazon-Liste aufgenommen werden.

   Nicht infrage kommende Produkte werden nicht in Amazon veröffentlicht. Wenn ein nicht infrage kommendes Produkt bereits in Amazon aufgeführt ist und Sie die Amazon-Liste mit Ihrer [!DNL Commerce] Katalogprodukt, die Menge für die Amazon, in der Änderungen an `0` um den Verkauf des Erzeugnisses zu verhindern. Informationen zum manuellen Entfernen einer Liste finden Sie unter [Beenden einer Amazon-Auflistung](./end-listings-manually.md). Produkte, die nicht für Amazon-Anforderungen infrage kommen, sind hier nicht aufgeführt. Diese Produkte sind auf der [Registerkarte &quot;Inaktive Listen&quot;](./inactive-listings.md).

- **[!UICONTROL Eligible Listings]** - aufgelistete Produkte können auf der Grundlage Ihrer aktuellen Listenregeln und -bedingungen in die Amazon-Liste aufgenommen werden und sind auch für Amazon-Anforderungen geeignet. Diese Liste enthält Ihre vorhandenen Amazon-Listen, die importiert werden (falls Sie **Importieren von Drittanbieterlisten** auf `Import Listing` in [Listening-Einstellungen](./third-party-listing-settings.md)).

- **[!UICONTROL New Listings]** - Die aufgelisteten Produkte enthalten Ihre [!DNL Commerce] Katalogprodukte, die auf Grundlage Ihrer aktuellen Listenregeln und -bedingungen für eine Amazon-Auflistung zugelassen werden, sowie neue Amazon-Listen erstellen und veröffentlichen.

### Listenvorschau anzeigen

1. Klicken **[!UICONTROL Listing Rules]** im Dashboard speichern.

1. Anzeigen oder Hinzufügen von [Auflistungsregeln](./listing-rules.md).

1. Ändern Sie Ihre [Bedingungen für Listening-Regeln](./ob-define-condition-example.md).

1. Klicken **[!UICONTROL Preview Changes]**.

1. Überprüfen und bestätigen Sie Ihre Auflistungen im _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_ und _[!UICONTROL New Listings]_Registerkarten.

1. Wenn Ihre Auflistungen Ihren Erwartungen entsprechen, klicken Sie auf **[!UICONTROL Save and close]**.

   Wenn Ihre Listen nicht wie erwartet angezeigt werden, klicken Sie auf **[!UICONTROL Back]** und ändern Sie Ihre Regeln und Bedingungen, bis Ihre Listen Ihren Erwartungen entsprechen.

![Vorschau der Listening-Regel](assets/amazon-listing-rule-preview.png)

### Auflisten von Vorschaudatensätzen

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Product ID] | Die eindeutige, sequenzielle Zahl, die einer [!DNL Commerce] -Katalogprodukt, wenn es hinzugefügt wird. |
| [!UICONTROL Thumbnail] | Zeigt eine Miniaturansicht des Hauptproduktbilds an. |
| [!UICONTROL Name] | Der Name des Produkts, das im [!DNL Commerce] [Produktraster](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Type] | Der Produkttyp, der im [!DNL Commerce] Produktraster. |
| [!UICONTROL Attribute Set] | Der Name des Attributsatzes, der als Vorlage für das Produkt verwendet wird und im [!DNL Commerce] Produktraster. |
| [!UICONTROL SKU] | Die eindeutige Lagereinheit, die dem Produkt zugewiesen und im [!DNL Commerce] Produktraster. |
| [!UICONTROL Visibility] | Gibt an, wo das Produkt sichtbar und im [!DNL Commerce] Produktraster. Optionen:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| Status | Gibt den Status des Produkts an, das im [!DNL Commerce] Produktraster. Optionen: `Enabled` / `Disabled` |

![Workflow für die Listenvorschau](assets/listing-preview-flowchart.png)
