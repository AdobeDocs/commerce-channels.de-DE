---
title: Hinzufügen oder Überprüfen des Amazon API-Schlüssels
description: In Ihrer Commerce-Konfiguration können Sie mit dem validierten Amazon-API-Schlüssel Ihre Stores in Ihr Amazon Seller-Konto integrieren.
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Hinzufügen oder Überprüfen des Amazon-API-Schlüssels

Beim Zugriff auf den Amazon-Vertriebskanal überprüft und validiert [!DNL Commerce] automatisch den Amazon-API-Schlüssel, den Sie in Ihrer Store-Konfiguration hinzugefügt haben. Wenn dies validiert wurde, können Sie mit dem nächsten Schritt [Store-Integration](./store-integration.md) fortfahren.

Wenn der Amazon-API-Schlüssel fehlt, ungültig oder abgelaufen ist, müssen Sie Ihren Schlüssel aktualisieren. Es wird eine Meldung angezeigt, in der Sie aufgefordert werden, einen API-Schlüssel abzurufen und ihn zu Ihrer Amazon-Vertriebskanalkonfiguration hinzuzufügen.

## Abrufen und Hinzufügen des Amazon-API-Schlüssels nach Aufforderung

Der API-Schlüssel wird jedes Mal überprüft, wenn Sie auf Ihren Amazon-Vertriebskanal zugreifen.

1. Melden Sie sich bei [!DNL Commerce] Admin an.

1. Navigieren Sie in der Seitenleiste _[!UICONTROL Admin]_zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Wenn Sie zum ersten Mal auf den Amazon-Vertriebskanal zugreifen oder Ihr API-Schlüssel aktualisiert werden muss, fordert Sie das System dazu auf, den Vorgang abzuschließen.

   ![Abrufen und Hinzufügen der Amazon API-Schlüsselaufforderung](assets/amazon-api-verification-prompt.png)

1. Klicken Sie auf **[!UICONTROL Sign in]** , um auf Ihr [!DNL Commerce]-Webkonto zuzugreifen.

   Die Seite &quot;Commerce-Konten&quot;wird in einer neuen Browser-Registerkarte geöffnet.

   - Wenn Sie bei Ihrem [!DNL Commerce]-Konto angemeldet sind, wird der _[!UICONTROL API Portal]_-Abschnitt der_[!UICONTROL My Account]_-Seite automatisch angezeigt.

   - Wenn Sie nicht angemeldet sind, werden Sie aufgefordert, Ihren [!DNL Commerce]-Kontonamen und Ihr Kennwort einzugeben, bevor die Registerkarte _[!UICONTROL API Portal]_angezeigt wird.

   - Wenn Sie kein Konto haben, besuchen Sie [die [!DNL Commerce] Kontoseite](https://account.magento.com/customer/account/login/){target=&quot;_blank&quot;} und registrieren Sie sich. Dieses Konto sollte Teil Ihres Unternehmens oder Ihres Unternehmens sein.

1. Bei Bedarf können Sie API-Schlüssel auf der Registerkarte _[!UICONTROL API Portal]_in Ihrem [!DNL Commerce]-Konto anzeigen und generieren.

   Um einen API-Schlüssel zu erstellen, geben Sie eine Beschreibung wie `Amazon Sales Channel` ein und klicken Sie auf **[!UICONTROL Add New]**. Der neue Schlüssel wird generiert und mit dem eingegebenen Namen angezeigt. Klicken Sie auf **[!UICONTROL Copy]** , um den neuen Schlüssel zu kopieren.

   ![API-Schlüssel generieren oder kopieren](assets/amazon-add-api-key.png)

1. Kehren Sie mit dem neu generierten und kopierten Schlüssel zur Registerkarte _[!UICONTROL Amazon Sales Channel]_im Browser zurück.

1. Klicken Sie auf der Seite _[!UICONTROL Welcome to Amazon Sales Channel]_auf **[!UICONTROL Add the key]**.

   Der Browser verlässt den Amazon-Verkaufskanal und eine Store-Konfigurationsseite öffnet die _[!UICONTROL Api Keys]_-Seite in der [!DNL Commerce]-Admin-Konsole. Sie können diese Seite manuell öffnen, wenn Sie zu **[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]** gehen, **[!UICONTROL Services]** im linken Bereich erweitern und **[!UICONTROL Magento Services]** auswählen.

1. Fügen Sie den kopierten Schlüssel für **[!UICONTROL Production Api key]** ein.

1. Klicken Sie auf **[!UICONTROL Save Config]**. Sie können jetzt zum Amazon-Vertriebskanal zurückkehren.

   ![Hinzufügen Ihres API-Schlüssels in Ihrer Store-Konfiguration](assets/config-magento-services-api-screen.png)

1. Navigieren Sie in der Seitenleiste _[!UICONTROL Admin]_zu **[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Der erneute Zugriff auf Amazon Sales Channel-Trigger [!DNL Commerce] überprüft und validiert Ihren API-Schlüssel und ermöglicht Ihnen den Fortfahren.

   Wenn Sie aufgefordert werden, den Schlüssel erneut zu überprüfen, wiederholen Sie diesen Vorgang _Hinzufügen und Überprüfen_.

![Nächstes ](assets/btn-next.png) [**SymbolWeiter zur Speicherintegration**](./store-integration.md)
