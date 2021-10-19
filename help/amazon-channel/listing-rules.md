---
title: Listungsregeln
description: Verwenden Sie Listungsregeln, um die Commerce-Katalogprodukte zu bestimmen, die als Amazon Marketplace-Listen veröffentlicht werden.
redirect_from: /sales-channels/asc/ob-listing-rules.html/sales-channels/asc/ob-listing-preview.html/sales-channels/asc/listing-rule-preview.html
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Listungsregeln

Sie können auf die Listungsregeln für den Store im [Dashboard speichern](./amazon-store-dashboard.md).

Mit Listungsregeln werden Regeln festgelegt, anhand derer bestimmt wird, welche Produkte Amazon Sales Kanal in Amazon veröffentlicht. Diese Regeln bieten viele Möglichkeiten, einfache bis komplexe Regeln zu erstellen, um Produkte als Auflistung einzubeziehen oder auszuschließen. Jede Regel besteht aus Bedingungen, die die Voraussetzungen für die Zulassung zur Produktliste festlegen.

Ihre Listungsregeln werden kontinuierlich mit Ihrer synchronisiert. [!DNL Commerce] Katalog. Wenn Sie neue hinzufügen [!DNL Commerce] Produkte, die die in Ihren Regeln festgelegten Anforderungen an die Förderfähigkeit erfüllen, werden automatisch zur Aufnahme in Amazon verarbeitet.

- Wenn Sie möchten, dass alle Ihre Produkte in einer Amazon-Liste veröffentlicht werden, legen Sie keine Bedingungen für Ihre Listungsregeln fest.

- Wenn Sie begrenzen möchten, welche Katalogprodukte auf Amazon veröffentlicht werden, definieren Sie die Bedingungen für Ihre Listingregeln. Die Festlegung der Bedingungen für Ihre Amazon-Listungsregeln folgt derselben Logik und demselben Verfahren wie die Festlegung der Bedingungen für die Festlegung der [Regeln für Warenkorb-Preise](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){Zielgruppe=&quot;_blank&quot;}.

- Wenn Ihre Listungsregeln ein Produkt ausschließen, ändert sich der Berechtigungsstatus für dieses Produkt in `Ineligible`. Nicht förderfähige Produkte werden nicht auf Amazon veröffentlicht.

- Wenn ein nicht zugelassenes Produkt bereits auf Amazon aufgeführt ist und Sie die Amazon-Liste Ihrem [!DNL Commerce] Katalogprodukt, die Menge für die Amazon-Auflistung ändert sich in `0` um den Verkauf der Ware zu verhindern. Amazon-Listen können [manuell entfernt](./end-listings-manually.md).

Änderungen der Menge und des Zulassungsstatus wirken sich auf alle Auflistungen aus, die die Amazon Seller-SKU auf Marktplätzen teilen, die für Geschäfte bestehen, die in derselben Region (gemäß Definition in _[!UICONTROL Amazon Marketplace Country]_während [Speicherintegration](./store-integration.md)). Eine Änderung an einer freigegebenen [!DNL Amazon Seller SKU] in einem Gebiet die Amazon-Liste des Erzeugnisses in einem anderen Land nicht beeinflusst.

![Listungsregeln](assets/ob-listing-rules.png)

## Listingregeleinstellungen konfigurieren

1. Klick **[!UICONTROL Listing Rules]** auf dem Dashboard.

1. Legen Sie die Bedingungen fest, unter denen die Produkte in Amazon aufgeführt werden dürfen.

Siehe [Beispiel: Bedingung definieren](./ob-define-condition-example.md).

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Websites] | Die verfügbaren Optionen hängen von der [Websites](https://docs.magento.com/user-guide/stores/websites-stores-views.html){Zielgruppe=&quot;_blank&quot;}, die Sie in Ihrem [!DNL Commerce] Konfiguration. Wählen Sie die Website für die in Amazon aufgeführten Produkte aus. Es kann nur eine Website ausgewählt werden, da für jede Website ein einzigartiger Amazon Store im Amazon Sales Kanal erstellt werden muss. |
| [!UICONTROL Conditions] | Wird verwendet, um [!DNL Commerce] Attribute für die Produktberechtigung in Ihrer Amazon-Region. Siehe [Beispiel: Bedingung definieren](./ob-define-condition-example.md). |

## Bedingungsarbeitsbereich

Alle Bereiche in den Bedingungen, die fett sind, können angeklickt werden, um die verschiedenen Optionen zu sehen.

- Fügen Sie keine Bedingungen hinzu, wenn alle Produkte innerhalb der ausgewählten Websites förderfähig sind.
- Es gibt eine komplexe Reihe von Back-End-Prozessen, die direkt mit Amazon-Systemen kommuniziert werden können. Aufgrund der Anzahl der Elemente, die Sie zu Listen versuchen, und der möglicherweise sehr ausgelasteten Amazon-Systeme (z. B. Black Freitag) kann es einige Zeit dauern, bis Ihre Artikel auf Amazon aufgelistet werden.

Weitere Informationen zu den Bedingungen finden Sie unter [Beschreiben Sie die Bedingungen](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){Zielgruppe=&quot;_blank&quot;}.

## Vorschau der Listungsregel

Wenn Sie die Bedingungsdefinitionen für Ihre Listingregeln ändern, können Sie auf **[!UICONTROL Preview Changes]** , um Regeländerungen und die Ansicht anzuwenden, wie Ihre Auflistungen beeinflusst werden. Überprüfen Sie Ihre Einträge in dieser Vorschau, bevor Sie Ihre Änderungen an den Regeln speichern.

Ihre Amazon-Auflistungen werden mit Ihren Regeln und definierten Bedingungen verglichen. Sie können dann Folgendes überprüfen:

- Welche Produkte werden aufgrund Ihres aktuellen Status in einen nicht förderfähigen Status verschoben [!DNL Amazon Seller Central] Konto
- Welche Erzeugnisse kommen aus nicht förderfähigen Ländern wieder in den förderfähigen Status?
- Welche Produkte sind neue Amazon-Listen und wurden aus Ihrem förderfähigen Amazon-Konto in Ihre Liste aufgenommen? [!DNL Commerce] Produkte

Mit der Listing-Vorschau können Sie Ihre potenziellen Amazon-Auflistungen Vorschau und alle erforderlichen Anpassungen an Ihren Listingregeln vornehmen.

Ihre potenziellen Amazon-Auflistungen werden auf der _[!UICONTROL Listing Preview]_Seite in einem von drei Registerkarten:

- **[!UICONTROL Ineligible Listings]** - Die aufgelisteten Produkte können aufgrund Ihrer aktuellen Listungsregeln und -bedingungen nicht in die Amazon-Liste aufgenommen werden.

   Nicht förderfähige Produkte werden nicht auf Amazon veröffentlicht. Wenn ein nicht zugelassenes Produkt bereits auf Amazon aufgeführt ist und Sie die Amazon-Liste Ihrem [!DNL Commerce] Katalogprodukt, die Menge für die Amazon-Auflistung ändert sich in `0` um den Verkauf der Ware zu verhindern. Informationen zum manuellen Entfernen einer Auflistung finden Sie unter [Beenden einer Amazon-Liste](./end-listings-manually.md). Produkte, die nicht unter die Amazon-Anforderungen fallen, sind hier nicht aufgeführt. Diese Erzeugnisse sind im [Registerkarte &quot;Inaktive Auflistungen&quot;](./inactive-listings.md).

- **[!UICONTROL Eligible Listings]** - Die aufgelisteten Produkte sind für eine Amazon-Auflistung auf der Grundlage Ihrer aktuellen Börsenregeln und -bedingungen infrage kommen und können auch von Amazon-Anforderungen erfasst werden. Diese Liste enthält Ihre vorhandenen Amazon-Listen, die importiert werden (falls Sie **Listen von Drittanbietern importieren** einstellen auf `Import Listing` in [Listingeinstellungen](./third-party-listing-settings.md)).

- **[!UICONTROL New Listings]** - Zu den aufgelisteten Produkten gehören [!DNL Commerce] Katalogprodukte, die aufgrund Ihrer aktuellen Listungsregeln und -bedingungen neu für die Amazon-Auflistung zugelassen sind, und erstellen und veröffentlichen Sie neue Amazon-Listen.

### Ansicht der Vorschau in der Auflistung

1. Klick **[!UICONTROL Listing Rules]** auf dem Dashboard.

1. Ansicht oder fügen Sie Ihre [Listungsregeln](./listing-rules.md).

1. Ändern Sie Ihre [Regelbedingungen für Auflistung](./ob-define-condition-example.md).

1. Klick **[!UICONTROL Preview Changes]**.

1. Überprüfen und bestätigen Sie Ihre Einträge im _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_ und _[!UICONTROL New Listings]_Tabulatoren.

1. Wenn Ihre Auflistungen Ihren Erwartungen entsprechen, klicken Sie **[!UICONTROL Save and close]**.

   Wenn Ihre Auflistungen nicht wie erwartet angezeigt werden, klicken Sie **[!UICONTROL Back]** und ändern Sie Ihre Regeln und Bedingungen, bis Ihre Auflistungen Ihren Erwartungen entsprechen.

![Vorschau der Listungsregel](assets/amazon-listing-rule-preview.png)

### Listet Vorschauen auf

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Product ID] | Die eindeutige, sequenzielle Nummer, die einem [!DNL Commerce] Katalogprodukt, wenn es hinzugefügt wird. |
| [!UICONTROL Thumbnail] | Zeigt eine Miniaturansicht des Hauptproduktbildes an. |
| [!UICONTROL Name] | Der Name des Produkts, verwaltet in [!DNL Commerce] [Produktraster](https://docs.magento.com/user-guide/catalog/products.html){Zielgruppe=&quot;_blank&quot;}. |
| [!UICONTROL Type] | Der Produkttyp, verwaltet in der [!DNL Commerce] Produktraster. |
| [!UICONTROL Attribute Set] | Der Name des Attributsatzes, der als Vorlage für das Produkt verwendet wird, verwaltet in [!DNL Commerce] Produktraster. |
| [!UICONTROL SKU] | Die dem Produkt zugewiesene, in der [!DNL Commerce] Produktraster. |
| [!UICONTROL Visibility] | Gibt an, wo das Produkt sichtbar ist, verwaltet in der [!DNL Commerce] Produktraster. Optionen:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| Status | Gibt den Status des Produkts an, verwaltet in [!DNL Commerce] Produktraster. Optionen: `Enabled` / `Disabled` |

![Workflow für Vorschau auflisten](assets/listing-preview-flowchart.png)
