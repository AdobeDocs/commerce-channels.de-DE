---
title: Hinzufügen oder Überprüfen des Amazon-API-Schlüssels
description: In Ihrer Commerce-Konfiguration können Sie mit dem validierten Amazon-API-Schlüssel Ihre Stores in Ihr Amazon Seller-Konto integrieren.
role: Admin, Developer
feature: Sales Channels, Integration, Tools and External Services
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Hinzufügen oder Überprüfen des Amazon-API-Schlüssels

Beim Zugriff auf den Amazon-Vertriebskanal [!DNL Commerce] überprüft und validiert automatisch den Amazon-API-Schlüssel, den Sie in Ihrer Store-Konfiguration hinzugefügt haben. Wenn validiert, können Sie mit dem nächsten Schritt fortfahren, [Store-Integration](./store-integration.md).

Wenn der Amazon-API-Schlüssel fehlt, ungültig oder abgelaufen ist, müssen Sie Ihren Schlüssel aktualisieren. Es wird eine Meldung angezeigt, in der Sie aufgefordert werden, einen API-Schlüssel abzurufen und ihn zu Ihrer Amazon-Vertriebskanalkonfiguration hinzuzufügen.

## Abrufen und Hinzufügen des Amazon-API-Schlüssels nach Aufforderung

Der API-Schlüssel wird jedes Mal überprüft, wenn Sie auf Ihren Amazon-Vertriebskanal zugreifen.

1. Melden Sie sich bei der [!DNL Commerce] Admin.

1. Im _[!UICONTROL Admin]_Seitenleiste, navigieren Sie zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Wenn Sie zum ersten Mal auf den Amazon-Vertriebskanal zugreifen oder Ihr API-Schlüssel aktualisiert werden muss, fordert Sie das System dazu auf, den Vorgang abzuschließen.

   ![Abrufen und Hinzufügen der Amazon API-Schlüsselaufforderung](assets/amazon-api-verification-prompt.png){width="500"}

1. Klicken **[!UICONTROL Sign in]** , um auf [!DNL Commerce] Webkonto.

   Die Seite &quot;Commerce-Konten&quot;wird in einer neuen Browser-Registerkarte geöffnet.

   - Wenn Sie bei Ihrem [!DNL Commerce] -Konto, _[!UICONTROL API Portal]_Abschnitt_[!UICONTROL My Account]_ automatisch angezeigt.

   - Wenn Sie noch nicht angemeldet sind, werden Sie aufgefordert, Ihre [!DNL Commerce] Benutzername und Kennwort des Kontos vor _[!UICONTROL API Portal]_angezeigt.

   - Wenn Sie kein Konto haben, besuchen Sie [die [!DNL Commerce] Kontoseite](https://account.magento.com/customer/account/login/){target="_blank"} und registrieren. Dieses Konto sollte Teil Ihres Unternehmens oder Ihres Unternehmens sein.

1. Bei Bedarf können Sie API-Schlüssel für die _[!UICONTROL API Portal]_in der [!DNL Commerce] -Konto.

   Geben Sie zum Erstellen eines API-Schlüssels eine Beschreibung wie `Amazon Sales Channel` und klicken Sie auf **[!UICONTROL Add New]**. Der neue Schlüssel wird generiert und mit dem eingegebenen Namen angezeigt. Klicken **[!UICONTROL Copy]** , um den neuen Schlüssel zu kopieren.

   ![API-Schlüssel generieren oder kopieren](assets/amazon-add-api-key.png){width="500" zoomable="yes"}

1. Kehren Sie mit dem neu generierten und kopierten Schlüssel zum _[!UICONTROL Amazon Sales Channel]_im Browser.

1. Im _[!UICONTROL Welcome to Amazon Sales Channel]_Seite, klicken Sie auf **[!UICONTROL Add the key]**.

   Der Browser verlässt den Amazon-Verkaufskanal und eine Store-Konfigurationsseite öffnet die _[!UICONTROL Api Keys]_in der [!DNL Commerce] Admin. Sie können diese Seite manuell öffnen, wenn Sie **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**, erweitern **[!UICONTROL Services]** im linken Bereich und wählen Sie **[!UICONTROL Magento Services]**.

1. Fügen Sie den kopierten Schlüssel für **[!UICONTROL Production Api key]**.

1. Klicken **[!UICONTROL Save Config]**. Sie können jetzt zum Amazon-Vertriebskanal zurückkehren.

   ![Hinzufügen Ihres API-Schlüssels in Ihrer Store-Konfiguration](assets/config-magento-services-api-screen.png){width="600" zoomable="yes"}

1. Im _[!UICONTROL Admin]_Seitenleiste, navigieren Sie zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Zugriff auf Amazon-Vertriebskanal-Trigger [!DNL Commerce] überprüfen und validieren Sie Ihren API-Schlüssel und ermöglichen Ihnen den Fortfahren.

   Wenn Sie aufgefordert werden, den Schlüssel erneut zu überprüfen, wiederholen Sie dies _Hinzufügen und Überprüfen_ Prozess.

![Nächstes Symbol](assets/btn-next.png) [**Weitere Speicherintegration**](./store-integration.md)
