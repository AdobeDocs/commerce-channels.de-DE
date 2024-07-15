---
title: '[!DNL Amazon Sales Channel] Versionshinweise'
description: Informationen zu allen [!DNL Amazon Sales Channel] Versionen finden Sie in den Versionshinweisen .
feature: Sales Channels, Release Notes
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: df8bbec23d34b53a0e694c924aca5b1ed41e4d08
workflow-type: tm+mt
source-wordcount: '2010'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] Versionshinweise

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] kann auf Instanzen mit Magento Open Source, Adobe Commerce und Adobe Commerce in Cloud-Infrastrukturversionen 2.3.x und 2.4.x installiert werden. Die -Erweiterung wird auf Adobe Commerce 2.1, Magento Open Source 2.2 oder Magento 1 nicht mehr unterstützt.
> <br>Unterstützung ist nur für [!DNL Amazon sales channel] -Versionen 4.0.0 und 4.1.0 in Adobe Commerce 2.3.x verfügbar.
> <br>[!DNL Amazon sales channel] Version 4.2.0+ ist mit Adobe Commerce-Versionen 2.3.x kompatibel, unterstützt wird jedoch nur Adobe Commerce 2.4.x.
>

Diese Versionshinweise beschreiben die erste Version von [!DNL Amazon sales channel] und umfassen:

![Neu](../assets/new.svg) Neue Funktionen
![Korrektur des Problems](../assets/fix.svg) Fehlerbehebungen und Verbesserungen
![Bekanntes Problem](../assets/bug.svg) Bekannte Probleme

Informationen zu Versionierung, Unterstützung und Kompatibilität finden Sie unter [Bevorstehende Versionen](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) .

Unter [Produktverfügbarkeit](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) erfahren Sie, welche Adobe Commerce-Versionen diese Erweiterung unterstützen.

## v4.5.0

*30. August 2023*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg) Das Adobe.IO-API-Gateway wurde hinzugefügt, das von MAGI geändert wurde, um die Authentifizierungssicherheit zu verbessern. `ServicesId` bietet eine neue Benutzeroberfläche zum Verwalten Ihrer Adobe.IO-Anmeldedaten, ähnlich wie andere [Adobe Commerce Services](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html).

>[!NOTE]
>
>Merchants müssen sicherstellen, dass die [privaten und öffentlichen API-Schlüssel](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html) für die Produktion aktualisiert werden.


![Problem behoben](../assets/fix.svg) Es wurde ein Konfigurationseinstellungsproblem identifiziert und der Bestellerstellungsfluss behoben.

## v4.4.4

*7. März 2023*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Problem behoben](../assets/fix.svg) Unterstützung für Adobe Commerce 2.4.6 und PHP 8.2 hinzugefügt.

![Korrektur des Problems](../assets/fix.svg) Reduziertes Rauschen in Protokollen.

![Problem behoben](../assets/fix.svg) Verbesserte Stabilität beim Abrufen von Aktualisierungen.

![Problem behoben](../assets/fix.svg) Der Prozess zum Ausführen einer einzelnen aktionsähnlichen Pull-Aktion oder zum Anwenden über die CLI wurde vereinfacht.

![Problem behoben](../assets/fix.svg) Die Abhängigkeit für `magento/services-connector` wurde aktualisiert.

![Korrektur des Problems](../assets/fix.svg) Korrektur der Synchronisierungsprobleme in Konten des Vereinigten Königreichs mit ungültigem Ländercode.

![Korrektur des Problems](../assets/fix.svg) Die hartcodierte entity_type_id für die Katalogproduktentität verursacht Probleme mit der Magento Price Source.

![Korrektur des Fehlers](../assets/fix.svg) Korrektur des Fehlers, der verhindert hat, dass auch Konten, die in einem Backend aus einer anderen Instanz gelöscht wurden, aus der Benutzeroberfläche gelöscht wurden.

![Korrektur des Fehlers](../assets/fix.svg) Es wurde ein Problem behoben, bei dem einige Warenkorbregeln den Bestellimport verhinderten.

## v4.4.3

*7. März 2023*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Korrektur](../assets/fix.svg) Unterstützung für Adobe Commerce 2.4.4 hinzugefügt.

## v4.4.2

*11. November 2021*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Korrektur](../assets/fix.svg) Aktualisierte Abhängigkeiten zur Unterstützung anderer aktualisierter Erweiterungen.
![Korrektur](../assets/fix.svg) Unterstützung für PHP 8.1 hinzugefügt.

## v4.4.1

*11. November 2021*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Korrektur](../assets/fix.svg) Die Art und Weise, wie Adobe Commerce das Feld _Benutzername_ von Amazon erhält, wurde geändert. Zuvor gab es bei der Bestellerstellung einen Fehler, wenn das Feld _Benutzername_ Sonderzeichen enthielt. Adobe Commerce erhält jetzt die Daten für den _Benutzernamen_ und filtert die Sonderzeichen heraus, damit die Bestellung erfolgreich erstellt werden kann.

## v4.4.0

*9. April 2021*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg) Unterstützung für schreibgeschützten Modus zur Konfiguration hinzugefügt. Siehe [Verkaufskanaleinstellungen](sales-channel-settings.md).

![Korrektur](../assets/fix.svg) Der Datenfluss wurde geändert, sodass mehrere Kopien derselben Instanz Aktualisierungen gleichzeitig abrufen können.

![Korrektur](../assets/fix.svg) Der Synchronisierungsprozess für die Kontoinformationen wurde geändert. Es wurde ein Cron-Auftrag zur Synchronisierung mit einem Remote-Konto hinzugefügt und dieselben Funktionen zu den CLI-Befehlen hinzugefügt.

![Korrektur](../assets/fix.svg) Befehlsargumente und -flags für CLI wurden hinzugefügt, um eine präzisere Kontrolle zu ermöglichen.

![Fehlerbehebung](../assets/fix.svg) Korrektur des Source-Hintergrundaufgaben (cron) in der Systemkonfiguration.

![Korrektur](../assets/fix.svg) Korrektur des Fehlers, der die Erstellung von Bestellungen verhinderte, wenn der Ländercode auf Puerto Rico (PR) festgelegt war.

## v4.3.0

*3. März 2021*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-xxxx-->Die Funktion _Bestelldetails_ wurde neu gestaltet und verlässt sich nicht mehr auf die Einstellung _Bestellungen importieren_ . Bestelldetails werden jetzt in der Amazon Sales Channel-Oberfläche für alle Bestellungen angezeigt.

![Korrektur](../assets/fix.svg) Im Menü _[!UICONTROL Marketing]_im Admin wurde der Name von_[!UICONTROL Amazon]_ in _[!UICONTROL Amazon Sales Channel]_geändert.

![Bekanntes Problem](../assets/bug.svg) **Wichtig**: Bekannte Probleme mit Adobe Commerce 2.4.0-Kompatibilität wurden in der Adobe Commerce-Version 2.4.1 behoben.

- Amazon-Cron-Prozesse im Status &quot;`error`&quot;
- Die Installation mit Commerce 2.4.0 schlägt beim Erstellen von Datenspeichern in der Datenbank fehl
- Das Erstellen eines Produkts schlägt fehl, wenn MSI installiert ist

## v4.2.0

*3. März 2021*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

Wenn Sie eine frühere Version von [!DNL Amazon sales channel] installiert haben und versuchen, Ihre Adobe Commerce auf Version 2.4.0 zu aktualisieren, werden Sie aufgefordert, die Erweiterung zu aktualisieren, bevor Sie das Adobe Commerce-Update abschließen können.

![Bekanntes Problem](../assets/bug.svg) Wenn [!DNL Amazon sales channel] 4.2.0 in Version 2.4.0 integriert ist und [Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/introduction.html?lang=en) aktiviert ist, gibt es ein bekanntes Problem, das das Hinzufügen von Produkten in Ihren Commerce-Katalog verhindert. Dieses Problem wird in einer zukünftigen Commerce-Version behoben.

![Neu](../assets/new.svg) [!DNL Amazon sales channel] wurde verbessert, um textbasierte Adressdaten zu akzeptieren und sie mit standardisierten Adressformaten wie Stadt, Bundesland und Postleitzahl abzugleichen. Durch diese Aktualisierung können Bestell- und Versanddaten ohne Adressfehler mit Amazon synchronisiert (synchronisiert) werden.<br/>Beispielsweise gibt ein Käufer die Stadt, das Bundesland, die Postleitzahl als `Escondido, californiA 92025-1501` ein. Amazon Sales Channel importiert und ordnet die Daten dem Standardformat `Escondido, CA 92025` zu und synchronisiert sie dann in diesem standardisierten Format wieder mit Amazon.

![Neu](../assets/new.svg) Unterstützung für PHP 7.4 hinzugefügt.

![Neu](../assets/new.svg) <!--CHAN-4334-->Unterstützung für Adobe Commerce 2.4.x hinzugefügt. Frühere Versionen sind möglicherweise mit Commerce 2.4.x kompatibel, werden jedoch nicht unterstützt. Informationen zur Versionskompatibilität finden Sie unter [Bevorstehende Versionen](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) . Amazon Sales Channel muss auf Version 4.2.0 aktualisiert werden, bevor das Adobe Commerce 2.4.0 Update abgeschlossen werden kann.

![Korrektur](../assets/fix.svg) <!--CHAN-4431-->Korrektur eines Problems, das dazu führte, dass für britische Kunden der Fehler _Zugriff verweigert_ angezeigt wurde.

![Korrektur des Fehlers](../assets/fix.svg) <!--CHAN-4394-->Korrektur eines Fehlers, der verhindert hat, dass der Versandstatus von Amazon mit der entsprechenden Commerce-Bestellung synchronisiert wurde, sodass der Versandstatus der Bestellung in Commerce als `Pending` und in Amazon als `Unshipped` &quot;gesperrt&quot;wurde. Mit der neuen standardisierten Adressenfunktion wurden diese Versandstatusfehler behoben.

![Korrigieren Sie](../assets/fix.svg) <!--ticket#-->Die Synchronisation der Bestellungen (Synchronisation) wurde aktualisiert, um fehlgeschlagene Bestellimporte zu ignorieren. Dadurch werden mehrere Synchronisierungsversuche reduziert und nachfolgende Importe können verarbeitet werden, wobei alle fünf Minuten Bestellsynchronisierungsanforderungen gesendet werden. Synchronisierungsfehler werden weiterhin im Fehlerprotokoll aufgezeichnet, aber als &quot;verarbeitet&quot;markiert, um weitere Protokollierungsfunktionen zu ermöglichen. Außerdem entfernt [!DNL Amazon sales channel] jetzt automatisch überschüssige Daten, die für Bestellungen erfasst wurden, die nicht in Commerce erstellt werden.

![Fehlerbehebung](../assets/fix.svg) Die Fehlerprotokollierung wurde aktualisiert, um weitere Informationen zu Fehlern bei nicht abgefangenen Ausnahmen und Erweiterungen zu sammeln.

![Korrektur](../assets/fix.svg) <!--ticket#-->Korrektur eines Problems, das dazu führte, dass die anfängliche Synchronisierung der _niedrigsten Preis_ -Daten aufgrund eines fehlenden _Preis_ -Werts fehlschlug.

![Korrektur von ](../assets/fix.svg) <!--CHAN-4410-->Korrektur von Problemen, die in der Ansicht _Amazon-Bestellungen_ zu Filterfehlern führten, wenn das Datumsbereichsfeld leer gelassen wurde.

![Korrektur](../assets/fix.svg) <!--CHAN-4439-->Korrektur eines Fehlers, der zu quantitationsbezogenen Fehlern bei Bestell- und Fulfillment-Synchronisierungen führte. Die Erweiterung rundet nun die als Dezimalzahl eingegebenen Mengenwerte ab, bevor sie mit Amazon synchronisiert wird.<br/> Wenn beispielsweise ein Händler manuell die Menge `2.5` eingibt, rundet die Erweiterung den Wert auf `2` ab und synchronisiert dann die aktualisierte Menge mit Amazon.

## v4.1.0

*7. Mai 2020*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg) <!--4247, 4230-->Der Bestellimportierungsprozess wurde an die Commerce-Bestellanforderungen angepasst. Durch diese Änderungen werden Probleme behoben, durch die Commerce die entsprechende Bestellung für eine importierte Bestellung nicht erstellen konnte. Informationen zu Bestellblockern und Lösungen finden Sie unter [Verwalten von Bestellungen](managing-orders.md) .

![Neu](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324--> Der Abschnitt _Letzte Bestellungen_ des Store-Dashboards wurde aktualisiert und eine neue Ansicht _Alle Bestellungen_ hinzugefügt, in der alle Ihre Amazon-Bestellungen angezeigt werden, einschließlich Filteroptionen und Paginierung zum Anzeigen weiterer Bestellungen. Siehe [Amazon Store Dashboard](amazon-store-dashboard.md) und [Anzeigen von Amazon-Bestellungen](amazon-orders-all.md).

![Neu](../assets/new.svg) Die Spalte _[!UICONTROL Order Notes]_der neu gestalteten Tabelle_[!UICONTROL Amazon Orders]_ wurde sowohl in _[!UICONTROL Recent Orders]_als auch in_[!UICONTROL All Orders]_ -Ansichten hinzugefügt. _[!UICONTROL Order Notes]_teilen Sie dem Händler mit, dass beim Import der Bestellung ein Problem vorliegt. Siehe [Anzeigen von Amazon-Bestellungen](amazon-orders-all.md).

![Neu](../assets/new.svg) <!--CHAN-4013-->Die Produktbedingungsparameter wurden aktualisiert, um sie an das Programm [Amazon Renewed](https://sell.amazon.com/programs/renewed) anzupassen. Siehe [Erneute Produkte](renewed-products.md).

![Neu](../assets/new.svg) <!--CHAN-3680-->Aktualisierte [Amazon-Auftragsdetails](amazon-order-details.md) mit &quot;allgemeinen Daten&quot;für Bestellungen, die von Amazon erfüllt werden. Siehe [Erfüllt durch ](fulfilled-by.md).

![Korrektur](../assets/fix.svg) <!--CHAN-4069-->Korrektur eines Problems, das dazu führte, dass Symbole auf der Store-Karte verzerrt dargestellt wurden.

![Korrektur](../assets/fix.svg) <!--CHAN-4165-->Korrektur eines Fehlers, der verhindert hat, dass der Bildschirm _Anmeldung_ angezeigt wird, nachdem die Sitzung beendet wurde.

![Korrektur](../assets/fix.svg) <!--CHAN-4211-->Korrektur eines Problems, das dazu führte, dass der Amazon-Bestellsteuerbetrag nicht in die neue Commerce-Bestellung importiert werden konnte.

![Korrektur](../assets/fix.svg) <!--CHAN-4234-->Korrektur eines Fehlers, der dazu führte, dass die im Store-Dashboard angezeigten Umsatzsummen Bestellungen in den Status `Canceled` oder `Error` enthielten.

![Korrektur](../assets/fix.svg) <!--CHAN-4326-->Korrektur eines Fehlers, der dazu führte, dass bei Erweiterungen von Drittanbietern, die _Magento Shipping_ -Methoden zum Erstellen von Bestellungen verwenden, Bestellfehler beim Bestellimport verursacht wurden.

![Korrektur](../assets/fix.svg) <!--CHAN-4357-->Korrektur eines Problems, das bei der Ausführung der Cron-Synchronisierung Fehler verursachte. Dem CLI-Befehl wurde eine Sperre hinzugefügt, die verhindert, dass zwei Cron-Aufträge gleichzeitig synchronisiert werden.

![Fehlerbehebung](../assets/fix.svg) Aktualisierte Richtlinie zur Inhaltssicherheit für die Unterstützung mit Commerce Version 2.3.5.

## v4.0.0

*25. März 2020*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0 wird für Adobe Commerce 2.3.5 nicht unterstützt. Um Adobe Commerce 2.3.5 zu unterstützen, aktualisieren Sie auf Amazon Sales Channel 4.1.0.

![Neu](../assets/new.svg) Eine neue [Amazon-Sales Channel](amazon-sales-channel-home.md)-Homepage mit verbesserter &quot;Kartenansicht&quot;für Ihre Store-Informationen wurde eingeführt.

![Neu](../assets/new.svg) Ein neues [Dashboard speichern](amazon-store-dashboard.md) wurde mit Auflistungs-, aktuellen Bestellungen- und Store-Einstellungsinformationen eingeführt.

![Neu](../assets/new.svg): Es wurde ein einfacherer, optimierter [Onboarding-Prozess](amazon-onboarding-home.md) und [Standardspeichereinstellungen](default-store-settings.md) eingeführt, um Ihre Stores schneller zu integrieren.

![Bekanntes Problem](../assets/bug.svg) <!--CHAN-4102--> Wenn [Attribute erstellen](managing-attributes.md) zum Importieren von Bildern aus Listen und **Store-Ansichten** auf `All Store Views (Global)` festgelegt ist, liegt ein bekanntes Problem vor, das den Import von Bildern in alle Store-Ansichten verhindert. Wenn Sie die Einstellung für **Store-Ansichten (zum Importieren von Werten in)** in einen bestimmten Store ändern, werden die Bilder für diesen Store importiert.

## v3.0.1

*11. November 2019*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Korrektur](../assets/fix.svg) **Numerische Feldeinstellungen**: <!--CHAN-3779-->Felder, für die ein numerischer Wert erforderlich ist, wurden aktualisiert, sodass nur numerische Zeichen zulässig sind. Beispiel: Preisregeleinstellungen > Feld &quot;Anpassungsbetrag&quot;

![Korrektur](../assets/fix.svg) **Benutzerhandbuch-Links**: <!--CHAN-3778-->Falsche _Benutzerhandbuch_-Links wurden korrigiert.

![Korrektur](../assets/fix.svg) **Duplizieren von Amazon-Listen**: <!--CHAN-3593-->Ein zuvor gemeldetes Problem, das zu Duplikat-Amazon-Auflistungen führt, wurde jetzt korrigiert. Vor dieser Version hat die Erweiterung den Ländercode für die Amazon-Region zum SKU-Wert beim Import von Listen hinzugefügt. Die Liste stimmte mit dem Katalogelement überein, aber die Erweiterung erstellte eine neue, doppelte Liste mit der angehängten SKU. Mit dieser Version ändert die Erweiterung die SKU für importierte Listen nicht und an vorhandenen Listen werden keine Änderungen vorgenommen. Sie können die Option [!UICONTROL End Listing(s)] in Amazon verwenden, um doppelte Listen zu entfernen.

## v3.0.0

*7. Oktober 2019*

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

![Neu](../assets/new.svg) **Amazon UK Marketplace jetzt verfügbar**: Benutzer können beim Erstellen und Integrieren eines Commerce-Stores den britischen Marketplace auswählen. Dieses Upgrade für Großbritannien beinhaltet zusätzliche Unterstützung für:

- [MwSt.-Berechnungsdienst für Amazon](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [Produktsteuercode](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"} Informationen.

![Neu](../assets/new.svg) **Verbesserte Protokollierung**: <!--CHAN-3642, 3672--> Die Funktion **Debug-Protokollierung aktivieren** wurde implementiert, um zusätzliche Synchronisierungsdaten zu erfassen, wenn eine Fehlerbehebung erforderlich ist. Weitere Informationen finden Sie unter dem Thema [Sales Channel Settings](https://experienceleague.adobe.com/docs/commerce-admin/config/sales-channels.html) in der Konfigurationsreferenz.

![Korrektur](../assets/fix.svg) **Produktkatalog**: <!--CHAN-3687-->Korrektur eines Fehlers, der verhinderte, dass mit einer Amazon-Liste importierte Bilder auf das entsprechende Commerce-Katalogprodukt angewendet wurden.

![Fehlerbehebung](../assets/fix.svg) **Auftragserstellung**: <!--CHAN-3708-->Korrektur eines Problems, das dazu führte, dass Commerce keine Bestellungen für eine Amazon-Bestellung erstellte, die nicht mit einem Commerce-Katalogprodukt übereinstimmte.

![Bekanntes Problem](../assets/bug.svg) **Duplizieren von Amazon-Listen**: <!--CHAN-3593-->Dieses Problem führt dazu, dass der Katalog ein Element für eine importierte Auflistung erstellt, wobei dieselbe SKU verwendet wird, am Ende jedoch ein Regionscode hinzugefügt wird. Amazon verarbeitet dann die geänderte SKU als neues Element und erstellt eine Liste. Dieses Problem wird in einer zukünftigen Version behoben.

## v2.0.0

[!BADGE Unterstützt]{type=Informative tooltip="Unterstützt"}

>[!NOTE]
>
>Version 1.0.0 war nur in begrenzter Version verfügbar.

![Neu](../assets/new.svg) **Vereinfachtes Onboarding und Warten**: Fügen Sie Ihr Amazon-Kundenkonto hinzu und integrieren Sie es in einen Schritt-für-Schritt-Prozess mit detaillierten Anweisungen, die über den Administrator verfügbar sind. Verwalten Sie Ihre Stores, Konten und aufgelisteten Produkte über ein Dashboard.

![Neu](../assets/new.svg) **Unterstützung mehrerer Konten**: Verwalten und überwachen Sie mehrere Amazon-Marken und Marketplace-Regionen über den Administrator.

![Neu](../assets/new.svg) **Intelligente Preise**: Legen Sie automatisierte Neupreisregeln fest, um Ihre Chancen für die begehrte Buy Box zu erhöhen. Stellen Sie die Preise so ein, dass sie sich dynamisch an den aktuellen Buy Box-Preis oder an die niedrigste Preisgestaltung des Konkurrenten anpassen. Legen Sie Beschränkungen für die Neuberechnung fest, um Ihre Marge zu schützen.

![Neu](../assets/new.svg) **Listing Management**: Automatisieren Sie Produktlisten und synchronisieren Sie Ihren Commerce-Katalog mithilfe von Listening-Regeln mit dem Amazon Marketplace. Fügen Sie spezifische Überschreibungen hinzu, um Ihre Angebote optimal zu steuern. Überwachen und verwalten Sie alle Ihre Einträge direkt über den Administrator.

![Neu](../assets/new.svg) **Konsistente Inventory management**: Lassen Sie die Lagerbestandsmengen in Commerce und Amazon konstant synchronisieren.

![Neu](../assets/new.svg) **Auftrags- und Ausführungsverwaltung**: Verfolgen Sie Amazon-Bestellungen über das Dashboard mit nahtlosen Kommunikations- und Bestandsaktualisierungen. Vervollständigen und verfolgen Sie die Auftragslieferungen, die von Amazon, dem Händler oder einer Kombination von Methoden erfüllt wurden.

![Bekanntes Problem](../assets/bug.svg) Es kann zu längeren Wartezeiten kommen, um die Produktmengen zu aktualisieren. Die Synchronisierung von Aktualisierungen für die Produktmenge kann etwa zwei Stunden dauern.

![Bekanntes Problem](../assets/bug.svg) Importierte Bestellungen können einen Typ von _Prime_ oder _Premium_ Bestellungen aufweisen. Sie sollten diese Bestellungen in Ihrem Amazon-Verkaufskonto überprüfen.

![Bekanntes Problem](../assets/bug.svg) Nicht infrage kommende gebündelte Produkte werden möglicherweise als für die Aufnahme in Amazon infrage kommende Produkte angezeigt. Eines der Produkte innerhalb des gebündelten Produkts ist möglicherweise nicht förderfähig. Wenn Probleme auftreten, überprüfen Sie den Berechtigungsstatus für gebündelte Produkte.

![Bekanntes Problem](../assets/bug.svg) Bei der Verwendung von Inventory management für Commerce 2.3.x wird bei der Erstellung einer Bestellung möglicherweise keine partielle Neuindizierung des Lagers Trigger. Die verkaufbare Menge berechnet stündlich neu, was während dieses Aktualisierungsintervalls zu einer Überschreibung führen kann.
