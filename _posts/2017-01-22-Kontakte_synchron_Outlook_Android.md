---
layout: post
title: Kontakte zwischen Outlook und Android synchronisieren
---

### Getestet mit:
1. Synology-NAS DS-216+II
2. Microsoft Outlook 2016
3. Android Handy (Samsung Galaxy S2plus)

### Anleitung:

#### Carddav Server installieren

* Im Paketmanager Carddav Server auswählen und installieren
  ![CardDav-Installation 1]({{ site.url }}/../images/synology/carddav_installieren.png)

* In den Einstellungen https aktivieren und Port einstellen.
  ![CardDav-Installation 1]({{ site.url }}/../images/synology/carddav_installieren_2.png)

#### Outlook CalDav Synchronizer installieren
Der Outlook CalDav Synchronizer ist ein OpenSource Projekt, welches aus einer Masterarbeit, an der Fachhochschule Technikum Wien, entstanden ist.

* Installationsdatei downloaden
  
  [Download-Link](https://sourceforge.net/projects/outlookcaldavsynchronizer/)

* Datei entpacken

  ![outlookcaldavsynchronizer 1]({{ site.url }}/../images/outlook/OutlookCalDavSynchronizer-installieren_1.png)

* Installieren

  Nach der Installation gibt es eine neue Lasche in Outlook

  ![outlookcaldavsynchronizer 2]({{ site.url }}/../images/outlook/OutlookCalDavSynchronizer-installieren_2.png)

* Profil anlegen
  
  ![caldav-profile 1]({{ site.url }}/../images/outlook/CalDav_Profil_1.png)

  ![caldav-profile 2]({{ site.url }}/../images/outlook/CalDav_Profil_2.png)

  ![caldav-profile 3]({{ site.url }}/../images/outlook/CalDav_Profil_3.png)

  Wenn man als "outlook folder:" den Kontakte-Ordner des Outlook-Kontos auswählt, werden die Kontakte direkt ins Microsoft-Outlook-Konto (outlook.com) synchronisiert. 
  Möchte man das nicht sollte, man einen anderen Ordner, ev. in einem anderen Email-Konto, auswählen.


#### CardDAV-Sync Free auf Android installieren

* Installation über google-play

  [Download CardDAV-Sync Free](https://play.google.com/store/apps/details?id=org.dmfs.carddav.sync&hl=de)

  Bei "server name or URL" folgendes eingeben: 

      https://synology-server-url:8443/addressbooks/users/name/addressbooks
