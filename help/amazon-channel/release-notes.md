---
title: '''[!DNL Amazon Sales Channel] Versionshinweise'
description: Informationen zu allen [!DNL Amazon Sales Channel] veröffentlicht.
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: 3b2f60ad2796ee1fdc8808fc0941d76a603b2213
workflow-type: tm+mt
source-wordcount: '1924'
ht-degree: 0%

---

# Versionshinweise

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] kann auf Instanzen mit Magento Open Source, Adobe Commerce und Adobe Commerce in den Cloud-Infrastrukturversionen 2.3.x und 2.4.x installiert werden. Die -Erweiterung wird in Adobe Commerce 2.1, Magento Open Source 2.2 oder Magento 1 nicht mehr unterstützt.
> <br>Support ist verfügbar für [!DNL Amazon sales channel]  Versionen 4.0.0 und 4.1.0 nur für Adobe Commerce 2.3.x.
> <br>[!DNL Amazon sales channel] Version 4.2.0+ ist mit Adobe Commerce-Versionen 2.3.x kompatibel, unterstützt wird jedoch nur Adobe Commerce 2.4.x.

Diese Versionshinweise beschreiben die erste Version von [!DNL Amazon sales channel] und umfassen:

![Neu](../assets/new.svg) Neue Funktionen
![Problem behoben](../assets/fix.svg) Fehlerbehebungen und Verbesserungen
![Bekanntes Problem](../assets/bug.svg) Bekannte Probleme

Siehe [Bevorstehende Versionen](https://devdocs.magento.com/release/){target="_blank"} für Versionierung, Unterstützung und Kompatibilität.

## v4.4.4

*7. März 2023*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Problem behoben](../assets/fix.svg) Unterstützung für Adobe Commerce 2.4.6 und PHP 8.2 hinzugefügt.

![Problem behoben](../assets/fix.svg) Geräuschminderung in Protokollen.

![Problem behoben](../assets/fix.svg) Verbesserte Stabilität beim Abrufen von Aktualisierungen.

![Problem behoben](../assets/fix.svg) Der Prozess für die Ausführung einer einzelnen aktionsähnlichen Pull-Methode oder für die Anwendung über die CLI wurde vereinfacht.

![Problem behoben](../assets/fix.svg) Die Abhängigkeit für `magento/services-connector`.

![Problem behoben](../assets/fix.svg) Synchronisierungsprobleme in Konten des Vereinigten Königreichs mit ungültigem Ländercode wurden behoben.

![Problem behoben](../assets/fix.svg) Die hartcodierte entity_type_id für die Katalogproduktentität verursacht Probleme mit der Magento-Preisquelle.

![Problem behoben](../assets/fix.svg) Es wurde ein Fehler behoben, der verhinderte, dass Konten, die in einem Backend aus einer anderen Instanz gelöscht wurden, auch aus der Benutzeroberfläche gelöscht wurden.

![Problem behoben](../assets/fix.svg) Es wurde ein Problem behoben, bei dem einige Warenkorbregeln den Bestellimport verhinderten.

## v4.4.3

*7. März 2023*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Fehlerbehebung](../assets/fix.svg) Adobe Commerce 2.4.4 wird nun unterstützt.

## v4.4.2

*11. November 2021*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Fehlerbehebung](../assets/fix.svg) Aktualisierte Abhängigkeiten zur Unterstützung anderer aktualisierter Erweiterungen.
![Fehlerbehebung](../assets/fix.svg) Unterstützung für PHP 8.1 hinzugefügt.

## v4.4.1

*11. November 2021*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Fehlerbehebung](../assets/fix.svg) Die Art und Weise, wie Adobe Commerce die _Benutzername_ aus Amazon. Zuvor gab es bei der Auftragserstellung einen Fehler, wenn die Variable _Benutzername_ -Feld Sonderzeichen enthielt. Adobe Commerce erhält jetzt die _Benutzername_ Daten und filtert die Sonderzeichen heraus, damit die Bestellung erfolgreich erstellt werden kann.

## v4.4.0

*9. April 2021*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Neu](../assets/new.svg) Unterstützung für schreibgeschützten Modus zur Konfiguration hinzugefügt. Siehe [Vertriebskanaleinstellungen](sales-channel-settings.md).

![Fehlerbehebung](../assets/fix.svg) Der Datenfluss wurde geändert, sodass mehrere Kopien derselben Instanz Aktualisierungen gleichzeitig abrufen können.

![Fehlerbehebung](../assets/fix.svg) Synchronisierungsprozess für Kontoinformationen wurde geändert. Es wurde ein Cron-Auftrag zur Synchronisierung mit einem Remote-Konto hinzugefügt und dieselben Funktionen zu den CLI-Befehlen hinzugefügt.

![Fehlerbehebung](../assets/fix.svg) CLI-Befehlsargumente und -Flags wurden hinzugefügt, um eine präzisere Steuerung zu ermöglichen.

![Fehlerbehebung](../assets/fix.svg) Die Quelle der Hintergrundaufgaben (cron) in der Systemkonfiguration wurde korrigiert.

![Fehlerbehebung](../assets/fix.svg) Korrektur des Fehlers, der die Erstellung von Bestellungen verhinderte, wenn der Ländercode auf Puerto Rico (PR) gesetzt war.

## v4.3.0

*3. März 2021*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-xxxx-->Die _Bestelldetails_ wurde neu gestaltet und verlässt sich nicht mehr auf die _Bestellungen importieren_ -Einstellung. Bestelldetails werden jetzt in der Amazon Sales Channel-Benutzeroberfläche für alle Bestellungen angezeigt.

![Fehlerbehebung](../assets/fix.svg) Im _[!UICONTROL Marketing]_im Admin-Menü wurde der Name geändert von_[!UICONTROL Amazon]_ nach _[!UICONTROL Amazon Sales Channel]_.

![Bekanntes Problem](../assets/bug.svg) **Wichtig**: Bekannte Probleme mit der Kompatibilität mit Adobe Commerce 2.4.0 wurden in der Adobe Commerce-Version 2.4.1 behoben.

- Amazon-Cron-Prozesse in `error` state
- Die Installation mit Commerce 2.4.0 schlägt beim Erstellen von Stores in der Datenbank fehl
- Das Erstellen eines Produkts schlägt fehl, wenn MSI installiert ist

## v4.2.0

*3. März 2021*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

Wenn Sie eine frühere [!DNL Amazon sales channel] -Version installiert sind und versuchen, Ihre Adobe Commerce auf Version 2.4.0 zu aktualisieren, werden Sie aufgefordert, die -Erweiterung zu aktualisieren, bevor Sie das Adobe Commerce-Update abschließen können.

![Bekanntes Problem](../assets/bug.svg) Wann [!DNL Amazon sales channel] 4.2.0 ist in Version 2.4.0 integriert und [Inventory management](https://docs.magento.com/user-guide/catalog/inventory.html) aktiviert ist, gibt es ein bekanntes Problem, das das Hinzufügen von Produkten in Ihren Commerce-Katalog verhindert. Dieses Problem wird in einer zukünftigen Commerce-Version behoben.

![Neu](../assets/new.svg) [!DNL Amazon sales channel] wurde verbessert, um textbasierte Adressdaten zu akzeptieren und sie mit standardisierten Adressformaten wie Stadt, Bundesland und Postleitzahl abzugleichen. Durch diese Aktualisierung können Bestell- und Versanddaten ohne Adressfehler mit Amazon synchronisiert (synchronisiert) werden.<br/>Beispielsweise gibt ein Käufer die Stadt, das Bundesland und die Postleitzahl als `Escondido, californiA 92025-1501`. Amazon Sales Channel importiert die Daten und stimmt sie mit dem Standardformat überein als `Escondido, CA 92025`und synchronisiert sie dann wieder mit Amazon in diesem standardisierten Format.

![Neu](../assets/new.svg) Unterstützung für PHP 7.4 hinzugefügt.

![Neu](../assets/new.svg) <!--CHAN-4334-->Adobe Commerce 2.4.x wird nun unterstützt. Frühere Versionen sind möglicherweise mit Commerce 2.4.x kompatibel, werden jedoch nicht unterstützt. Siehe [Bevorstehende Versionen](https://devdocs.magento.com/release/){:target=&quot;_blank&quot;} für Versionskompatibilität. Amazon Sales Channel muss auf Version 4.2.0 aktualisiert werden, bevor das Adobe Commerce 2.4.0 Update abgeschlossen werden kann.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4431-->Korrektur eines Problems, das zu einem _Zugriff verweigert_ Fehler für Kunden aus Großbritannien.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4394-->Fehlerkorrektur - Der Versandstatus von Amazon kann jetzt mit der entsprechenden Commerce-Bestellung synchronisiert werden, sodass der Versandstatus der Bestellung als `Pending` im Handel und `Unshipped` in Amazon. Mit der neuen standardisierten Adressfunktion wurden diese Versandstatusfehler behoben.

![Fehlerbehebung](../assets/fix.svg) <!--ticket#-->Die Synchronisierung der Reihenfolge wurde aktualisiert, um fehlgeschlagene Bestellimporte zu ignorieren. Dadurch werden mehrere Synchronisierungsversuche reduziert und nachfolgende Importe können verarbeitet werden, wobei alle fünf Minuten Bestellsynchronisierungsanforderungen gesendet werden. Synchronisierungsfehler werden weiterhin im Fehlerprotokoll aufgezeichnet, aber als &quot;verarbeitet&quot;markiert, um weitere Protokollierungsfunktionen zu ermöglichen. Außerdem [!DNL Amazon sales channel] entfernt nun automatisch überschüssige Daten, die für Bestellungen gesammelt wurden, die nicht in Commerce erstellt werden.

![Fehlerbehebung](../assets/fix.svg) Die Fehlerprotokollierung wurde aktualisiert, um mehr Informationen zu nicht abgefangenen Ausnahmefehlern und Fehlern bei der Aktualisierung von Erweiterungen zu sammeln.

![Fehlerbehebung](../assets/fix.svg) <!--ticket#-->Es wurde ein Problem behoben, das die anfängliche Synchronisierung der _niedrigster Preis_ Daten fehlschlagen, weil _price_ -Wert.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4410-->Korrektur von Problemen, die zu Filterfehlern in der _Amazon-Bestellungen_ anzeigen, wenn das Datumsbereichsfeld leer gelassen wird.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4439-->Es wurde ein Problem behoben, das zu quantitationsbezogenen Fehlern bei Bestell- und Fulfillment-Synchronisierungen führte. Die Erweiterung rundet nun die als Dezimalzahl eingegebenen Mengenwerte ab, bevor sie mit Amazon synchronisiert wird.<br/> Wenn beispielsweise ein Händler manuell eine Menge `2.5`, rundet die Erweiterung den Wert auf `2` und synchronisiert dann die aktualisierte Menge mit Amazon.

## v4.1.0

*7. Mai 2020*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Neu](../assets/new.svg) <!--4247, 4230-->Der Bestellimport-Prozess wurde an die Anforderungen für Commerce-Bestellungen angepasst. Durch diese Änderungen werden Probleme behoben, die dazu führten, dass Commerce die entsprechende Bestellung für eine importierte Bestellung nicht erstellen konnte. Siehe [Bestellungen verwalten](managing-orders.md) für Informationen zu Bestellblockern und Lösungen.

![Neu](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->Die _Letzte Bestellungen_ Abschnitt des Store-Dashboards hinzugefügt und ein neuer _Alle Bestellungen_ -Ansicht, die alle Ihre Amazon-Bestellungen anzeigt, einschließlich Filteroptionen und Paginierung für die Anzeige weiterer Bestellungen. Siehe [Amazon Store-Dashboard](amazon-store-dashboard.md) und [Anzeigen von Amazon-Bestellungen](amazon-orders-all.md).

![Neu](../assets/new.svg) Der _[!UICONTROL Order Notes]_Spalte der neu gestalteten_[!UICONTROL Amazon Orders]_ -Tabelle in beiden _[!UICONTROL Recent Orders]_und_[!UICONTROL All Orders]_ Ansichten. _[!UICONTROL Order Notes]_dem Händler mitteilen, dass ein Problem mit dem Import der Bestellung vorliegt. Siehe [Anzeigen von Amazon-Bestellungen](amazon-orders-all.md).

![Neu](../assets/new.svg) <!--CHAN-4013-->Die Parameter für die Produktbedingung wurden aktualisiert, um sie an die [Amazon erneuert](https://sell.amazon.com/programs/renewed) Programm. Siehe [Erneuerte Produkte](renewed-products.md).

![Neu](../assets/new.svg) <!--CHAN-3680-->Aktualisiert [Amazon-Bestelldetails](amazon-order-details.md) , um &quot;generische Daten&quot;für Bestellungen einzubeziehen, die von Amazon erfüllt werden. Siehe [Erfüllt von](fulfilled-by.md).

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4069-->Es wurde ein Problem behoben, das zu einer Verzerrung der Symbole auf der Store-Karte führte.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4165-->Korrektur eines Fehlers, der die _Anmelden_ angezeigt, nachdem die Sitzung beendet wurde.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4211-->Fehlerkorrektur - Der Amazon-Bestellsteuerbetrag kann jetzt in die neue Commerce-Bestellung importiert werden.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4234-->Korrektur eines Fehlers, der dazu führte, dass die im Store-Dashboard angezeigten Umsatzsummen Bestellungen in `Canceled` oder `Error` Status.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4326-->Korrektur eines Fehlers, der zu Fehlern beim Bestellimport führte, die mit Erweiterungen von Drittanbietern, die _Magento Shipping_ Methoden zum Erstellen von Bestellungen.

![Fehlerbehebung](../assets/fix.svg) <!--CHAN-4357-->Es wurde ein Problem behoben, das bei der Ausführung der Cron-Synchronisation Fehler verursachte. Dem CLI-Befehl wurde eine Sperre hinzugefügt, die verhindert, dass zwei Cron-Aufträge gleichzeitig synchronisiert werden.

![Fehlerbehebung](../assets/fix.svg) Aktualisierte Content Security-Richtlinie für Unterstützung mit Commerce-Version 2.3.5.

## v4.0.0

*25. März 2020*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0 wird für Adobe Commerce 2.3.5 nicht unterstützt. Für die Unterstützung mit Adobe Commerce 2.3.5 aktualisieren Sie auf Amazon Sales Channel 4.1.0.

![Neu](../assets/new.svg) Neu: [Amazon Sales Channel](amazon-sales-channel-home.md) Homepage mit verbesserter &quot;Kartenansicht&quot; für Ihre Store-Informationen.

![Neu](../assets/new.svg) Neu: [Store-Dashboard](amazon-store-dashboard.md) mit Listen, aktuellen Bestellungen und Store-Einstellungsinformationen.

![Neu](../assets/new.svg) Einführung einer einfacheren, optimierten [Onboarding-Prozess](amazon-onboarding-home.md) und [Standardspeichereinstellungen](default-store-settings.md) um Ihre Geschäfte schneller zu integrieren.

![Bekanntes Problem](../assets/bug.svg) <!--CHAN-4102--> Wann [Erstellen von Attributen](managing-attributes.md) zum Importieren von Bildern aus Listen und **Store-Ansichten** auf `All Store Views (Global)`, ist ein bekanntes Problem vorhanden, das den Import von Bildern in alle Store-Ansichten verhindert. Wenn Sie die Einstellung für **Ansichten speichern (zum Importieren von Werten in )** in einen bestimmten Speicher importieren die Bilder für diesen Store.

## v3.0.1

*11. November 2019*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Fehlerbehebung](../assets/fix.svg) **Numerische Feldeinstellungen**: <!--CHAN-3779-->Felder, für die ein numerischer Wert erforderlich ist, wurden aktualisiert, sodass nur numerische Zeichen zulässig sind. Beispiel: Preisregeleinstellungen > Feld &quot;Anpassungsbetrag&quot;

![Fehlerbehebung](../assets/fix.svg) **Benutzerhandbuch-Links**: <!--CHAN-3778-->Falsch _Benutzerhandbuch_ -Links korrigiert wurden.

![Fehlerbehebung](../assets/fix.svg) **Duplizieren von Amazon-Listen**: <!--CHAN-3593-->Ein zuvor gemeldetes Problem, das zu doppelten Amazon-Auflistungen führt, wurde jetzt behoben. Vor dieser Version hat die Erweiterung den Ländercode für die Amazon-Region zum SKU-Wert beim Import von Listen hinzugefügt. Die Liste stimmte mit dem Katalogelement überein, aber die Erweiterung erstellte eine neue, doppelte Liste mit der angehängten SKU. Mit dieser Version ändert die Erweiterung die SKU für importierte Listen nicht und an vorhandenen Listen werden keine Änderungen vorgenommen. Sie können die [!UICONTROL End Listing(s)] auf Amazon , um doppelte Listen zu entfernen.

## v3.0.0

*7. Oktober 2019*

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

![Neu](../assets/new.svg) **Amazon UK Marketplace jetzt verfügbar**: Benutzer können beim Erstellen und Integrieren eines Commerce-Stores den britischen Marketplace wählen. Dieses Upgrade für Großbritannien beinhaltet zusätzliche Unterstützung für:

- [Amazon - MwSt-Berechnungsservice](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [Produktsteuercode](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"} Informationen.

![Neu](../assets/new.svg) **Verbesserte Protokollierung**: <!--CHAN-3642, 3672-->Implementiert die **Aktivieren der Debug-Protokollierung** zur Erfassung zusätzlicher Synchronisierungsdaten bei der Fehlerbehebung. Siehe [Sales Channel-Einstellungen](https://docs.magento.com/user-guide/configuration/sales-channels/global-settings.html) Thema in der Konfigurationsreferenz.

![Fehlerbehebung](../assets/fix.svg) **Produktkatalog**: <!--CHAN-3687-->Fehlerkorrektur - Mit einer Amazon-Liste importierte Bilder können jetzt auf das entsprechende Commerce-Katalogprodukt angewendet werden.

![Fehlerbehebung](../assets/fix.svg) **Bestellerstellung**: <!--CHAN-3708-->Es wurde ein Fehler behoben, der dazu führte, dass Commerce keine Bestellungen für eine Amazon-Bestellung erstellte, die nicht mit einem Commerce-Katalogprodukt übereinstimmte.

![Bekanntes Problem](../assets/bug.svg) **Duplizieren von Amazon-Listen**: <!--CHAN-3593-->Dieses Problem führt dazu, dass der Katalog ein Element für eine importierte Liste erstellt, wobei dieselbe SKU verwendet wird, am Ende jedoch ein Regionscode hinzugefügt wird. Amazon verarbeitet dann die geänderte SKU als neues Element und erstellt eine Liste. Dieses Problem wird in einer zukünftigen Version behoben.

## v2.0.0

[!BADGE Kompatibilität]{type=Informative tooltip="Kompatibilität"}

>[!NOTE]
>
>Version 1.0.0 war nur in begrenzter Version verfügbar.

![Neu](../assets/new.svg)  **Vereinfachtes Onboarding und Warten**: Fügen Sie Ihr Amazon-Verkaufskonto hinzu und integrieren Sie es in einem Schritt-für-Schritt-Verfahren mit detaillierten Anweisungen, die über den Administrator verfügbar sind. Verwalten Sie Ihre Stores, Konten und aufgelisteten Produkte über ein Dashboard.

![Neu](../assets/new.svg)  **Unterstützung mehrerer Konten**: Verwalten und überwachen Sie mehrere Amazon-Marken und Marketplace-Regionen über den Administrator.

![Neu](../assets/new.svg)  **Intelligente Preise**: Legen Sie automatisierte Neupreisregeln fest, um Ihre Chancen für die begehrte Buy Box zu erhöhen. Stellen Sie die Preise so ein, dass sie sich dynamisch an den aktuellen Buy Box-Preis oder an die niedrigste Preisgestaltung des Konkurrenten anpassen. Legen Sie Beschränkungen für die Neuberechnung fest, um Ihre Marge zu schützen.

![Neu](../assets/new.svg)  **Listening-Verwaltung**: Automatisieren Sie Produktlisten und synchronisieren Sie Ihren Commerce-Katalog mithilfe von Listenregeln mit dem Amazon Marketplace. Fügen Sie spezifische Überschreibungen hinzu, um Ihre Angebote optimal zu steuern. Überwachen und verwalten Sie alle Ihre Einträge direkt über den Administrator.

![Neu](../assets/new.svg)  **Konsistente Inventory management**: Bewahren Sie Ihre Lagerbestandsmengen in Commerce und Amazon konstant auf.

![Neu](../assets/new.svg)  **Auftrags- und Ausführungsverwaltung**: Verfolgen Sie Amazon-Bestellungen über das Dashboard mit nahtlosen Kommunikations- und Bestandsaktualisierungen. Vervollständigen und verfolgen Sie die Auftragslieferungen, die von Amazon, dem Händler oder einer Kombination von Methoden erfüllt wurden.

![Bekanntes Problem](../assets/bug.svg)  Es kann vorkommen, dass Sie längere Wartezeiten haben, um die Produktmengen zu aktualisieren. Die Synchronisierung von Aktualisierungen für die Produktmenge kann etwa zwei Stunden dauern.

![Bekanntes Problem](../assets/bug.svg)  Die importierten Bestellungen können eine _Prime_ oder _Premium_ Bestellungen. Sie sollten diese Bestellungen in Ihrem Amazon-Verkaufskonto überprüfen.

![Bekanntes Problem](../assets/bug.svg)  Nicht infrage kommende gebündelte Produkte werden möglicherweise als für die Aufnahme in Amazon infrage kommend angezeigt. Eines der Produkte innerhalb des gebündelten Produkts ist möglicherweise nicht förderfähig. Wenn Probleme auftreten, überprüfen Sie den Berechtigungsstatus für gebündelte Produkte.

![Bekanntes Problem](../assets/bug.svg)  Bei Verwendung von Inventory management für Commerce 2.3.x wird bei der Erstellung einer Bestellung möglicherweise keine partielle Neuindizierung des Lagers Trigger. Die verkaufbare Menge berechnet stündlich neu, was während dieses Aktualisierungsintervalls zu einer Überschreibung führen kann.
