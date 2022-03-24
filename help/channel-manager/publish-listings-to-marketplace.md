---
title: Veröffentlichen von Listen in Walmart
description: Veröffentlichen Sie Auflistungen für Commerce-Produkte in Walmart Marketplace , um mit dem Verkauf zu beginnen.
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Veröffentlichen von Listen in Walmart

Wie andere Marktplätze ermöglicht es auch Walmart Anbietern, von anderen Anbietern verkaufte Artikel aufzulisten.

Die Plattform verwendet Produktidentifikatoren wie UPC und GTIN, um Artikel zuzuordnen, die bereits zum Verkauf angeboten werden.
Für passende Produkte listet der vorhandene Walmart Marketplace Aktualisierungen auf, um das Angebot für das Commerce-Produkt aufzunehmen.
In der Regel erscheinen Produkte mit den niedrigsten Preisen zuerst in den Ergebnissen. Aber auch andere Faktoren wie Bewertungen beeinflussen die Platzierung.

## Abgleichs-Workflow

Wenn Sie Produkte abgleichen, sendet der Kanal-Manager die Produktdaten an den Walmart Marketplace, um nach vorhandenen Listen mit Attributwerten zu suchen, die mit dem zugeordneten Commerce-Produktattribut übereinstimmen.

Wenn eine Übereinstimmung gefunden wird, wird die vorhandene Produktliste aktualisiert, um Ihr Angebot hinzuzufügen.

## Voraussetzungen

Bevor Sie Produkte zuordnen, überprüfen Sie, ob Ihre Produktkatalog-Attributwerte die Walmart-Anforderungen erfüllen, und konfigurieren Sie die Attributeinstellungen. Siehe [Produktabgleich konfigurieren](map-product-attributes-for-matching.md)

## Produkte auswählen und abgleichen

1. Öffnen Sie einen verbundenen Vertriebskanal.

1. Von **[!UICONTROL Listings]**, wählen Sie Produkte für die Übereinstimmung aus, die in *[!UICONTROL Draft]* Status.

   ![Produkte aus Listen auswählen und zur Übereinstimmung senden](assets/products-in-marketplace-sales-channel.png)

1. Auswählen **[!UICONTROL Match Products]**.

   Eine Meldung gibt die Anzahl der Produkte an, die zum Abgleich gesendet wurden.

   ![Produkte an den verbundenen Vertriebskanal senden](assets/products-submit-for-matching.png)

   Es kann bis zu 30 Minuten dauern, bis Walmart Marketplace den Match-Vorgang abschließt.

   Der Status für ausgewählte Produkte ändert sich in *[!UICONTROL Processing]* bis die Match-Vorgänge abgeschlossen sind. Es kann bis zu 30 Minuten dauern, bis Walmart Marketplace den Match-Vorgang abschließt.

## Prüfen des Übereinstimmungsstatus

1. Auswählen **Produkte aktualisieren** , um den aktuellen Produktstatus zu aktualisieren.

1. Überprüfen Sie den Produktstatus.

   Nach Abschluss der Übereinstimmung kann der Status *Übereinstimmung* oder *Fehler*.

   * **[!UICONTROL Match]** gibt an, dass das Produkt erfolgreich abgeglichen wurde. Ihr Produktangebot wurde auf einer vorhandenen Walmart Marketplace-Liste veröffentlicht.

   * **[!UICONTROL Error]** bezeichnet eine der folgenden Eigenschaften:

      * Es ist ein Fehler aufgetreten und der Match-Vorgang ist fehlgeschlagen.

      * Es wurde keine Übereinstimmung gefunden.

      * Übereinstimmung gefunden, aber Produkt als inszeniert veröffentlicht, weil die [Marketplace store ist nicht aktiv](walmart-prerequisites.md#walmart-marketplace-store-status).

## Fehlerbehebung bei Produktübereinstimmungsfehlern

Wenn der Vorgang der Produktübereinstimmung fehlschlägt, gibt der Walmart Marketplace einen Fehlercode zurück und der Kanal-Manager zeigt den Fehlerstatus in den Informationen zur Produktliste an.

Zeigen Sie die Details der Fehlermeldungen an, indem Sie den Mauszeiger über die **Fehler** Statusbezeichnung. Häufige Fehler, die zurückgegeben werden, sind falsch formatierte Produkt-ID-Werte oder fehlende erforderliche Attribute.

## Produkt-ID-Werte korrigieren

| Typ | Beschreibung | Beispiel |
|------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, die 12-stellige Zahl einschließlich der Prüfziffer.</br></br>Wenn Ihr UPC weniger als 12 Ziffern enthält, z. B. UPC-E, das 8-stellig ist, fügen Sie</br>führende Nullen zur Erfüllung der Anforderungen. | Ändern von `45678912345` nach `045678912345` |
| GTIN | GTIN-14, die 14-stellige Zahl einschließlich der Prüfziffer.</br></br>Wenn Ihr GTIN weniger als 14 Stellen enthält, fügen Sie führende Nullen hinzu </br>, um die Anforderungen zu erfüllen. | Änderung `456789123456` nach `0045678912345` |
| EAN | GTIN-13, die 13-stellige Zahl einschließlich der Prüfziffer.</br></br>Wenn Ihr EAN weniger als 13 Stellen enthält, fügen Sie den Zeilensprung hinzu.</br>Nullen zur Erfüllung der Anforderung. | Ändern von `4567891234` nach `0004567891234` |

Weitere Informationen zu den Fehler-Codes von Walmart Marketplace finden Sie in der [Walmart Seller-Hilfe](https://sellerhelp.walmart.com/s/guide?article=000005844).
