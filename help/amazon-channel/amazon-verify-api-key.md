---
title: Amazon API-Schlüssel Hinzufügen oder überprüfen
description: In Ihrer Commerce-Konfiguration ermöglicht Ihnen der validierte Amazon API-Schlüssel die Integration Ihrer Geschäfte mit Ihrem Amazon Seller-Konto.
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Amazon API-Schlüssel Hinzufügen oder überprüfen

beim Zugriff auf Amazon Sales Kanal, [!DNL Commerce] überprüft und validiert automatisch den Amazon API-Schlüssel, den Sie in Ihrer Store-Konfiguration hinzugefügt haben. Wenn validiert, können Sie mit dem nächsten Schritt fortfahren. [Integration speichern](./store-integration.md).

Wenn der Amazon API-Schlüssel fehlt, ungültig oder abgelaufen ist, müssen Sie den Schlüssel aktualisieren. Es wird eine Meldung angezeigt, in der Sie aufgefordert werden, einen API-Schlüssel zu erhalten und ihn Ihrer Amazon Sales Kanal-Konfiguration hinzuzufügen.

## Amazon API-Schlüssel bei Aufforderung abrufen und hinzufügen

Der API-Schlüssel wird jedes Mal überprüft, wenn Sie auf Ihren Amazon Sales Kanal zugreifen.

1. Anmelden bei [!DNL Commerce] Admin.

1. Auf _[!UICONTROL Admin]_Sidebar, Gehe zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Wenn Sie zum ersten Mal auf Amazon Sales Kanal zugreifen oder Ihr API-Schlüssel aktualisiert werden muss, fordert das System Sie während des Vorgangs auf.

   ![Eingabeaufforderung für Amazon API-Schlüssel abrufen und Hinzufügen](assets/amazon-api-verification-prompt.png)

1. Klick **[!UICONTROL Sign in]** , um auf [!DNL Commerce] Webkonto.

   Die Seite Commerce-Konten wird in einer neuen Browserregisterkarte geöffnet.

   - Wenn Sie bei Ihrem [!DNL Commerce] Konto, _[!UICONTROL API Portal]_Abschnitt_[!UICONTROL My Account]_ Seite wird automatisch angezeigt.

   - Wenn Sie nicht angemeldet sind, werden Sie aufgefordert, Ihre [!DNL Commerce] Benutzername und Kennwort des Kontos vor _[!UICONTROL API Portal]_angezeigt.

   - Wenn Sie kein Konto haben, besuchen Sie [die [!DNL Commerce] Kontoseite](https://account.magento.com/customer/account/login/){Zielgruppe=&quot;_blank&quot;} und registrieren. Dieses Konto sollte Teil Ihrer Firma oder Ihres Geschäfts sein.

1. Bei Bedarf können Sie API-Schlüssel auf der _[!UICONTROL API Portal]_in der [!DNL Commerce] Konto.

   Geben Sie zum Erstellen eines API-Schlüssels eine Beschreibung wie `Amazon Sales Channel` und klicken **[!UICONTROL Add New]**. Der neue Schlüssel wird erstellt und mit dem von Ihnen eingegebenen Namen angezeigt. Klick **[!UICONTROL Copy]** um den neuen Schlüssel zu kopieren.

   ![API-Schlüssel erstellen oder kopieren](assets/amazon-add-api-key.png)

1. Kehren Sie mit dem neuen Schlüssel erstellt und kopiert zum _[!UICONTROL Amazon Sales Channel]_im Browser.

1. Auf _[!UICONTROL Welcome to Amazon Sales Channel]_Seite, klicken **[!UICONTROL Add the key]**.

   Der Browser verlässt den Amazon Sales Kanal und eine Store-Konfigurationsseite öffnet die _[!UICONTROL Api Keys]_Seite im [!DNL Commerce] Admin. Sie können diese Seite manuell öffnen, wenn Sie zu **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**, erweitern **[!UICONTROL Services]** im linken Bereich und wählen Sie **[!UICONTROL Magento Services]**.

1. Kopierten Schlüssel einfügen für **[!UICONTROL Production Api key]**.

1. Klick **[!UICONTROL Save Config]**. Sie können jetzt zum Amazon Sales Kanal zurückkehren.

   ![Ihren API-Schlüssel in Ihrer Store-Konfiguration hinzufügen](assets/config-magento-services-api-screen.png)

1. Auf _[!UICONTROL Admin]_Sidebar, Gehe zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Wiederaufnahme des Zugriffs auf Amazon Sales Kanal-Trigger [!DNL Commerce] überprüfen und validieren Sie Ihren API-Schlüssel und können fortfahren.

   Wenn Sie aufgefordert werden, den Schlüssel erneut zu bestätigen, wiederholen Sie dies _hinzufügen und Überprüfen_ verarbeiten.

![Nächstes Symbol](assets/btn-next.png) [**Integration weiter speichern**](./store-integration.md)
