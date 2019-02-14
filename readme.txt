BITS Behörden-IT-Sicherheitstraining



Stand: 11.12.2018

Version 5.01


Ansprechpartner Dr. Lutz Gollan, Behörde für Inneres und Sport, Hamburg
E-Mail: Lutz.Gollan@bis.hamburg.de



1.Überblick

Unter dem Titel „BITS Behörden-IT-Sicherheitstraining“ hat im Jahr 2006 eine Arbeitsgruppe des Arbeitskreises Informationstechnologie des Städte- und Gemeindebundes Nordrhein-Westfalen das für Unternehmen konzipierte Computersicherheitstraining „open beware!“ an die Anforderungen von Verwaltungen angepasst. Mittlerweile liegt die aktualisierte Version 5 vor. Seit Oktober 2010 wird BITS von der Kommunal Agentur NRW GmbH (https://www.kommunalagenturnrw.de) mit Unterstützung von Dr. Lutz Gollan, Behörde für Inneres und Sport, Hamburg, herausgegeben. Die letzten Änderungen sind der Changelog-Datei zu entnehmen.



2.Ziel

Durch das Training sollen die Mitarbeiterinnen und Mitarbeiter von Verwaltungen, die regelmäßig an EDV-Arbeitsplätzen und insbesondere mit dem Internet beschäftigt sind, durch gezielte Information und Selbstlerneinheiten für die Sicherheitsaspekte der Computer- und Internetnutzung sensibilisiert werden.


Das Training ist kostenlos und vollständig browserbasiert.



3.Installation und Anpassung

„BITS Behörden-IT-Sicherheitstraining“ steht als ZIP-Datei zur Verfügung. Für die Mitarbeiterschaft kann es auf einem Server, einem Arbeitsplatz oder auf einem Wechselspeichermedium (DVD, USB-Stick) entpackt werden. Da „BITS Behörden-IT-Sicherheitstraining“ HTML-basiert ist, kann es problemlos in einen Intranetauftritt integriert werden. 

BITS kann auch auf ein Microsoft Sharepoint-Verzeichnis geladen und direkt dort aufgerufen werden.



In einigen Ordnern befindet sich eine Readme.txt, die Hinweise zum Anpassen, etwa der CSS-Dateien, gibt.



Vor der Freigabe für die Mitarbeiterschaft sollte die Seite „Ansprechpersonen“ für die entsprechende Verwaltung angepasst werden. Dies ist die Datei „index.htm“ im Pfad „allgemeines\ansprechpartner“. Hierzu sind HTML-Kenntnisse erforderlich. Gleiches gilt für den Fall, dass anderslautende Dienstvereinbarungen oder -anweisungen, insbesondere für die Kapitel "E-Mail" und "Vertrauliche Daten", existieren. Diese und weitere Dokumente können über die Seite "allgemeines\dokumente" verlinkt werden.

Das Bild im Kopf von BITS ist die Datei header.jpg im Pfad "images\design" (960px breit, 140px hoch). Dazu kommt das linke Bild mit den "Logos" im gleichen Ordner (logolinks.jpg 220px breit, 140px hoch).

Bitte bedenken Sie, dass BITS nur ein Angebot darstellt und leicht auf die lokalen Anforderungen hin angepasst werden kann.



Über die Herausgeber bzw. den oben genannten Ansprechpartner kann der MD5-Hashwert der BITS-Version abgefragt werden. Dadurch soll verhindert werden, dass eine manipulierte BITS-Version heruntergeladen bzw. eingesetzt wird.



4. Bedienung und technische Anforderungen

Die Bedienung von „BITS Behörden-IT-Sicherheitstraining“ erfolgt durch den Aufruf der „index.html“-Seite (unmittelbar oder durch Verlinkung hierauf). Anschließend können die weitestgehend barrierefreien Seiten durch die Maus oder durch Tastaturbefehle genutzt werden.



BITS unterstützt grundsätzlich jeden aktuellen Browser. JavaScript muss aktiviert sein, andernfalls kommt es bei der Navigation und bei den Wissenstests zu Problemen. Eine Soundkarte bzw. Lautsprecher sind zur Nutzung nicht erforderlich. Dank des direkt eingebundenen Bootstrap-Frameworks und des responsiven Webdesigns ist auch eine Nutzung über mobile Endgeräte möglich. BITS wurde mit den Browsern MS Internet Explorer, Edge, Vivaldi, Mozilla Firefox und Chrome getestet.



5. "Gewinnspiel"

Es besteht die Möglichkeit, dass bei den Wissenschecks am Ende der Lektionen bei Anklicken der richtigen Antwort Buchstaben eingeblendet werden. Wenn die entsprechenden Buchstaben durch den Nutzer innerhalb eines Gewinnspiels der Behörde eingesendet werden, kann so ein Anreiz zur Nutzung von BITS geschaffen werden.



5.1

Das Gewinnspiel ist zunächst ausgeschaltet und wird über eine Einstellung in der CSS-Definition sichtbar gemacht.

Ändern von
	/*  Wissensquiz - Gewinnspiel einschalten / ausschalten */
		.panel-footer-quiz {
		  visibility: hidden;
		  /* visibility: visible;  */
		} 
in
	/* Wissensquiz - Gewinnspiel einschalten / ausschalten */
		.panel-footer-quiz {
		  /*  visibility: hidden; */
		  visibility: visible;  
		  }



5.2
Als Standardlösung ist folgender Satz bereite hinterlegt:
Sicherheit_entsteht,_wenn_alle_mitmachen!

Sie können diese ändern. Der Wissens-Check ist dazu jeweils in den Dateien test0*.htm in den Lektrionen in folgender Reihenfolge anzupassen:
1	\e-mail\test01.htm		Si
2	\e-mail\test02.htm		ch
3	\e-mail\test03.htm		er
4	\e-mail\test04.htm		he
5	\viren\test01.htm		it
6	\viren\test02.htm		_e
7	\viren\test03.htm		nt
8	\viren\test04.htm		st
9	\passworte\test01.htm		eh
10	\passworte\test02.htm		h
11	\passworte\test03.htm		t
12	\passworte\test04.htm		,
13	\passworte\test05.htm		_
14	\passworte\test06.htm		w
15	\internet\test01.htm		e
16	\internet\test02.htm		n
17	\internet\test03.htm		n
18	\internet\test04.htm		_
19	\vertraulich\test01.htm		a
20	\vertraulich\test02.htm		l
21	\vertraulich\test03.htm		l
22	\socialmedia\test01.htm		e
23	\socialmedia\test02.htm		_
24	\socialmedia\test03.htm		m
25	\cloud\test01.htm		i
26	\cloud\test02.htm		ma
27	\cloud\test03.htm		a
28	\cloud\test04.htm		c
29	\mobile\test01.htm		h
30	\mobile\test02.htm		e
31	\mobile\test03.htm		n
32	\mobile\test04.htm		!

Im HTML-Quellcode zum Beispiel in der Datei  \e-mailt\test01.htm die Buchstaben "Si" hinterlegt worden. Dort können im Lösungs-Bereich 
          <h4 class="modal-title">Richtig !</h4>
        		<div class="panel-footer-quiz">
				<h5>
				Zur Lösung des Quiz notieren Sie folgende Buchstaben:</h5>
				<h3>
				<span class="label label-warning">S</span>
				<span class="label label-warning">i</span>
				</h3>
				</div>
in Zeilen 163 und 164 die Buchstaben nach Belieben angepasst und bei Bedarf die Zeilen kopiert und eingefügt (bei mehr als 2 Lösungsbuchstaben) 
oder gelöscht (nur 1 Lösungsbuchstabe)			
				<span class="label label-warning">S</span>
				<span class="label label-warning">i</span>
		

6. BITS-Portal

Für Administratoren steht kostenfrei das BITS-Portal http://www.bits-portal.eu zur Verfügung. Dort werden Beta-Versionen bereitgehalten, neue Funktionen und Inhalte vorgestellt und diskutiert.



7.Rechtliches

„BITS Behörden-IT-Sicherheitstraining“ basiert auf open beware!, das von der BDG GmbH & Co. KG, jetzt NTT Security (Germany) GmbH, herausgegeben wurde.

Die Urheber sind Herr Dr. Lutz Gollan und Herr Hartmut Honermann, PureSec GmbH.



Die technische Realisierung erfolgt durch Herrn Werner Eising, Stadt Coesfeld.



BITS ist kostenlos und steht unter der Creative Commons (CC) Lizenz BY-SA (https://creativecommons.org/licenses/by-sa/3.0/de/).


Sie dürfen:

— Teilen — das Material in jedwedem Format oder Medium vervielfältigen und weiterverbreiten
-
— Bearbeiten — das Material remixen, verändern und darauf aufbauen
und zwar für beliebige Zwecke, sogar kommerziell.


Der Lizenzgeber kann diese Freiheiten nicht widerrufen solange Sie sich an die Lizenzbedingungen halten:

— Namensnennung — Sie müssen angemessene Urheber- und Rechteangaben machen, einen Link zur Lizenz (diese Seite) beifügen und angeben, ob Änderungen vorgenommen wurden. Diese Angaben dürfen in jeder angemessenen Art und Weise gemacht werden, allerdings nicht so, dass der Eindruck entsteht, der Lizenzgeber unterstütze gerade Sie oder Ihre Nutzung besonders.

— Weitergabe unter gleichen Bedingungen — Wenn Sie das Material remixen, verändern oder anderweitig direkt darauf aufbauen, dürfen Sie Ihre Beiträge nur unter derselben Lizenz wie das Original verbreiten

- Keine weiteren Einschränkungen — Sie dürfen keine zusätzlichen Klauseln oder technische Verfahren einsetzen, die anderen rechtlich irgendetwas untersagen, was die Lizenz erlaubt.



Das integrierte Bootstrap-Framework (https://getbootstrap.com/) steht unter der MIT-Lizenz, bei einer Veränderung von BITS etc. dürfen die Lizenzhinweise nicht aus dem Quelltext entfernt werden. Das Copyright für Bootstrap liegt bei Twitter.



Die Grafiken sind unterliegen der Common Criteria CC0 (https://openclipart.org/share und https://pixabay.com/). Die Grafik viren03b-bot.jpg wurde von Herrn Jörg Lekschas erstellt.

 Das Urheberrecht für die Grafik header.jpg im Kopfbereich von BITS liegt bei fotolia.de/kras99. Beim Kapitel "Cloud" hat Frau Heike Brzezina wertvolle Hinweise gegeben.



Änderungs- oder Ergänzungswünsche nimmt Dr. Lutz Gollan (Lutz.Gollan@bis.hamburg.de) gerne entgegen.



-------------------------------------------------------------
