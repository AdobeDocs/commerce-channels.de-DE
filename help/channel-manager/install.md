---
title: 'install [!DNL Channel Manager]'
description: "Installieren Sie die Erweiterung[!DNL Channel Manager] ."
role: Admin, Developer
feature: Sales Channels, Install
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 1e74150e6ac88dbabb2e4bbb2fa2f243072eb03f
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---


# Installieren Sie [!DNL Channel Manager]

Überprüfen Sie die [Anforderungen](onboard.md#requirements) und sammeln Sie die erforderlichen Informationen, bevor Sie den Kanal-Manager installieren.

## Installieren der Erweiterung

Die Installationsanweisungen für den Kanalmanager hängen davon ab, ob Adobe Commerce oder Magento Open Source lokal oder in der Cloud-Infrastruktur bereitgestellt wird.

- Installieren Sie es auf einer [lokalen Instanz](#install-on-an-on-premises-instance).

- Installieren auf einer [[!DNL Adobe Commerce] Cloud-Infrastrukturinstanz](#install-adobe-commerce-on-cloud-infrastructure)

Bei beiden Methoden müssen Sie die Befehlszeilenschnittstelle (CLI) verwenden.

>[!NOTE]
>
>Hilfe zur Installation der [!DNL Commerce]-Software mithilfe der CLI finden Sie unter [Installieren einer Erweiterung](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

### Installation auf einer lokalen Instanz

Verwenden Sie diese Anweisungen, um [!DNL Channel Manager] in Adobe Commerce zu installieren und die Magento Open Source auf einer lokalen Instanz durchzuführen.

1. Melden Sie sich beim [!DNL Commerce] -Server als [Benutzer mit der Berechtigung](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/file-system/configure-permissions.html) an, in das [!DNL Commerce] -Dateisystem zu schreiben.

1. Setzen Sie Ihre Website in den [Wartungsmodus](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/maintenance-mode.html).

   ```bash
   $ bin/magento maintenance:enable
   ```

1. Fügen Sie im Stammverzeichnis des Projekts [!DNL Commerce] den Kanal-Manager zu `composer.json` hinzu.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. Geben Sie bei Aufforderung die Zugriffsschlüssel aus Ihrem [!DNL Commerce] -Konto ein.

   Ihr öffentlicher Schlüssel ist Ihr Benutzername, Ihr privater Schlüssel ist Ihr Passwort.

1. Aktualisieren Sie die Abhängigkeiten und installieren Sie die Erweiterung.

   ```bash
   composer update magento/channel-manager
   ```

   Der Befehl `composer update` aktualisiert nur die Abhängigkeiten, die für [!DNL Channel Manager] erforderlich sind. Um alle Abhängigkeiten zu aktualisieren, verwenden Sie stattdessen diesen Befehl: `composer update`.

1. Warten Sie, bis Composer die Aktualisierung der Projektabhängigkeiten abgeschlossen und etwaige Fehler behoben hat.

1. Überprüfen Sie die Modulinstallation:

   - Überprüfen Sie den Modulstatus.

     ```bash
     bin/magento module:status Magento_SalesChannels
     ```

     Beispielantwort:

     ```
     Module is enabled
     ```

   - Wenn das Modul nicht aktiviert ist, aktivieren Sie es.

   ```bash
   bin/magento module:enable Magento_SalesChannels
   ```

1. Registrieren Sie die Erweiterung.

   ```bash
   bin/magento setup:upgrade
   ```

1. Kompilieren Sie bei entsprechender Aufforderung Ihr [!DNL Commerce] -Projekt erneut.

   ```bash
   bin/magento setup:di:compile
   ```

1. Bereinigen Sie den Cache.

   ```bash
   bin/magento cache:clean
   ```

1. Wartungsmodus deaktivieren.

   ```bash
   bin/magento maintenance:disable
   ```

### Installieren auf einer Adobe Commerce on Cloud Infrastructure-Instanz

Arbeiten Sie in einer Entwicklungsverzweigung, wenn Sie Ihrer Cloud-Instanz eine Erweiterung hinzufügen.

Hilfe zur Verwendung von Verzweigungen finden Sie unter [Erste Schritte zum Erstellen von Verzweigungen](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html) im _Commerce on Cloud Infrastructure Guide_.

Während der Installation wird der Erweiterungsname (`magento\channel-manager`) automatisch in die Datei [app/etc/config.php](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/store-settings.html) eingefügt. Sie müssen die Datei nicht direkt bearbeiten.

1. Wechseln Sie auf Ihrer lokalen Workstation zum Stammordner des Cloud-Projekts.

1. Erstellen oder auschecken Sie einen Entwicklungs-[Zweig](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html).

1. Fügen Sie mithilfe des Composer-Namens die Erweiterung zum Abschnitt `require` der Datei `composer.json` hinzu.

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. Aktualisieren Sie die Abhängigkeiten und installieren Sie die Erweiterung.

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   Der Befehl `composer update` aktualisiert nur die Abhängigkeiten, die für [!DNL Channel Manager] erforderlich sind. Um alle Abhängigkeiten zu aktualisieren, verwenden Sie stattdessen diesen Befehl: `composer update`.

1. Fügen Sie Änderungen an Code-Änderungen hinzu, übertragen Sie sie und fügen Sie sie in die Datei `composer.lock` und in die Datei `composer.json` ein.

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m "Install channel manager extension" 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. Nachdem der Build- und Bereitstellungsprozess abgeschlossen ist, melden Sie sich mit SSH bei der Remote-Umgebung an und überprüfen Sie, ob die Erweiterung ordnungsgemäß installiert wurde.

```bash
   bin/magento module:status Magento_SalesChannels
```

Beispielantwort:

```
Module is enabled
```

Wenn das Modul deaktiviert ist, aktivieren Sie es in Ihrer lokalen Umgebung ](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/extensions.html) und stellen Sie Ihre Änderungen bereit.[


1. Nachdem Sie die Erweiterung erfolgreich installiert haben, melden Sie sich bei [!UICONTROL Admin] an, um [den Commerce Services Connector zu konfigurieren](connect.md).

   >[!NOTE]
   >
   >Anweisungen zum Aktualisieren des Kanal-Managers auf eine neue Version finden Sie unter [Module und Erweiterungen aktualisieren](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html).


## Fehlerbehebung

Verwenden Sie die folgenden Informationen, um Fehler zu beheben, die während des Installationsprozesses von Channel Manager auftreten.

### Falsche Composer-Schlüssel

Wenn die [Zugriffsschlüssel](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html), die für die Authentifizierung am Composer-Repository verwendet werden, ungültig sind oder nicht mit den [!DNL MAGE ID] verknüpft sind, die für die Anmeldung für den [!DNL Channel Manager]-Dienst verwendet werden, wird der folgende Fehler angezeigt.

```
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

Überprüfen Sie die Schlüsselkonfiguration:

1. Suchen Sie den Speicherort der Datei &quot;`auth.json`&quot;:

   ```bash
   $ composer config –global home
   ```

1. Anzeigen der Datei &quot;`auth.json`&quot;.

   ```bash
   $ cat /path/to/auth.json
   ```

1. Vergewissern Sie sich, dass die Anmeldeinformationen in der Datei &quot;auth.json&quot;mit [den Schlüsseln übereinstimmen, die mit der MAGE ID](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) verknüpft sind, die zur Registrierung für den Kanal-Manager-Dienst verwendet wurde.

### Unzureichender Speicher für PHP

Der folgende Fehler wird angezeigt, wenn dem System nicht genügend Speicher für PHP zugewiesen ist.

```
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

Verwenden Sie eine der folgenden Methoden, um das Speicherproblem zu beheben:

- [Erhöhen Sie die Speicherbegrenzung für PHP](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/php-settings.html) in der Umgebungsdatei `php.ini`. Überprüfen Sie außerdem, ob die Commerce-Instanz über die [empfohlenen Werte](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html) für andere PHP-Einstellungen verfügt.

- Geben Sie die Speicherbegrenzung über die Befehlszeile an.

  ```bash
  $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
  ```

  Beispiel:

  ```bash
  $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
  ```

### Fehlende Ansicht

Wenn Sie während der Installation des Kanalmanagers einen Fehler wegen des Fehlens von `process_catalog_exporter_view` erhalten, versuchen Sie, die Indexer zu aktualisieren [2}.](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/manage-indexers.html)

```bash
php bin/magento indexer:refresh
```

### Cloud-Bereitstellungsfehler

Probleme bei der Bereitstellung der Erweiterung in der Cloud finden Sie unter [Fehler bei der Bereitstellung der Erweiterung](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/deploy/recover-failed-deployment.html).
