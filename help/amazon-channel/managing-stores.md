---
title: Amazon Stores-Ansicht
description: Navigieren Sie zur Ansicht "Amazon Stores", um die grundlegenden Statistiken für jeden Ihrer Amazon Stores zu überprüfen und auf die Verwaltungsoptionen zuzugreifen.
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Ansicht &quot;Amazon Stores&quot;

Bei Ansicht der Homepage des Amazon-Vertriebskanals wird standardmäßig die Ansicht _Amazon Stores_ geöffnet.

![Ansicht &quot;Amazon Stores&quot;](assets/amazon-sales-channel-home-tabs.png)

Die _[!UICONTROL Amazon Stores]_-Ansicht zeigt eine &quot;Store-Karte&quot;für jeden Ihrer Amazon Stores zusammen mit einigen grundlegenden Statistiken und Verwaltungsoptionen. Die auf jeder Karte angezeigten Zusammenfassungsinformationen enthalten jeden Store-Status, das erstellte Datum, das Datum der letzten Aktualisierung und Auflistungen, die beachtet werden müssen (Beispiel: Unvollständige Listen) und der zugewiesenen [!DNL Commerce]-Website.

Bei der Anzeige der Ansicht _[!UICONTROL Amazon Store]_ermöglicht jede Store-Karte Folgendes:

- Um einen Store [dashboard](./amazon-store-dashboard.md) zu öffnen, klicken Sie auf **[!UICONTROL View Store]**.

- Um einen Store-Status zu ändern oder einen Store zu löschen, klicken Sie auf **[!UICONTROL Action]** und wählen Sie:

   - **[!UICONTROL Activate]** /  **[!UICONTROL Deactivate]**  - Wählen Sie aus, den Status des Stores in  `Active` bzw.  `Inactive`zu ändern.

      Wenn Sie einen `Inactive`-Store in den Status `Active` ändern, werden Auflistungen und die Bestellaktivität für den Store aktiviert. Dabei werden die aktuellen Store-Einstellungen verwendet (z. B. Listeneinstellungen, Preisregeln und Überschreibungen).

      Wenn Sie einen Store-Status von `Active` in `Inactive` ändern, werden Listen und die Bestellaktivität für den Store ausgesetzt. Ein inaktiver Store behält alle Store-Einstellungen und -Auflistungen bei, stoppt jedoch vorübergehend die Synchronisation von Preis, Menge und Auftragsverwaltung, bis der Store wieder den Status `Active` erhält. Mit dieser Funktion können Sie Ihre Store-Aktivität auf regionaler Ebene steuern, ohne dass Sie Ihren Amazon-Store neu integrieren oder neu integrieren müssen oder historische Bestellungen- und Verkaufsdaten verloren gehen.

   - **[!UICONTROL Delete]** - Wählen Sie aus, einen nicht mehr benötigten Store zu löschen.

      Wählen Sie aus, wann Sie einen vorhandenen Amazon-Store und dessen Integrationseinstellungen mit Ihrem [!DNL Amazon Seller Central]-Konto löschen möchten. Durch das Löschen des Kontos wird der Store aus dem Amazon-Vertriebskanal entfernt, einschließlich aller Kontoeinstellungen, Auflistungen, Protokolle und anderer Informationen zu diesem Store. Der Store kann nach dem Löschen nicht abgerufen werden. Es muss ein neuer Store erstellt werden.

>[!NOTE]
>Um die während der Integration dem Store zugewiesene Website zu ändern, müssen Sie den Store löschen und den Store erneut mit der anderen Website hinzufügen, die während der Store-Integration definiert wurde.

| Store Card | Beschreibung |
|--- |--- |
| Top-Bereich | Umfasst: <br>Das Regionssymbol für den Store, definiert während [Store-Integration](./store-integration.md).<br> Die zugewiesene  _[!UICONTROL Magento Website]_, während der Store-Integration definiert.<br>Die_[!UICONTROL Status]_ Ihres Ladens. Optionen: **[!UICONTROL Active]** - Die Speicherintegration ist mit Amazon abgeschlossen und überprüft und steht für die Verkaufsaktivität zur Verfügung. **[!UICONTROL Inactive]** - Die Speicherintegration ist abgeschlossen, wird jedoch nicht verwendet oder steht nicht für Verkaufsaktivitäten zur Verfügung. Wenn `Inactive` Ihre Amazon-Verkäufe angehalten werden. Wenn `Active`, werden der Umsatz und zusätzliche Einstellungen vor der Aktivierung aktualisiert.<br>Das  *[!UICONTROL Last Updated]* Datum der letzten Änderung am Amazon Store-Setup.<br>Das  *[!UICONTROL Created]* Datum, an dem der Amazon Store im Amazon-Vertriebskanal erstellt wurde. |
| Zweiter Abschnitt | Enthält ein Zusammenfassungsdiagramm zu Store-Aktivitäten für die letzten 30 Tage sowie Hinweise und Warnhinweise für alle Einträge, die beachtet werden müssen. |
| Unterer Bereich | Umfasst die Optionen &quot;Store anzeigen&quot;und &quot;Aktion&quot;.<br>Um das Store- [Dashboard](./amazon-store-dashboard.md) zu öffnen, klicken Sie auf  **[!UICONTROL View Store]**.<br>Um einen Store zu aktivieren, zu deaktivieren oder zu löschen, klicken Sie auf  **[!UICONTROL Actions]**. |
