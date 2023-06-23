# ansible-assessment

## Aufgabenstellung

Die durch dieses Repository verwalteten Server soll installiert werden.
Dafür sollst du ein entsprechendes Ansible Playbook schreiben, welches folgende
Tasks auf **allen Servern der Gruppe Webserver** ausführt:

- Das Betriebssystem auf den neusten Stand bringt
- Installation der Pakete htop, tmux und den Webserver Nginx
- Management des Nginx-Dienstes, d.h. am Ende des Ansible runs
  - soll der Dienst laufen
  - soll der Dienst bei einem allfälligen Systemneustart automatisch starten
- Beim Aufruf von http://<server> wird ein `index.html` ausgeliefert, welches
  den Benutzer mit einem "Herzlich Willkommen auf <FQDN>" begrüsst.

Deine Lösung der obigen Tasks erwarten wir als Pull-Request (PR) hier in diesem
Repo. Diesen können wir dann reviewen.

## Vorgaben

Das Inventar der Server ist vorgegeben, ebenso das `index.html`-Template,
welches die Variable `greeting` enthält.

Falls du den Code auch testen möchtest, bietet dieses Repo zu Testzwecken:

- ein Conda-Environment, welches Ansible und weitere Software installieren kann
- ein Vagrantfile, um mittels Vagrant passende lokale virtuelle Server zu
erstellen
