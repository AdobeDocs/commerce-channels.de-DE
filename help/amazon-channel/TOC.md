---
user-guide-title: Benutzerhandbuch für Amazon Sales Channel
user-guide-description: Generieren von Verkäufen über Amazon durch Integration von Adobe Commerce oder Magento Open Source in Ihre [!DNL Amazon Seller Central] -Konto.
breadcrumb-title: Amazon-Vertriebskanal
role: Admin, User
feature: Sales Channels
recommendations: noDisplay
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# Amazon-Vertriebskanal - [!DNL channel manager] für Adobe Commerce {#amazon}

- [Benutzerhandbuch für Amazon Sales Channel](guide-overview.md)
- [Einführung in den Amazon-Vertriebskanal](overview.md)
- Erste Schritte {#getting-started}
   - [Über Amazon Marketplace](about-amazon-marketplace.md)
   - [Amazon und der Commerce-Katalog](about-listings-and-catalog.md)
   - [Best Practices und Einschränkungen](amazon-best-practices.md)
   - [Installieren der Erweiterung](install.md)
- Onboarding {#onboarding}
   - [Onboard Amazon Sales Channel](amazon-onboarding-home.md)
   - [Aufgaben vor der Einrichtung](amazon-pre-setup-tasks.md)
   - [Erstellen [!DNL Commerce] -Attribute für Amazon](ob-creating-magento-attributes.md)
   - [Überprüfen des Amazon-API-Schlüssels](amazon-verify-api-key.md)
   - [Speicherintegration](store-integration.md)
   - [Erstellen einer Listungsregel](ob-create-listing-rule.md)
   - [Standardmäßige Store-Einstellungen](default-store-settings.md)
- Verwalten des Vertriebskanals {#manage}
   - [Startseite](amazon-sales-channel-home.md)
   - [Amazon Stores](managing-stores.md)
   - [Workspace-Steuerelemente](workspace-controls.md)
   - [Lernen und Vorbereitung](learning-preparation.md)
   - Attribute {#attributes}
      - [Anzeigen von Attributen](attributes-view.md)
      - [Attribute verwalten](managing-attributes.md)
      - [Erstellen und Bearbeiten von Attributen](creating-attributes.md)
      - [Anzeigen der Attributzuordnung](amazon-matching-attributes-values.md)
   - [Admin-Einstellungen für Vertriebskanäle](sales-channel-settings.md)
   - [Amazon Store-Dashboard](amazon-store-dashboard.md)
   - [Speichereinstellungen](ob-store-review.md)
- Listening-Einstellungen {#listing-settings}
   - [Listeneinstellungen anzeigen](listing-settings.md)
   - [Aktionen auf der Produktliste](product-listing-actions.md)
   - [Drittanbieterlisten](third-party-listing-settings.md)
   - [Börsenkurs](listing-price.md)
   - [(B2B) Geschäftspreise](business-pricing.md)
   - [Lager/Menge](stock-quantity.md)
   - [Erfüllt von](fulfilled-by.md)
   - [Katalogsuche](catalog-search.md)
   - [Bedingung für die Produktliste](product-listing-condition.md)
   - [Erneuerte Produkte](renewed-products.md)
- [Bestelleinstellungen](order-settings.md)
- [Einstellungen zur Store-Integration](store-integration-settings.md)
- Listen- und Preisregeln {#rules}
   - [Listening-Regeln](listing-rules.md)
   - Preisregeln {#pricing-rules}
      - [Preise verwalten](pricing-products.md)
      - [Neue Preisregel hinzufügen](add-pricing-rule.md)
      - [Allgemeine Einstellungen für Preisregeln](pricing-rule-general-settings.md)
      - [Bedingungen für Preisregeln](pricing-rule-conditions.md)
      - [Aktionen für Preisregeln](pricing-rule-actions.md)
      - [Standardpreisregel](standard-price-rules.md)
      - [Intelligente Neupreisregel](intelligent-repricing-rules.md)
      - [Bedingte Unterschiede zwischen Wettbewerbern](competitor-conditional-variances.md)
      - [Preisanpassung](price-adjustment.md)
      - [Floor-Preis](floor-price.md)
      - [Optionaler Höchstpreis](optional-ceiling-price.md)
      - [Preissegment](price-scope.md)
      - [Preisprioritätslogik](price-priority-logic.md)
      - [Buy Box-Mitbewerber-Preise](buy-box-competitor-pricing.md)
      - [Niedrigste Preise für Wettbewerber](lowest-competitor-pricing.md)
   - Beispiele {#rules-examples}
      - [Bedingung definieren](ob-define-condition-example.md)
      - [Beispiele für Preisregeln](price-rule-examples.md)
- Berichte und Protokolle {#reports-logs}
   - [Protokolle und Berichte speichern](amazon-logs-reports.md)
   - Store-Berichte {#store-reports}
      - [Preisanalyse](competitive-price-analysis.md)
      - [Verbesserungen bei Listen](listing-improvements.md)
   - Protokolle {#logs}
      - [Protokoll zu Änderungen auflisten](listing-changes-log.md)
      - [Kommunikationsfehlerprotokoll](communication-errors-log.md)
- Listen verwalten {#admin-listings}
   - [Verwalten von Amazon-Listen](managing-product-listings.md)
   - Nach Status/Tab {#status-tab}
      - [Nach Status/Tab verwalten](managing-listings-by-tab.md)
      - [Unvollständige Listen](incomplete-listings.md)
      - [Neue Drittanbieterlisten](new-third-party-listings.md)
      - [Listenbereit](ready-to-list.md)
      - [Inaktive Listen](inactive-listings.md)
      - [Aktive Listen](active-listings.md)
      - [Überschreibungen](overrides.md)
      - [Nicht infrage kommende Listen](ineligible-listings.md)
      - [Eingestellte Listen](ended-listings.md)
   - Nach Aktionen {#actions}
      - [Verwalten nach Aktionen](managing-listings-by-action.md)
      - [Erstellen und Zuweisen von Katalogprodukten](creating-assigning-catalog-products.md)
      - [Erstellen und Bearbeiten von Überschreibungen](creating-editing-overrides.md)
      - [Alias-Verkäufer-SKU erstellen](create-alias-seller-sku.md)
      - [Zugewiesene ASIN bearbeiten](edit-assigned-asin.md)
      - [Beenden einer Amazon-Auflistung](end-listings-manually.md)
      - [Amazon-Liste veröffentlichen](publish-listings-manually.md)
      - [Erforderliche Informationen aktualisieren](amazon-manually-update-incomplete-listing.md)
      - [Details anzeigen](product-listing-details.md)
- Bestellungen verwalten {#admin-orders}
   - [Bestellungen verwalten](managing-orders.md)
   - [Anzeigen von Amazon-Bestellungen](amazon-orders-all.md)
   - [Amazon-Bestelldetails anzeigen](amazon-order-details.md)
   - [Allgemeine Aufgaben zur Bestellverarbeitung](common-order-processing.md)
   - [Erfüllungs-Workflows](fulfillment-workflows.md)
   - [Abbrechen nicht versandter Bestellungen](cancel-unshipped-order.md)
- [Versionshinweise](release-notes.md)
