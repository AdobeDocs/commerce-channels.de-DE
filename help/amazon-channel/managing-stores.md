---
title: Amazon Stores-Ansicht
description: Navigieren Sie zur Ansicht "Amazon Stores", um die grundlegenden Statistiken für jeden Ihrer Amazon Stores zu überprüfen und auf die Verwaltungsoptionen zuzugreifen.
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Amazon Stores-Ansicht

Wenn Sie sich die Startseite des Amazon-Vertriebskanals ansehen, wird die _Amazon Stores_ -Ansicht wird standardmäßig geöffnet.

![Ansicht &quot;Amazon Stores&quot;](assets/amazon-sales-channel-home-tabs.png)

Die _[!UICONTROL Amazon Stores]_-Ansicht zeigt für jeden Ihrer Amazon-Stores eine &quot;Store-Karte&quot;mit einigen grundlegenden Statistiken und Verwaltungsoptionen an. Die auf jeder Karte angezeigten Zusammenfassungsinformationen enthalten jeden Store-Status, das erstellte Datum, das Datum der letzten Aktualisierung und Auflistungen, die beachtet werden müssen (Beispiel: Unvollständige Listen) und die zugewiesenen [!DNL Commerce] Website.

Beim Anzeigen der _[!UICONTROL Amazon Store]_anzeigen, können Sie mit jeder Speicherkarte:

- So öffnen Sie einen Store [Dashboard](./amazon-store-dashboard.md)klicken **[!UICONTROL View Store]**.

- Um einen Store-Status zu ändern oder einen Store zu löschen, klicken Sie auf **[!UICONTROL Action]** und wählen Sie:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Ändern Sie den Status des Stores in `Active` oder `Inactive`zurück.

      Ändern von `Inactive` speichern in `Active` Status aktiviert Auflistungen und die Bestellaktivität für den Store unter Verwendung der aktuellen Store-Einstellungen (z. B. Listeneinstellungen, Preisregeln und Überschreibungen).

      Ändern des Speicherstatus von `Active` nach `Inactive` status setzt Auflistungen und die Bestellaktivität für den Store aus. Ein inaktiver Store behält alle Store-Einstellungen und -Auflistungen bei, stoppt jedoch vorübergehend die Synchronisierung von Preis, Menge und Auftragsverwaltung, bis der Store wieder zu `Active` Status. Mit dieser Funktion können Sie Ihre Store-Aktivität auf regionaler Ebene steuern, ohne dass Sie Ihren Amazon-Store neu integrieren oder neu integrieren müssen oder historische Bestellungen- und Verkaufsdaten verloren gehen.

   - **[!UICONTROL Delete]** - Wählen Sie aus, einen nicht mehr benötigten Store zu löschen.

      Wählen Sie aus, wann Sie einen vorhandenen Amazon-Store und dessen Integrationseinstellungen mit Ihrem [!DNL Amazon Seller Central] -Konto. Durch das Löschen des Kontos wird der Store aus dem Amazon-Vertriebskanal entfernt, einschließlich aller Kontoeinstellungen, Auflistungen, Protokolle und anderer Informationen zu diesem Store. Der Store kann nach dem Löschen nicht abgerufen werden. Es muss ein neuer Store erstellt werden.

>[!NOTE]
>Um die während der Integration dem Store zugewiesene Website zu ändern, müssen Sie den Store löschen und den Store erneut mit der anderen Website hinzufügen, die während der Store-Integration definiert wurde.

| Store Card | Beschreibung |
|--- |--- |
| Top-Bereich | Umfasst: <br>Das Regionssymbol für den Store, das während der [Store-Integration](./store-integration.md).<br> Die zugewiesenen _[!UICONTROL Magento Website]_, definiert während der Store-Integration.<br>Die_[!UICONTROL Status]_ Ihres Ladens. Optionen: **[!UICONTROL Active]** - Die Speicherintegration ist mit Amazon abgeschlossen und überprüft und steht für die Verkaufsaktivität zur Verfügung. **[!UICONTROL Inactive]** - Die Speicherintegration ist abgeschlossen, wird jedoch nicht verwendet oder steht nicht für Verkaufsaktivitäten zur Verfügung. Wann `Inactive`, werden Ihre Amazon-Verkäufe ausgesetzt. Wann `Active`, Verkaufsumsatz und zusätzliche Einstellungen, die vor der Aktivierung aktualisiert werden sollen.<br>Die *[!UICONTROL Last Updated]* Datum der letzten Änderung am Amazon Store-Setup.<br>Die *[!UICONTROL Created]* Datum, an dem der Amazon Store im Amazon-Vertriebskanal erstellt wurde. |
| Zweiter Abschnitt | Enthält ein Zusammenfassungsdiagramm zu Store-Aktivitäten für die letzten 30 Tage sowie Hinweise und Warnhinweise für alle Einträge, die beachtet werden müssen. |
| Unterer Bereich | Umfasst die Optionen &quot;Store anzeigen&quot;und &quot;Aktion&quot;.<br>So öffnen Sie den Store [Dashboard](./amazon-store-dashboard.md)klicken **[!UICONTROL View Store]**.<br>Um einen Store zu aktivieren, zu deaktivieren oder zu löschen, klicken Sie auf **[!UICONTROL Actions]**. |
