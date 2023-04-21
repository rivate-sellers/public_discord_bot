# Öffentlicher Diskussions-Bot

## Zielsetzung

Unser Discord Bot soll es den Nutzern unter anderem ermöglichen, sich als Verkäufer zu bewerben und Aufträge zu erhalten. Das System soll transparent und fair sein und die Sicherheit und Vertraulichkeit der Aufträge gewährleisten.

## Funktionalitäten

### Bewerbung als Verkäufer

- Nutzer können sich als Verkäufer bewerben, indem sie auf einen Button klicken, ein Modal ausfüllen und eine Bewerbung abschicken.
- Bewerber können im Modal angeben, ob sie bereit sind, ein NDA zu unterzeichnen oder nicht.
- Die Bewerbungen werden in einem Warteschlangensystem gespeichert und von Moderatoren geprüft.
- Wird eine Bewerbung angenommen, erhält der Nutzer Zugang zu den Aufträgen.

### Aufträge

- Das Team kann Aufträge mit einem Festpreis erstellen, die dann vom Bot in einem Embed mit allen Informationen an einen bestimmten Kanal gesendet werden.
- Nur autorisierte Verkäufer können die Aufträge sehen und sich dafür bewerben.
- Wenn ein Auftrag angenommen wird, wird auch ein Modmail-Kanal mit dem Ersteller des Auftrags geöffnet. Alle Nachrichten, die in diesem Kanal gesendet werden, werden als private Nachricht an den Benutzer gesendet, um die Anonymität des Teammitglieds zu gewährleisten. 

### Modmail-System

- Wenn sich ein Benutzer als Verkäufer anmeldet, wird automatisch ein Ticket-Kanal auf dem Discord-Server erstellt.
- Der Ticket-Kanal wird als Modmail-System verwendet, so dass der Benutzer alle Nachrichten, die das Team in diesen Kanal schreibt, als private Nachricht erhält.
- Das Team kann den Kanal auch nutzen, um mit dem Verkäufer zu kommunizieren, wenn es Fragen oder Bedenken gibt.
### Team-Befehle

- Das Team hat Zugriff auf spezielle Befehle, um das Sellersystem zu verwalten.
- Zu diesen Befehlen gehören das Annehmen und Ablehnen von Verkäuferbewerbungen, das manuelle Hinzufügen von Verkäufern, das Kicken von Verkäufern und das Anzeigen abgeschlossener Aufträge.

### Weiteres
- Die Sprache aller Modals basiert auf der vom Benutzer gewählten Sprache. (Englisch oder Deutsch)

## Technische Umsetzung

- Der Bot wird mit der Discord API und der Programmiersprache Java, mit der [JDA ](https://jda.wiki/) Bibliothek entwickelt.
- Die Daten werden in einer [MongoDB](https://mongodb.com/) Datenbank gespeichert.
