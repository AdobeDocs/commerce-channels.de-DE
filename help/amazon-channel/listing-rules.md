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

Sie können auf die Listening-Regeln für den Store im [Dashboard speichern](./amazon-store-dashboard.md) zugreifen.

Listening-Regeln definieren die Regeln, um zu bestimmen, welche Produkte der Amazon-Vertriebskanal in Amazon veröffentlicht. Diese Regeln bieten viele Optionen zum Erstellen einfacher bis komplexer Regeln zum Ein- oder Ausschließen von Produkten als Listen. Jede Regel besteht aus Bedingungen, die die Voraussetzungen für die Produktlisten-Eignung festlegen.

Ihre Listening-Regeln werden kontinuierlich mit Ihrem [!DNL Commerce]-Katalog synchronisiert. Wenn Sie neue [!DNL Commerce]-Produkte hinzufügen, die die von Ihren Listening-Regeln festgelegten Eignungsanforderungen erfüllen, werden die Produkte automatisch für die Auflistung in Amazon verarbeitet.

- Wenn Sie möchten, dass alle Ihre Produkte in einer Amazon-Liste veröffentlicht werden, legen Sie keine Bedingungen für Ihre Listening-Regeln fest.

- Wenn Sie begrenzen möchten, welche Ihrer Katalogprodukte in Amazon veröffentlicht werden, definieren Sie Ihre Bedingungen für die Listenregel. Das Definieren der Bedingungen für Ihre Amazon-Listening-Regeln folgt derselben Logik und demselben Prozess wie das Definieren der Bedingungen für [Warenkorbpreisregeln](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}.

- Wenn Ihre Listening-Regeln ein Produkt ausschließen, ändert sich der Berechtigungsstatus für dieses Produkt in `Ineligible`. Nicht infrage kommende Produkte werden nicht in Amazon veröffentlicht.

- Wenn ein nicht infrage kommendes Produkt bereits in Amazon aufgeführt ist und Sie die Amazon-Liste mit Ihrem [!DNL Commerce]-Katalogprodukt abgleichen, ändert sich die Menge für die Amazon-Auflistung in `0`, um den Verkauf des Produkts zu verhindern. Amazon-Listen können [manuell entfernt](./end-listings-manually.md) sein.

Änderungen an Menge und Berechtigungsstatus wirken sich auf alle Auflistungen aus, die die Amazon Seller-SKU auf Marktplätzen teilen, die für Geschäfte vorhanden sind, die in derselben Region verkauft werden (wie in _[!UICONTROL Amazon Marketplace Country]_während der [Store-Integration](./store-integration.md) definiert). Eine Änderung an einem freigegebenen [!DNL Amazon Seller SKU] in einer Region wirkt sich jedoch nicht auf die Amazon-Listen des Produkts in einem anderen Land aus.

![Listening-Regeln](assets/ob-listing-rules.png)

## Einstellungen für Listening-Regeln konfigurieren

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Rules]** .

1. Legen Sie die gewünschten Bedingungen für die Berechtigung von Produkten fest, die in Amazon aufgeführt werden sollen.

Siehe [Beispiel: Definieren Sie eine Bedingung](./ob-define-condition-example.md).

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Websites] | Die verfügbaren Optionen hängen von den [Websites](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} ab, die Sie in Ihrer [!DNL Commerce]-Konfiguration eingerichtet haben. Wählen Sie die Website für die in Amazon aufgeführten Produkte aus. Es kann nur eine Website ausgewählt werden, da für jede Website ein eindeutiger Amazon Store erforderlich ist, der im Amazon-Vertriebskanal erstellt wurde. |
| [!UICONTROL Conditions] | Wird verwendet, um die [!DNL Commerce]-Attribute für die Produkteignung in Ihrer Amazon-Region zu definieren. Siehe [Beispiel: Definieren Sie eine Bedingung](./ob-define-condition-example.md). |

## Bedingungsarbeitsbereich

Auf alle Bereiche in den fett gedruckten Bedingungen kann geklickt werden, um die verschiedenen Optionen anzuzeigen.

- Fügen Sie keine Bedingungen hinzu, wenn alle Produkte auf den ausgewählten Websites infrage kommen.
- Es gibt eine komplexe Reihe von Back-End-Prozessen, die direkt mit den Systemen von Amazon kommunizieren. Je nachdem, wie viele Elemente Sie auflisten möchten und wie beschäftigt die Amazon-Systeme sein könnten (z. B. Black Friday), kann es einige Zeit dauern, bis Ihre Artikel in Amazon aufgelistet werden.

Weitere Informationen zu Bedingungen finden Sie unter [Beschreibung der Bedingungen](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}.

## Vorschau der Listening-Regel

Wenn Sie Ihre Bedingungsdefinitionen für Ihre Listenregeln ändern, können Sie auf **[!UICONTROL Preview Changes]** klicken, um Ihre Regeländerungen anzuwenden und zu sehen, wie sich Ihre Listen auswirken. Überprüfen Sie Ihre Auflistungen in dieser Listenvorschau-Funktion, bevor Sie Ihre Änderungen an den Listening-Regeln speichern.

Ihre Amazon-Listen werden mit Ihren Regeln und definierten Bedingungen verglichen. Anschließend können Sie Folgendes überprüfen:

- Welche Produkte werden auf Grundlage Ihres aktuellen [!DNL Amazon Seller Central]-Kontos in den Status &quot;Nicht qualifiziert&quot; versetzt
- Welche Erzeugnisse werden aus nicht förderfähigen Ländern wieder in den förderfähigen Status versetzt?
- Welche Produkte sind neue Amazon-Listen und wurden aus Ihren infrage kommenden [!DNL Commerce]-Produkten zu Ihrer Amazon-Liste hinzugefügt?

Die Listenvorschau ermöglicht es Ihnen, eine Vorschau Ihrer potenziellen Amazon-Auflistungen anzuzeigen und die erforderlichen Anpassungen an Ihren Listenregeln vorzunehmen.

Ihre potenziellen Amazon-Auflistungen werden auf der Seite _[!UICONTROL Listing Preview]_in einem von drei Registerkarten angezeigt:

- **[!UICONTROL Ineligible Listings]** - Die aufgelisteten Produkte können aufgrund Ihrer aktuellen Listenregeln und -bedingungen nicht in die Amazon-Liste aufgenommen werden.

   Nicht infrage kommende Produkte werden nicht in Amazon veröffentlicht. Wenn ein nicht infrage kommendes Produkt bereits in Amazon aufgeführt ist und Sie die Amazon-Liste mit Ihrem [!DNL Commerce]-Katalogprodukt abgleichen, ändert sich die Menge für die Amazon-Auflistung in `0`, um den Verkauf des Produkts zu verhindern. Informationen zum manuellen Entfernen einer Auflistung finden Sie unter [Beenden einer Amazon-Auflistung](./end-listings-manually.md). Produkte, die nicht für Amazon-Anforderungen infrage kommen, sind hier nicht aufgeführt. Diese Produkte sind auf der Registerkarte [Inaktive Listen](./inactive-listings.md) aufgeführt.

- **[!UICONTROL Eligible Listings]** - aufgelistete Produkte können auf der Grundlage Ihrer aktuellen Listenregeln und -bedingungen in die Amazon-Liste aufgenommen werden und sind auch für Amazon-Anforderungen geeignet. Diese Liste enthält Ihre vorhandenen Amazon-Listen, die importiert werden (wenn Sie **Drittanbieterlisten importieren** in [Listeneinstellungen](./third-party-listing-settings.md) auf `Import Listing` gesetzt haben).

- **[!UICONTROL New Listings]** - Zu den aufgelisteten Produkten gehören Ihre  [!DNL Commerce] Katalogprodukte, die auf der Grundlage Ihrer aktuellen Listenregeln und -bedingungen neu für die Amazon-Auflistung infrage kommen. Außerdem können Sie neue Amazon-Listen erstellen und veröffentlichen.

### Listenvorschau anzeigen

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Rules]** .

1. Zeigen Sie Ihre [Listening-Regeln](./listing-rules.md) an oder fügen Sie sie hinzu.

1. Ändern Sie Ihre [Listing Rule Conditions](./ob-define-condition-example.md).

1. Klicken Sie auf **[!UICONTROL Preview Changes]**.

1. Überprüfen und bestätigen Sie Ihre Auflistungen auf den Registerkarten _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_ und _[!UICONTROL New Listings]_.

1. Wenn Ihre Auflistungen Ihren Erwartungen entsprechen, klicken Sie auf **[!UICONTROL Save and close]**.

   Wenn Ihre Auflistungen nicht wie erwartet angezeigt werden, klicken Sie auf **[!UICONTROL Back]** und ändern Sie Ihre Regeln und Bedingungen, bis Ihre Auflistungen Ihren Erwartungen entsprechen.

![Vorschau der Listening-Regel](assets/amazon-listing-rule-preview.png)

### Auflisten von Vorschaudatensätzen

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Product ID] | Die eindeutige, sequenzielle Nummer, die einem [!DNL Commerce] -Katalogprodukt zugewiesen wird, wenn es hinzugefügt wird. |
| [!UICONTROL Thumbnail] | Zeigt eine Miniaturansicht des Hauptproduktbilds an. |
| [!UICONTROL Name] | Der Name des Produkts, verwaltet im [!DNL Commerce] [Produktraster](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Type] | Der Produkttyp, der im Produktraster [!DNL Commerce] verwaltet wird. |
| [!UICONTROL Attribute Set] | Der Name des Attributsatzes, der als Vorlage für das Produkt verwendet wird und im Produktraster [!DNL Commerce] verwaltet wird. |
| [!UICONTROL SKU] | Die eindeutige Lagereinheit, die dem Produkt zugewiesen ist und im Produktraster [!DNL Commerce] verwaltet wird. |
| [!UICONTROL Visibility] | Gibt an, wo das Produkt sichtbar ist, verwaltet im Produktraster [!DNL Commerce]. Optionen:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| Status | Gibt den Status des Produkts an, das im Produktraster [!DNL Commerce] verwaltet wird. Optionen: `Enabled` / `Disabled` |

![Workflow für die Listenvorschau](assets/listing-preview-flowchart.png)
