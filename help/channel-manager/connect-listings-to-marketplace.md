---
title: Listen mit Walmart verbinden
description: Verbinden von Auflistungen für Commerce-Produkte mit [!DNL Walmart Marketplace]um den Verkauf zu beginnen.
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: 418bb6a91817f49f3c3ae39a8d26370bfeb39099
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Listen mit Walmart verbinden

Wie andere Marktplätze, [!DNL Walmart] Ermöglicht es Drittanbietern, von anderen Anbietern verkaufte Artikel aufzulisten.

- [!DNL Walmart Marketplace] verwendet Produktidentifikatoren wie UPC und GTIN, um Produkte mit bestehenden abzugleichen [!DNL Walmart Marketplace] Auflistungen.

- Für passende Produkte listet der Walmart Marketplace Aktualisierungen auf, um das Commerce-Produktangebot bei der Verbindung eines Produkts von einzubeziehen. [!DNL Channel Manager].

- Normalerweise erscheinen Produktangebote mit den niedrigsten Preisen zuerst in der [!DNL Walmart Marketplace] Auflistung, aber auch andere Faktoren wie Bewertungen wirken sich auf die Platzierung aus.

## Produkte abgleichen

Wenn Sie Produkte abgleichen, sendet der Kanal-Manager die Produktdaten an [!DNL Walmart Marketplace] , um nach vorhandenen Listen mit Attributwerten zu suchen, die mit dem zugeordneten Commerce-Produktattribut übereinstimmen. Übereinstimmungskriterien werden durch die [attribute-mapping-Konfiguration](map-catalog-attributes.md) für Ihren Store-Kanal.

Wenn eine Übereinstimmung gefunden wird, wird die vorhandene Produktliste aktualisiert, um Ihr Angebot hinzuzufügen.

### Voraussetzungen

Bevor Sie Produkte zuordnen, überprüfen Sie, ob die Produktkatalog-Attributwerte die Walmart-Anforderungen erfüllen, und konfigurieren Sie die Produktattributeinstellungen. Siehe [Katalogattribute zuordnen](map-catalog-attributes.md).

#### Produkte auswählen und abgleichen

1. Öffnen Sie einen verbundenen Vertriebskanal.

1. Von **[!UICONTROL Listings]**, wählen Sie Produkte für die Übereinstimmung aus, die in *[!UICONTROL Draft]* Status.

   ![Produkte aus Listen auswählen und zur Übereinstimmung senden](assets/products-in-marketplace-sales-channel.png)

1. Auswählen **[!UICONTROL Match Products]**.

   Eine Meldung gibt die Anzahl der Produkte an, die zum Abgleich gesendet wurden.

   ![Produkte an den verbundenen Vertriebskanal senden](assets/products-submitted-for-matching.png)

   Der Status für ausgewählte Produkte ändert sich in [!UICONTROL *Verarbeitung*] bis der Match-Vorgang abgeschlossen ist. Es kann bis zu 30 Minuten dauern, bis Walmart Marketplace den Match-Vorgang abschließt.

### Prüfen des Übereinstimmungsstatus

Nachdem die Übereinstimmung abgeschlossen ist, wählen Sie die **[!UICONTROL Refresh products]** , um den aktuellen Produktstatus anzuzeigen. *Übereinstimmung* oder *Fehler*.

- **[!UICONTROL Match]** gibt an, dass das Produkt erfolgreich abgeglichen wurde. Ihr Produktangebot war mit einer vorhandenen Walmart Marketplace-Liste verbunden. Wenn die Variable [Marketplace store ist nicht aktiv](walmart-requirements.md#walmart-marketplace-store-status), *[!UICONTROL Staged for Match]* wird im *[!UICONTROL Status detail]* Spalte. Staging-Produkte werden automatisch verbunden, wenn die [!DNL Walmart Marketplace] store aktiviert ist.

- **[!UICONTROL Error]** gibt an, dass der Match-Vorgang aufgrund eines der folgenden Probleme fehlgeschlagen ist:

   - [!DNL Channel Manager] konnte aufgrund eines Verbindungsproblems nicht zur Übereinstimmung gesendet werden.

   - Es wurde keine Übereinstimmung gefunden.

   - Übereinstimmung gefunden, die Liste kann jedoch nicht verknüpft werden, weil [!DNL Walmart Marketplace] einen Fehlercode zurückgegeben. Siehe **[!UICONTROL Error Description]** für Informationen zum Problem.

### Checkliste für Walmart

Überprüfen Sie nach übereinstimmenden Produkten die aktualisierte Produktliste und überprüfen Sie Produktdetails, Preis und Lagermenge aus der [[!UICONTROL Walmart Marketplace Seller Account Items] Dashboard](https://seller.walmart.com/items-and-inventory/manage-items) , um das aktualisierte Produkt zu überprüfen.

### Fehlerbehebung bei Produktübereinstimmungsfehlern

Wenn der Vorgang zur Produktanpassung mit einem Fehler fehlschlägt, wird die Fehlermeldung im *[!UICONTROL Status detail]* in der Spalte [!UICONTROL Channel Manager] Produktliste.

Häufige Fehler, die zurückgegeben werden, sind falsch formatierte Produkt-ID-Werte oder fehlende erforderliche Attribute.

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

- Vergewissern Sie sich, dass Sie die [Walmart-Anforderungen](walmart-requirements.md).

- Überprüfen Sie in Ihrem Commerce-Produktkatalog, ob die Katalogkonfiguration für die Produkte, die auf dem Walmart Marketplace aufgelistet werden sollen, alle erforderlichen Attribute aufweist und den Inhaltsrichtlinien von Walmart Marketplace entspricht.

- Stellen Sie sicher, dass der Cron-Auftrag ausgeführt wird, um den Exportvorgang abzuschließen.

   - Informationen zu Vor-Ort-Instanzen finden Sie unter [Cron konfigurieren und ausführen](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   - Informationen zur Adobe Cloud-Infrastruktur finden Sie unter [Einrichten von Cron-Aufträgen](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### Erstellen der hochzuladenden Produktdatendatei

1. Von Ihrem [Walmart Seller-Konto](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), laden Sie eine Produktlisten-Vorlage vom Walmart Seller Center herunter.

   - Wählen Sie auf der Seite &quot;Produktkatalogelemente&quot;die Option **[!UICONTROL Add Items]**. Wählen Sie anschließend **[!UICONTROL Add items in bulk]**.

      ![Option &quot;Elemente stapelweise hinzufügen&quot;in der Walmart Marketplace-Elementkonfiguration](assets/walmart-seller-account-add-items-bulk.png)

   - Wählen Sie auf der Download-Seite **[!UICONTROL Full Setup]**. Wählen Sie dann eine Elementkategorie aus und laden Sie die Kategorievorlage herunter.

      ![Kategorievorlagenoption herunterladen in der Walmart Marketplace -Elementkonfiguration](assets/walmart-seller-account-full-setup-download.png)

   - Stellen Sie sicher, dass die Vorlage die erforderlichen und empfohlenen Attribute für die Produktliste enthält.

1. Aus dem [!DNL Commerce] Admin, wählen Sie die Produktdaten aus, die von Ihrer Adobe Commerce-Site exportiert werden sollen.

   - Wählen Sie im Admin die Option [!UICONTROL **System** > Datenübertragung > **Export**].

   - Im [!UICONTROL Export] in der [!UICONTROL Entity Type] Feld, wählen Sie [!UICONTROL **Produkte**].

   - Im [!UICONTROL Entity Attributes] -Tabelle die Auswahlkriterien für den Export von Produktdaten konfigurieren.
   ![Seite &quot;Produktdaten exportieren&quot;im [!UICONTROL Commerce Admin]](assets/walmart-seller-account-full-setup-download.png)

   Verwenden Sie Filter, um die Attributwerte auszuwählen und zu konfigurieren, die für die Produktkategorien gelten, in denen Sie verkaufen. Stellen Sie sicher, dass Walmarts erforderliche und empfohlene Attribute eingeschlossen sind (siehe [Daten exportieren](https://docs.magento.com/user-guide/system/data-export.html) detaillierte Anweisungen finden Sie im Adobe Commerce-Benutzerhandbuch.)

   Um ein Attribut aus dem Export auszuschließen, wählen Sie die [!UICONTROL **Ausschließen**] am Anfang der Zeile.

1. Scrollen Sie zum Ende der Attributtabelle und wählen Sie [!UICONTROL **Weiter**] , um den Datenexport zu starten.

   Die CSV-Exportdatei wird mithilfe von Cron-Aufträgen über eine Nachrichtenwarteschlange verarbeitet und in der `var/export/folder`. (Siehe [Verwalten von Nachrichtenwarteschlangen](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) im *Entwicklerhandbuch für Commerce*.

1. Öffnen Sie die Excel-Vorlage für die Produktkategorie Walmart Marketplace und führen Sie die exportierten Produktdaten mithilfe von Excel-Makros in die Excel-Vorlage zusammen.

1. Laden Sie die Excel-Datei mit den exportierten Produktdaten hoch.

   - Kehren Sie zur Seite &quot;Produktkatalog-Elemente&quot;im [Walmart Seller Center](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   - Auswählen [!UICONTROL **Elemente hinzufügen** > **Stapelweises Hinzufügen von Elementen**].
   - Ziehen Sie die abgeschlossene Tabelle in den Bereich Hochladen .
   - Auswählen [!UICONTROL **Einsenden**].
   - Wählen Sie die [!UICONTROL  **Aktivitäts-Feed**] , um den Fortschritt anzuzeigen.

Eine vollständige Anleitung finden Sie unter [Elemente stapelweise mit Vollartikelspezifikation hinzufügen](https://sellerhelp.walmart.com/s/guide?article=000007680) im [!DNL *Walmart Seller-Hilfe*].
