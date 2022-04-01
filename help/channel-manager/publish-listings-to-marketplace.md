---
title: Veröffentlichen von Listen in Walmart
description: Veröffentlichen Sie Auflistungen für Commerce-Produkte in Walmart Marketplace , um mit dem Verkauf zu beginnen.
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: a10ab3f7fa7049e48d83a942f6c5441d8147b12c
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Veröffentlichen von Listen in Walmart

Wie andere Marktplätze ermöglicht es auch Walmart Anbietern, von anderen Anbietern verkaufte Artikel aufzulisten.

Die Plattform verwendet Produktidentifikatoren wie UPC und GTIN, um Artikel zuzuordnen, die bereits zum Verkauf angeboten werden.
Für passende Produkte enthält der vorhandene Walmart Marketplace Aktualisierungen, die das Commerce-Produktangebot enthalten.

Normalerweise erscheinen Produkte mit den niedrigsten Preisen zuerst in den Ergebnissen, aber andere Faktoren wie Bewertungen beeinflussen auch die Platzierung.

## Produkte abgleichen

Wenn Sie Produkte abgleichen, sendet der Kanal-Manager die Produktdaten an den Walmart Marketplace, um nach vorhandenen Listen mit Attributwerten zu suchen, die mit dem zugeordneten Commerce-Produktattribut übereinstimmen. Übereinstimmungskriterien werden durch die [Konfiguration der Attributzuordnung](map-product-attributes-for-matching.md) für Ihren Store-Kanal.

Wenn eine Übereinstimmung gefunden wird, wird die vorhandene Produktliste aktualisiert, um Ihr Angebot hinzuzufügen.

### Voraussetzungen

Bevor Sie Produkte zuordnen, überprüfen Sie, ob Ihre Produktkatalog-Attributwerte die Walmart-Anforderungen erfüllen, und konfigurieren Sie die Attributeinstellungen. Siehe [Produktabgleich konfigurieren](map-product-attributes-for-matching.md)

#### Produkte auswählen und abgleichen

1. Öffnen Sie einen verbundenen Vertriebskanal.

1. Von **[!UICONTROL Listings]**, wählen Sie Produkte für die Übereinstimmung aus, die in *[!UICONTROL Draft]* Status.

   ![Produkte aus Listen auswählen und zur Übereinstimmung senden](assets/products-in-marketplace-sales-channel.png)

1. Auswählen **[!UICONTROL Match Products]**.

   Eine Meldung gibt die Anzahl der Produkte an, die zum Abgleich gesendet wurden.

   ![Produkte an den verbundenen Vertriebskanal senden](assets/products-submit-for-matching.png)

   Der Status für ausgewählte Produkte ändert sich in [!UICONTROL *Verarbeitung*] bis der Match-Vorgang abgeschlossen ist. Es kann bis zu 30 Minuten dauern, bis Walmart Marketplace den Match-Vorgang abschließt.

### Prüfen des Übereinstimmungsstatus

1. Auswählen **Produkte aktualisieren** , um den aktuellen Produktstatus zu aktualisieren.

1. Überprüfen Sie den Produktstatus.

   Nach Abschluss der Übereinstimmung kann der Status *Übereinstimmung* oder *Fehler*.

   * **[!UICONTROL Match]** gibt an, dass das Produkt erfolgreich abgeglichen wurde. Ihr Produktangebot wurde auf einer vorhandenen Walmart Marketplace-Liste veröffentlicht.

   * **[!UICONTROL Error]** bezeichnet eine der folgenden Eigenschaften:

      * Es ist ein Fehler aufgetreten und der Match-Vorgang ist fehlgeschlagen.

      * Es wurde keine Übereinstimmung gefunden.

      * Übereinstimmung gefunden, aber Produkt als inszeniert veröffentlicht, weil die [Marketplace store ist nicht aktiv](walmart-prerequisites.md#walmart-marketplace-store-status).

### Checkliste für Walmart

Überprüfen Sie nach übereinstimmenden Produkten die aktualisierte Produktliste und überprüfen Sie Produktdetails, Preis und Lagermenge aus der [[!UICONTROL Walmart Marketplace Seller Account Items] Dashboard](https://seller.walmart.com/items-and-inventory/manage-items) , um das aktualisierte Produkt zu überprüfen.

### Fehlerbehebung bei Produktübereinstimmungsfehlern

Wenn der Vorgang der Produktübereinstimmung fehlschlägt, gibt der Walmart Marketplace einen Fehlercode zurück und der Kanal-Manager zeigt den Fehlerstatus in den Informationen zur Produktliste an.

Zeigen Sie die Details der Fehlermeldungen an, indem Sie den Mauszeiger über die **Fehler** Statusbezeichnung. Häufige Fehler, die zurückgegeben werden, sind falsch formatierte Produkt-ID-Werte oder fehlende erforderliche Attribute.

#### Produkt-ID-Werte korrigieren

| Typ | Beschreibung | Beispiel |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, die 12-stellige Zahl einschließlich der Prüfziffer. </br></br>Wenn Ihr UPC weniger als 12 Stellen umfasst, z. B. UPC-E mit 8 Stellen, fügen Sie zur Erfüllung der Anforderung Nullen hinzu. | Ändern von `45678912345` nach `045678912345` |
| GTIN | GTIN-14, die 14-stellige Zahl einschließlich der Prüfziffer. </br></br>Wenn Ihr GTIN weniger als 14 Stellen enthält, fügen Sie führende Nullen hinzu </br>, um die Anforderungen zu erfüllen. | Änderung `456789123456` nach `0045678912345` |
| EAN | GTIN-13, die 13-stellige Zahl einschließlich der Prüfziffer. </br></br>Wenn Ihr EAN weniger als 13 Stellen enthält, fügen Sie den Zeilensprung hinzu. </br>Nullen zur Erfüllung der Anforderung. | Ändern von `4567891234` nach `0004567891234` |

Weitere Informationen zu den Fehler-Codes von Walmart Marketplace finden Sie in der [Walmart Seller-Hilfe](https://sellerhelp.walmart.com/s/guide?article=000005844).

## Hochladen neuer Produktlisten

Verwenden Sie für Produkte, die auf dem Walmart Marketplace nicht übereinstimmen, eine Excel-Vorlage der Walmart-Produktkategorie, um Produktlisten stapelweise hochzuladen. Sie füllen die Walmart-Vorlage mit Produktkatalogdaten, die aus Ihrer Commerce-Instanz exportiert wurden.

Überprüfen Sie Ihren Produktkatalog für neue Produktlisten, um sicherzustellen, dass Produkte, die Sie auf dem Walmart Marketplace verkaufen möchten, über die für Produktlisten im Walmart Marketplace erforderlichen Attribute verfügen.

**Walmart Marketplace listings-Attributanforderungen**

| **Attribut** | **Anforderungsstufe** |
|--------------------------|-----------------------|
| SKU | Erforderlich |
| Produktname | Erforderlich |
| Produkt-ID-Typ | Erforderlich |
| Produkt-ID | Erforderlich |
| Marke | Erforderlich |
| Kurzbeschreibung | Erforderlich |
| Verkaufspreis | Erforderlich |
| Site-Beschreibung | Erforderlich |
| URL des Hauptbilds | Erforderlich |
| Versandgewichtung | Erforderlich |
| Wichtigste Funktionen | Empfohlen |
| Modellnummer | Empfohlen |
| Name des Herstellers | Empfohlen |
| Teilenummer des Herstellers | Empfohlen |
| Größe | Empfohlen |
| Farbe | Empfohlen |
| URL des Hauptbilds | Optional |
| Zusätzliche Bild-URL | Optional |
| Hersteller | Optional |

### Voraussetzungen

* Vergewissern Sie sich, dass Sie die [Walmart-Voraussetzungen](https://docs.google.com/document/d/1bEbCyVLXJQQsbZvEwetJvZKWQJOKoiw5Ia1uB4Bs4uo/edit#heading=h.k2lo9voad1gx).

* Überprüfen Sie in Ihrem Commerce-Produktkatalog, ob die Katalogkonfiguration für die Produkte, die auf dem Walmart Marketplace aufgelistet werden sollen, alle erforderlichen Attribute aufweist und den Inhaltsrichtlinien von Walmart Marketplace entspricht.

* Stellen Sie sicher, dass der Cron-Auftrag ausgeführt wird, um den Exportvorgang abzuschließen.

   * Informationen zu Vor-Ort-Instanzen finden Sie unter [Cron konfigurieren und ausführen](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   * Informationen zur Adobe Cloud-Infrastruktur finden Sie unter [Einrichten von Cron-Aufträgen](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### Erstellen der hochzuladenden Produktdatendatei

1. Von Ihrem [Walmart Seller-Konto](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), laden Sie eine Produktlisten-Vorlage vom Walmart Seller Center herunter.

   * Wählen Sie auf der Seite &quot;Produktkatalogelemente&quot;die Option **[!UICONTROL Add Items]**. Wählen Sie anschließend **[!UICONTROL Add items in bulk]**.

      ![Option &quot;Elemente stapelweise hinzufügen&quot;in der Walmart Marketplace-Elementkonfiguration](assets/walmart-seller-account-add-items-bulk.png)

   * Wählen Sie auf der Download-Seite **[!UICONTROL Full Setup]**. Wählen Sie dann eine Elementkategorie aus und laden Sie die Kategorievorlage herunter.

      ![Kategorievorlagenoption herunterladen in der Walmart Marketplace -Elementkonfiguration](assets/walmart-seller-account-full-setup-download.png)

   * Stellen Sie sicher, dass die Vorlage die erforderlichen und empfohlenen Attribute für die Produktliste enthält.

1. Aus dem [!DNL Commerce] Admin, wählen Sie die Produktdaten aus, die von Ihrer Adobe Commerce-Site exportiert werden sollen.

   * Wählen Sie im Admin die Option [!UICONTROL **System** > Datenübertragung > **Export**].

   * Im [!UICONTROL Export] in der [!UICONTROL Entity Type] Feld, wählen Sie [!UICONTROL **Produkte**].

   * Im [!UICONTROL Entity Attributes] -Tabelle die Auswahlkriterien für den Export von Produktdaten konfigurieren.
   ![Seite &quot;Produktdaten exportieren&quot;im [!UICONTROL Commerce Admin]](assets/walmart-seller-account-full-setup-download.png)

   Verwenden Sie Filter, um die Attributwerte auszuwählen und zu konfigurieren, die für die Produktkategorien gelten, in denen Sie verkaufen. Stellen Sie sicher, dass Walmarts erforderliche und empfohlene Attribute eingeschlossen sind (siehe [Daten exportieren](https://docs.magento.com/user-guide/system/data-export.html) detaillierte Anweisungen finden Sie im Adobe Commerce-Benutzerhandbuch.)

   Um ein Attribut aus dem Export auszuschließen, wählen Sie die [!UICONTROL **Ausschließen**] am Anfang der Zeile.

1. Scrollen Sie zum Ende der Attributtabelle und wählen Sie [!UICONTROL **Weiter**] , um den Datenexport zu starten.

   Die CSV-Exportdatei wird mithilfe von Cron-Aufträgen über eine Nachrichtenwarteschlange verarbeitet und in der `var/export/folder`. (Siehe [Verwalten von Nachrichtenwarteschlangen](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) im *Entwicklerhandbuch für Commerce*.

1. Öffnen Sie die Excel-Vorlage für die Produktkategorie Walmart Marketplace und führen Sie die exportierten Produktdaten mithilfe von Excel-Makros in die Excel-Vorlage zusammen.

1. Laden Sie die Excel-Datei mit den exportierten Produktdaten hoch.

   * Kehren Sie zur Seite &quot;Produktkatalog-Elemente&quot;im [Walmart Seller Center](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   * Auswählen [!UICONTROL **Elemente hinzufügen** > **Stapelweises Hinzufügen von Elementen**].
   * Ziehen Sie die abgeschlossene Tabelle in den Bereich Hochladen .
   * Auswählen [!UICONTROL **Einsenden**].
   * Wählen Sie die [!UICONTROL  **Aktivitäts-Feed**] , um den Fortschritt anzuzeigen.

Eine vollständige Anleitung finden Sie unter [Elemente stapelweise mit Vollartikelspezifikation hinzufügen](https://sellerhelp.walmart.com/s/guide?article=000007680) im [!DNL *Walmart Seller-Hilfe*].
