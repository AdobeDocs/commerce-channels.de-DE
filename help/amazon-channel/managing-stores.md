---
title: Amazon Stores Ansicht
description: Rufen Sie die Amazon Stores-Ansicht auf, um schnell die grundlegenden Statistiken für jeden Ihrer Amazon-Stores und die Zugriffssteuerungsoptionen zu überprüfen.
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Amazon Stores Ansicht

Bei Ansicht der Amazon Sales Kanal Startseite _Amazon Stores_ Ansicht wird standardmäßig geöffnet.

![Amazon Stores Ansicht](assets/amazon-sales-channel-home-tabs.png)

Die _[!UICONTROL Amazon Stores]_Ansicht zeigt eine &quot;Store Card&quot; für jeden Ihrer Amazon Stores sowie einige grundlegende Statistiken und Verwaltungsoptionen an. Die auf jeder Karte angezeigten Zusammenfassungen enthalten den jeweiligen Speicherstatus, das erstellte Datum, das letzte aktualisierte Datum und Listen, die beachtet werden müssen (Beispiel: Unvollständige Auflistungen) und zugewiesene [!DNL Commerce] Website.

Bei Ansicht des _[!UICONTROL Amazon Store]_Ansicht, jede Ladenkarte ermöglicht Ihnen:

- So öffnen Sie einen Laden [Dashboard](./amazon-store-dashboard.md), klicken **[!UICONTROL View Store]**.

- Klicken Sie zum Ändern des Speicherstatus oder Löschen eines Speichers auf **[!UICONTROL Action]** und wählen Sie:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Wählen Sie, um den Status des Store zu ändern in `Active` oder `Inactive`, bzw.

      Ändern eines `Inactive` speichern in `Active` -Status aktiviert Auflistungen und die Aktivität der Bestellungen für den Store und verwendet dabei die aktuellen Store-Einstellungen (wie z. B. Listeneinstellungen, Preisregeln und Überschreibungen).

      Ändern des Speicherstatus von `Active` nach `Inactive` -Status setzt die Aktivität der Einträge und der Bestellung für den Store aus. Ein inaktiver Store behält alle Speichereinstellungen und -auflistungen bei, stoppt jedoch vorübergehend die Synchronisierung von Preis, Menge und Auftragsverwaltung, bis der Store wieder zu `Active` Status. Mit dieser Funktion können Sie Ihre Store-Aktivität auf regionaler Ebene kontrollieren, ohne dass Sie Ihren Amazon Store neu integrieren oder neu integrieren müssen oder die historischen Auftragsdaten und Verkaufsdaten verloren gehen.

   - **[!UICONTROL Delete]** - Wählen Sie , um einen Store zu löschen, der nicht mehr benötigt wird.

      Wählen Sie aus, wann Sie einen vorhandenen Amazon Store und dessen Integrationseinstellungen mit Ihrem [!DNL Amazon Seller Central] Konto. Durch Löschen des Kontos wird der Store aus dem Amazon Sales Kanal entfernt, sowie alle Kontoeinstellungen, Einträge, Protokolle und andere Informationen zu diesem Store. Der Speicher kann nach dem Löschen nicht abgerufen werden. Es muss ein neuer Store erstellt werden.

>[!NOTE]
>Um die dem Store während der Integration zugewiesene Website zu ändern, müssen Sie den Store löschen und den Store erneut mit der während der Speicherintegration definierten Website hinzufügen.

| Karte speichern | Beschreibung |
|--- |--- |
| Oberer Abschnitt | Enthält: <br>Das Regionssymbol für den Store, definiert während [Speicherintegration](./store-integration.md).<br> Zugewiesene _[!UICONTROL Magento Website]_, definiert während der Speicher-Integration.<br>Die_[!UICONTROL Status]_ in Ihrem Geschäft. Optionen: **[!UICONTROL Active]** - Die Filialintegration ist vollständig und mit Amazon verifiziert und steht für die Aktivität von Verkäufen zur Verfügung. **[!UICONTROL Inactive]** - Die Store-Integration ist vollständig, wird jedoch nicht verwendet und ist nicht für die Aktivität von Verkäufen verfügbar. Wann `Inactive`Ihre Amazon-Verkäufe werden angehalten. Wann `Active`, Umsatzerlöse und zusätzliche Einstellungen werden vor der Aktivierung zur Aktualisierung gespeichert.<br>Die *[!UICONTROL Last Updated]* Datum der letzten Änderung der Amazon Store-Einrichtung.<br>Die *[!UICONTROL Created]* Datum, an dem der Amazon Store im Amazon Sales Kanal erstellt wurde. |
| Mittlerer Abschnitt | Enthält ein Zusammenfassungs-Diagramm der Store-Aktivität der letzten 30 Tage sowie Hinweise und Warnhinweise für alle Auflistungen, die beachtet werden müssen. |
| Unterer Abschnitt | Enthält die Optionen &quot;Ansicht speichern&quot;und &quot;Aktion&quot;.<br>So öffnen Sie den Laden [Dashboard](./amazon-store-dashboard.md), klicken **[!UICONTROL View Store]**.<br>Klicken Sie zum Aktivieren, Deaktivieren oder Löschen eines Speichers auf **[!UICONTROL Actions]**. |
