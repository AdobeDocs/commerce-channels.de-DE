---
title: "[!UICONTROL Amazon Stores] view"
description: Navigieren Sie zur Ansicht "Amazon Stores", um die grundlegenden Statistiken für jeden Ihrer Amazon Stores schnell zu überprüfen und auf die Verwaltungsoptionen zuzugreifen.
feature: Sales Channels, Storefront
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# [!UICONTROL Amazon Stores] Ansicht

Bei Ansicht der Homepage des Amazon-Verkaufskanals wird standardmäßig die Ansicht _Amazon Stores_ geöffnet.

![Ansicht &quot;Amazon Stores&quot;](assets/amazon-sales-channel-home-tabs.png){width="600" zoomable="yes"}

Die Ansicht &quot;_[!UICONTROL Amazon Stores]_&quot;zeigt eine &quot;Store-Karte&quot;für jeden Ihrer Amazon-Stores zusammen mit einigen grundlegenden Statistiken und Verwaltungsoptionen an. Die auf jeder Karte angezeigten Zusammenfassungsinformationen enthalten jeden Store-Status, das erstellte Datum, das Datum der letzten Aktualisierung, Auflistungen, die Aufmerksamkeit erfordern (Beispiel: Unvollständige Auflistungen) und die zugewiesene [!DNL Commerce] Website.

Bei Ansicht der Ansicht &quot;_[!UICONTROL Amazon Store]_&quot; ermöglicht jede Store-Karte Folgendes:

- Um einen Store [Dashboard](./amazon-store-dashboard.md) zu öffnen, klicken Sie auf **[!UICONTROL View Store]**.

- Um einen Store-Status zu ändern oder einen Store zu löschen, klicken Sie auf **[!UICONTROL Action]** und wählen Sie:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Entscheiden Sie, den Status des Stores auf `Active` bzw. `Inactive` zu ändern.

     Wenn Sie einen `Inactive` -Store in den Status `Active` ändern, werden Auflistungen und die Bestellaktivität für den Store aktiviert. Dabei werden die aktuellen Store-Einstellungen verwendet (z. B. Listeneinstellungen, Preisregeln und Überschreibungen).

     Wenn Sie einen Store-Status von `Active` in den Status `Inactive` ändern, werden Listen und die Bestellaktivität für den Store ausgesetzt. Ein inaktiver Store behält alle Store-Einstellungen und -Auflistungen bei, stoppt jedoch vorübergehend die Synchronisation von Preis, Menge und Auftragsverwaltung, bis der Store wieder den Status &quot;`Active`&quot;erhält. Mit dieser Funktion können Sie Ihre Store-Aktivität auf regionaler Ebene steuern, ohne dass Sie Ihren Amazon-Store neu integrieren oder neu integrieren müssen oder historische Bestellungen- und Verkaufsdaten verloren gehen.

   - **[!UICONTROL Delete]** - Wählen Sie aus, einen nicht mehr benötigten Store zu löschen.

     Wählen Sie aus, wann Sie einen vorhandenen Amazon-Store und dessen Integrationseinstellungen mit Ihrem [!DNL Amazon Seller Central] -Konto löschen möchten. Durch das Löschen des Kontos wird der Store aus dem Amazon-Vertriebskanal entfernt, einschließlich aller Kontoeinstellungen, Auflistungen, Protokolle und anderer Informationen zu diesem Store. Der Store kann nach dem Löschen nicht abgerufen werden. Es muss ein neuer Store erstellt werden.

>[!NOTE]
>Um die während der Integration dem Store zugewiesene Website zu ändern, müssen Sie den Store löschen und den Store erneut mit der anderen Website hinzufügen, die während der Store-Integration definiert wurde.

| Store Card | Beschreibung |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Top-Bereich | Umfasst: <br>Das Regionssymbol für den Store, das während der [Speicherintegration](./store-integration.md) definiert wurde.<br> Die zugewiesene _[!UICONTROL Magento Website]_, die während der Speicherintegration definiert wurde.<br>Die_[!UICONTROL Status]_ Ihres Stores. Optionen: **[!UICONTROL Active]** - Die Speicherintegration ist mit Amazon abgeschlossen und überprüft und steht für die Verkaufsaktivität zur Verfügung. **[!UICONTROL Inactive]** - Die Speicherintegration ist abgeschlossen, wird jedoch nicht verwendet oder steht nicht für Verkaufsaktivitäten zur Verfügung. Wenn `Inactive`, werden Ihre Amazon-Verkäufe angehalten. Wenn `Active`, werden Verkaufsumsätze und zusätzliche Einstellungen vor der Aktivierung gespeichert und aktualisiert.<br>Das *[!UICONTROL Last Updated]* Datum der letzten Änderung am Amazon Store-Setup.<br>Das *[!UICONTROL Created]* Datum, an dem der Amazon-Store im Amazon-Verkaufskanal erstellt wurde. |
| Zweiter Abschnitt | Enthält ein Zusammenfassungsdiagramm zu Store-Aktivitäten für die letzten 30 Tage sowie Hinweise und Warnhinweise für alle Auflistungen, die beachtet werden müssen. |
| Unterer Bereich | Umfasst die Optionen &quot;Store anzeigen&quot;und &quot;Aktion&quot;.<br>Klicken Sie auf **[!UICONTROL View Store]**, um den Store [Dashboard](./amazon-store-dashboard.md) zu öffnen.<br>Klicken Sie auf **[!UICONTROL Actions]**, um einen Store zu aktivieren, zu deaktivieren oder zu löschen. |
