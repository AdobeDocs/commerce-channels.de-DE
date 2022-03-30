---
title: Installieren [!DNL Channel Manager]
description: Installieren Sie die Channel Manager-Erweiterung.
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 8f07b215c20cc28aa9a6862bcb2b00da30a1ed84
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Installieren des Kanal-Managers

Überprüfen Sie die [Voraussetzungen](onboard.md#prerequisites) und sammeln Sie die erforderlichen Informationen, bevor Sie den Kanal-Manager installieren.

## Mindeststabilitätseinstellung aktualisieren

Aktualisieren Sie vor der Installation der Erweiterung die `minimum-stability` Anforderungen in `composer.json` -Datei, damit Sie frühe Versionen von Channel Manager mithilfe von Composer installieren können.

Um die Konfiguration zu aktualisieren, fügen Sie die folgenden Zeilen zum `composer.json` -Datei.

```json
{
   "minimum-stability": "alpha",
   "prefer-stable": true
}
```

## Installieren der Erweiterung

Die Installationsanweisungen für den Kanalmanager hängen davon ab, ob Adobe Commerce oder Magento Open Source lokal oder in der Cloud-Infrastruktur bereitgestellt wird.

- Installieren auf einem [Vor-Ort-Instanz](#install-on-an-on-premises-instance).

- Installieren auf einem [[!DNL Adobe Commerce] auf der Cloud-Infrastrukturinstanz](#install-adobe-commerce-on-cloud-infrastructure)

Bei beiden Methoden müssen Sie die Befehlszeilenschnittstelle (CLI) verwenden.

>[!NOTE]
>
>Hilfe bei der Installation [!DNL Commerce] -Software, die die CLI verwendet, siehe [Allgemeine CLI-Installation](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;}.

### Installation auf einer lokalen Instanz

Verwenden Sie diese Anweisungen zur Installation auf Adobe Commerce- und Magento Open Source-Plattformen.

1. Melden Sie sich bei der [!DNL Commerce] Server als [Benutzer mit Berechtigungen](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/file-system-perms.html){target=&quot;_blank&quot;} zum Schreiben in die [!DNL Commerce] Dateisystem.

1. Website in [Wartungsmodus](https://devdocs.magento.com/guides/v2.4/install-gde/install/cli/install-cli-subcommands-maint.html){target=&quot;_blank&quot;}.

   ```bash
   $ bin/magento maintenance:enable
   ```

1. Aus dem [!DNL Commerce] Projektstammordner, Hinzufügen von Kanal-Manager zu `composer.json`.

   ```bash
    $ composer require magento/channel-manager --no-update
   ```

1. Geben Sie bei entsprechender Aufforderung die Zugriffsschlüssel aus Ihrem [!DNL Commerce] -Konto.

   Ihr öffentlicher Schlüssel ist Ihr Benutzername. Ihr privater Schlüssel ist Ihr Passwort.

1. Aktualisieren Sie die Abhängigkeiten und installieren Sie die Erweiterung.

   ```bash
   $ composer update
   ```

   Die `composer update` -Befehl aktualisiert alle Abhängigkeiten. Verwenden Sie stattdessen diesen Befehl, um nur Abhängigkeiten im Zusammenhang mit dem Kanal-Manager zu aktualisieren: `composer update magento/channel-manager`.

1. Warten Sie, bis Composer die Aktualisierung der Projektabhängigkeiten abgeschlossen und etwaige Fehler behoben hat.

1. Installation überprüfen

   ```bash
   $ bin/magento module:status channel-manager
   ```

   Beispielantwort:

   ```terminal
   Module is disabled
   ```

1. Registrieren Sie die Erweiterung.

   ```bash
   $ bin/magento setup:upgrade
   ```

1. Kompilieren Sie bei entsprechender Aufforderung Ihre [!DNL Commerce] Projekt.

   ```bash
   $ bin/magento setup:di:compile
   ```

1. Stellen Sie sicher, dass die Erweiterung aktiviert ist:

   ```bash
   $ bin/magento module:status channel-manager
   ```

   Beispielantwort:

   ```bash
   Module is enabled
   ```

1. Bereinigen Sie den Cache.

   ```bash
   $ bin/magento cache:clean
   ```

1. Wartungsmodus deaktivieren.

   ```bash
    $ bin/magento maintenance:disable
   ```

### Installieren auf einer Adobe Commerce on Cloud Infrastructure-Instanz

Arbeiten Sie in einer Entwicklungsverzweigung, wenn Sie Ihrer Cloud-Instanz eine Erweiterung hinzufügen.

Hilfe zur Verwendung von Verzweigungen finden Sie unter [Erste Schritte mit der Erstellung von Zweigen](https://devdocs.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;} in der Adobe Commerce-Entwicklerdokumentation.

Während der Installation wird der Erweiterungsname (`&lt;VendorName>\_&lt;ComponentName>`) wird automatisch in die [app/etc/config.php](https://devdocs-beta.magento.com/guides/v2.3/config-guide/config/config-php.html)Datei {target=&quot;_blank&quot;}. Sie müssen die Datei nicht direkt bearbeiten.

1. Wechseln Sie auf Ihrer lokalen Workstation zum Stammordner des Cloud-Projekts.

1. Erstellen oder Auschecken einer Entwicklung [Verzweigung](https://devdocs-beta.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;}.

1. Fügen Sie mithilfe des Composer-Namens die Erweiterung zum `require` Abschnitt `composer.json` -Datei.

   ```bash
   $ composer require magento/channel-manager --no-update
   ```

1. Hinzufügen, Übertragen und Push-Code-Änderungen, die Änderungen an beiden `composer.lock` und `composer.json` -Datei.

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m “Install channel manager extension” 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. Nachdem der Build und die Bereitstellung abgeschlossen sind, melden Sie sich mit SSH bei der Remote-Umgebung an und überprüfen Sie, ob die Erweiterung ordnungsgemäß installiert wurde.

   ```bash
   $ bin/magento module:status channel-manager
   ```

   Beispielantwort:

   ```terminal
   Module is enabled
   ```

1. Nachdem die Installation erfolgreich abgeschlossen wurde, melden Sie sich bei der [!UICONTROL Admin] nach [Konfigurieren von Commerce Services Connector](connect.md).

   >[!NOTE]
   >
   >Anweisungen zum Aktualisieren des Kanal-Managers auf eine neue Version finden Sie unter [Upgrade-Module und -Erweiterungen](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html){target=&quot;_blank&quot;}.


## Fehlerbehebung

Verwenden Sie die folgenden Informationen, um Fehler zu beheben, die während des Installationsprozesses von Channel Manager auftreten.

### Falsche Composer-Schlüssel

Wenn die Variable [Zugriffsschlüssel](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}, das zur Authentifizierung beim Composer-Repository verwendet wird, ungültig oder nicht mit dem [!DNL MAGE ID] verwendet, um sich für die [!DNL Channel Manager] -Dienst, wird der folgende Fehler angezeigt.


```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

Überprüfen Sie die Schlüsselkonfiguration:

1. Suchen Sie den Speicherort der `auth.json` Datei:

   ```bash
   $ composer config –global home
   ```

1. Anzeigen der `auth.json` -Datei.

   ```bash
   $ cat /path/to/auth.json
   ```

1. Überprüfen Sie, ob die Anmeldedaten in auth.json übereinstimmen. [die Schlüssel, die mit der MAGE ID verknüpft sind](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}, das zur Registrierung für den Kanal-Manager-Dienst verwendet wird.

### Unzureichender Speicher für PHP

Der folgende Fehler wird angezeigt, wenn dem System nicht genügend Speicher für PHP zugewiesen ist.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

Verwenden Sie eine der folgenden Methoden, um das Speicherproblem zu beheben:

- [Erhöhen Sie die Speicherbegrenzung für PHP.](https://devdocs.magento.com/cloud/project/magento-app-php-ini.html#increase-php-memory-limit){target=&quot;_blank&quot;} in der Umgebung `php.ini` -Datei. Überprüfen Sie außerdem, ob die Commerce-Instanz über die [empfohlene Werte](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html){target=&quot;_blank&quot;} für andere PHP-Einstellungen.

- Geben Sie die Speicherbegrenzung über die Befehlszeile an.

   ```bash
   $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
   ```

   Beispiel:

   ```bash
   $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
   ```

### Fehlende Ansicht

Wenn Sie eine Fehlermeldung über eine fehlende `process_catalog_exporter_view` während der Installation des Kanal-Managers versuchen Sie es [Indexer aktualisieren](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-index.html#config-cli-subcommands-index-reindex){target=&quot;_blank&quot;}.

```bash
php bin/magento indexer:refresh
```

### Cloud-Bereitstellungsfehler

Probleme bei der Bereitstellung der Erweiterung in der Cloud finden Sie unter [Fehler bei der Erweiterungsbereitstellung](https://devdocs.magento.com/cloud/trouble/trouble_comp-deploy-fail.html){target=&quot;_blank&quot;}.