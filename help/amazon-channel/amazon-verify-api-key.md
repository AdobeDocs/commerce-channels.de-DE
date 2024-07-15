---
title: Hinzufügen oder Überprüfen des Amazon-API-Schlüssels
description: In Ihrer Commerce-Konfiguration können Sie mit dem validierten Amazon-API-Schlüssel Ihre Geschäfte in Ihr Amazon-Verkaufskonto integrieren.
role: Admin, Developer
feature: Sales Channels, Integration, Tools and External Services
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Hinzufügen oder Überprüfen des Amazon-API-Schlüssels

Beim Zugriff auf den Amazon-Vertriebskanal überprüft und validiert [!DNL Commerce] automatisch den Amazon-API-Schlüssel, den Sie in Ihrer Store-Konfiguration hinzugefügt haben. Wenn dies validiert wurde, können Sie mit dem nächsten Schritt [Speicherintegration](./store-integration.md) fortfahren.

Wenn der Amazon-API-Schlüssel fehlt, ungültig oder abgelaufen ist, müssen Sie Ihren Schlüssel aktualisieren. Es wird eine Meldung angezeigt, in der Sie aufgefordert werden, einen API-Schlüssel abzurufen und ihn zu Ihrer Amazon-Vertriebskanalkonfiguration hinzuzufügen.

## Abrufen und Hinzufügen des Amazon-API-Schlüssels nach Aufforderung

Der API-Schlüssel wird jedes Mal überprüft, wenn Sie auf Ihren Amazon-Vertriebskanal zugreifen.

1. Melden Sie sich bei [!DNL Commerce] Admin an.

1. Gehen Sie auf der _[!UICONTROL Admin]_Seitenleiste zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Wenn Sie zum ersten Mal auf den Amazon-Vertriebskanal zugreifen oder Ihr API-Schlüssel aktualisiert werden muss, fordert Sie das System dazu auf, den Vorgang abzuschließen.

   ![Abrufen und Hinzufügen der Amazon API-Schlüsselaufforderung](assets/amazon-api-verification-prompt.png){width="500"}

1. Klicken Sie auf **[!UICONTROL Sign in]** , um auf Ihr [!DNL Commerce] -Webkonto zuzugreifen.

   Die Seite Commerce-Konten wird in einer neuen Browserregisterkarte geöffnet.

   - Wenn Sie bei Ihrem [!DNL Commerce] -Konto angemeldet sind, wird der Abschnitt _[!UICONTROL API Portal]_der Seite_[!UICONTROL My Account]_ automatisch angezeigt.

   - Wenn Sie nicht angemeldet sind, werden Sie aufgefordert, Ihren Benutzernamen und Ihr Passwort für das [!DNL Commerce]-Konto einzugeben, bevor die Registerkarte _[!UICONTROL API Portal]_angezeigt wird.

   - Wenn Sie kein Konto haben, besuchen Sie [die [!DNL Commerce] Kontoseite](https://account.magento.com/customer/account/login/){target="_blank"} und registrieren Sie sich. Dieses Konto sollte Teil Ihres Unternehmens oder Ihres Unternehmens sein.

1. Bei Bedarf können Sie API-Schlüssel auf der Registerkarte _[!UICONTROL API Portal]_in Ihrem [!DNL Commerce]-Konto anzeigen und generieren.

   Geben Sie zum Erstellen eines API-Schlüssels eine Beschreibung wie `Amazon Sales Channel` ein und klicken Sie auf **[!UICONTROL Add New]**. Der neue Schlüssel wird generiert und mit dem eingegebenen Namen angezeigt. Klicken Sie auf **[!UICONTROL Copy]** , um den neuen Schlüssel zu kopieren.

   ![API-Schlüssel generieren oder kopieren](assets/amazon-add-api-key.png){width="500" zoomable="yes"}

1. Kehren Sie mit dem neu generierten und kopierten Schlüssel zur Registerkarte _[!UICONTROL Amazon Sales Channel]_im Browser zurück.

1. Klicken Sie auf der Seite _[!UICONTROL Welcome to Amazon Sales Channel]_auf **[!UICONTROL Add the key]**.

   Der Browser verlässt den Amazon-Verkaufskanal und eine Speicherkonfigurationsseite öffnet die Seite _[!UICONTROL Api Keys]_im Admin [!DNL Commerce]. Sie können diese Seite manuell öffnen, wenn Sie zu **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]** gehen, im linken Bereich **[!UICONTROL Services]** erweitern und **[!UICONTROL Magento Services]** auswählen.

1. Fügen Sie den kopierten Schlüssel für **[!UICONTROL Production Api key]** ein.

1. Klicken Sie auf **[!UICONTROL Save Config]**. Sie können jetzt zum Amazon-Vertriebskanal zurückkehren.

   ![Hinzufügen Ihres API-Schlüssels in Ihrer Store-Konfiguration](assets/config-magento-services-api-screen.png){width="600" zoomable="yes"}

1. Gehen Sie auf der _[!UICONTROL Admin]_Seitenleiste zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Überprüfen und validieren Sie Ihren API-Schlüssel, indem Sie erneut auf die Amazon Sales Channel-Trigger [!DNL Commerce] zugreifen und den Vorgang fortsetzen können.

   Wenn Sie aufgefordert werden, den Schlüssel erneut zu überprüfen, wiederholen Sie diesen Vorgang &quot;_Hinzufügen und Überprüfen_&quot;.

![Nächstes Symbol](assets/btn-next.png) [**Weiter zur Store-Integration**](./store-integration.md)
