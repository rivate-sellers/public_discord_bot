
# Rivate öffentlicher Discord Bot

Unser Discord Bot soll es den Nutzern unter anderem ermöglichen, sich als Verkäufer zu bewerben und Aufträge zu erhalten. Das System soll transparent und fair sein und die Sicherheit und Vertraulichkeit der Aufträge gewährleisten.





## Funktionalitäten
### Bewerbung als Verkäufer
- Nutzer können sich als Verkäufer bewerben, indem sie auf einen Button klicken, ein Modal ausfüllen und eine Bewerbung abschicken.
![](https://media.discordapp.net/attachments/1099762343799423119/1099763641705824326/image.png?width=703&height=676)
- Bewerber können im Modal angeben, ob sie bereit sind, ein NDA zu unterzeichnen oder nicht. Außerdem müssen im Modal weitere folgende Daten angegeben werden
![](https://media.discordapp.net/attachments/1099762343799423119/1099765534444245143/image.png)
zusätzlich soll es in dem Modal einen Abschnitt geben, in welchem man seinen Bewerbungsbereich angeben kann. Desweiteren einen Abschnitt, in welchem man seine PayPal Email Adresse angeben kann. Folgende Bewerbungsbereiche werden von Rivate angeboten:
Bewerbungsbereiche |  
-------- |  
Entwicklung   | 
Design   |  
Social Media |


- Die Bewerbungen werden in einem Warteschlangensystem gespeichert und von Moderatoren geprüft.
- Wird eine Bewerbung angenommen, erhält der Nutzer Zugang zu den Aufträgen.

### Aufträge

- Das Team kann auf dem Teamserver Aufträge mit folgenden Parametern erstellen:
Parameter |  
-------- |  
Titel des Auftrags   | 
Bereich des Auftrags |
genaue Beschreibung des Auftrags   |  
Bezahlung |
ggf. ein Bild

nach dem Absenden des Auftrags wird dieser in ein Embed zusammengefasst und für den Auftragsersteller sichtbar. Dieser kann mit einem Klick auf den untenstehenden Button den Auftrag absenden, welcher dann auf den öffentlichen Discord in den entsprechenden Kanal gesendet wird.
- Wenn ein Auftrag von einem Nutzer angenommen wird, wird auch ein Modmail-Kanal mit dem Ersteller des Auftrags geöffnet. Alle Nachrichten, die in diesem Kanal gesendet werden, werden als private Nachricht an den Benutzer gesendet, um die Anonymität des Teammitglieds zu gewährleisten.

### Modmail-System

- Wenn sich ein Benutzer als Verkäufer anmeldet, wird automatisch ein Ticket-Kanal auf dem Discord-Server erstellt.
- Der Ticket-Kanal wird als Modmail-System verwendet, so dass der Benutzer alle Nachrichten, die das Team in diesen Kanal schreibt, als private Nachricht erhält.
- Das Team kann den Kanal auch nutzen, um mit dem Verkäufer zu kommunizieren, wenn es Fragen oder Bedenken gibt.

### Team-Befehle

- Das Team hat Zugriff auf spezielle Befehle, um das Verkäufersystem zu verwalten.
- Zu diesen Befehlen gehören das Annehmen und Ablehnen von Verkäuferbewerbungen, das manuelle Hinzufügen von Verkäufern, das Kicken von Verkäufern und das Anzeigen abgeschlossener Aufträge. Zudem muss es einen Befehl geben, welcher die, im Modal angegeben Informationen des Nutzers anzeigt.

### Weiteres
- Die Sprache aller Modals basiert auf der vom Benutzer gewählten Sprache. (Englisch oder Deutsch)

## Technische Umsetzung

- Der Bot wird mit der Discord API und der Programmiersprache Java, mit der [JDA ](https://jda.wiki/) Bibliothek entwickelt.
- Die Daten werden in einer [MongoDB](https://mongodb.com/) Datenbank gespeichert.




