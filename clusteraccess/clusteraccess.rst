.. clusteraccess:

.. zugang:

---------------------
Zugang zur Lab Umgebung
---------------------

Zugangs-Übersicht
-----------------
Die Lab Umgebung stehen physisch in der USA im Bundesstaat Arizona (Phoenix). Um auf diese zugreifen zu können wird ein Remote Zugriff benötigt.
Hierfür stehen 2 Optionen zur Auswahl: **Pulse VPN** *ODER* **Parallel VDI Zugang.**


.. figure:: images/zugang.png

Frame Zugang (empfohlen)
-----------------------------------

.. figure:: images/Nutanix-XiFrame_color.png

Um sich mit Frame auf die Demo Umgebung einzuloggen, den Link klicken: https://frame.nutanix.com/x/labs
Die Zugangsdaten sind mit den anderen Möglichkeiten identisch.

Pulse Secure VPN Client
-----------------------------------

.. note::
   Um den VPN Zugang zu nutzen muss ein VPN Client installiert werden, dafür werden Administrator Rechte auf Ihrem Laptop benötigt.


1.	Falls der Client bereits installiert ist bitte zu  Schritt 5 springen.
2.	Um den Client herunter zu laden bitte an folgender Website unter Verwendung der bereitgestellten Zugangsdaten anmelden: https://xlv-useast1.nutanix.com

    .. figure:: images/pulsewebsite.png

3.	Herunterladen & installieren des Clients.

    .. figure:: images/pulsedownload.png

4.	Abmelden an der Web UI.

5.	Lokal installierten Client öffnen und eine neue Verbindung mit folgenden Parametern hinzufügen:

- **Type**: "Policy Secure (UAC) or Connection Server (VPN)""
- **Name**: HPOC VPN
- **Server URL**: https://xlv-uswest1.nutanix.com

6.	Sobald der Client eingerichtet ist mit den bereitgestellten Zugangsdaten verbinden.

.. figure:: images/pulseconnected.png

Parallels VDI Zugang (optional)
-------------------------------
.. note::
  Die deutlich empfohlene Lösung um auf die HPoC Umgebung zuzugreifen ist die Pulse VPN Verbindung, da die Parallel VDI Verbindung i.d.R. deutlich langsamer ist. Für die Fälle in denen aufgrund diverser Gründe (u.a. fehlende lokale Admin Rechte) keine Pulse VPN Verbindung möglich ist, besteht alternativ noch die Option mittels Parallel VDI auf die Umgebung (u.a. auch ohne Installation eines lokalen Clients) zuzugreifen.

1.	Unter Verwendung der bereitgestellten Zugangsdaten bitte an folgender Website anmelden: https://xld-uswest1.nutanix.com

   .. figure:: images/parallel-website.png

2.	Sobald angemeldet wird Ihnen angezeigt, dass Sie derzeit noch keine Anwendung installiert haben ("no Applications Found"). Danach beginnt automatisch oder manuell die Identifizierung ob bei Ihnen eine Parallel Client Installation vorhanden ist:

   .. figure:: images/parallel-dedecting.png

3. Falls noch kein Client installiert ist, haben Sie nun die Option einen Parallel Client zu installieren (**Achtung: lokale Installationsrecht erforderlich**) oder den HTML5 WebClient ohne zusätzliche Installation zu verwenden. 

    .. figure:: images/parallel-client-detecting.png

4. Danach taucht auf der Parallel Website der für Sie bereitgestellte VDI Desktop auf - nun können Sie sich mit diesem verbinden:

  .. figure:: images/parallel-connectionapp.png

5.	Danach gelangen Sie (je nach Parallel Client Option) im Browser oder auch in der Parallel Client App auf dem VDI Desktop mit Zugang zu Ihrer HPoC Umgebung:

  .. figure:: images/parallel-vdidesktop.png
