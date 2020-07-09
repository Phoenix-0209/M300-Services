# M300-Services
M300-Services
Hell000 W0rld "#thisisn0tatest"


Erschaffen des Vagrantfile:

![1](/Pictures/1.png)

Docker Provisioning Funktion entdeckt:

![1](/Pictures/2.png)

1.Versuch die Provisioning Funktion im Vagrantfile einzubauen:

![1](/Pictures/3dockerprovisioning.png)

Ubuntu VM started, jedoch wird kein Docker installiert:

![1](/Pictures/4gitbashdockerfailure.png)

Anderer Versuch, mit "shell" Provisioning versuche ich direkt die Commands zur installation von docker zu implmentieren, jedoch schlägt dies immernoch fehl:

![1](/Pictures/5atomundbashwithoutyes.png)

Nun habe ich erkannt, dass noch ein "-y" fehlt um den installationscommand ganz am ende zu bestätigen:

![1](/Pictures/6atombashwithYes.png)

Ich versuche nun den letzten installationscommand erneut manuell durchzuführen, in der hoffnung, dass es wenigstens so klappt, jedoch ist das resultat konsistent und ich erhalte immernoch die Fehlermeldung "Hash Sum mismatch"

![1](/Pictures/7manuelinstalldocker.png)
![1](/Pictures/8manuelinstalldocker.png)

Mein Workaround welchen ich mit Hilfe von Miguel erarbeitet habe sieht nun wie folgt aus und installiert erfolgreich Docker:

Workaround: sudo apt-get install docker.io

![1](/Pictures/9dockerisinstalled.png)

Die VM hat erfolgreich eine IP Adresse erhalten.

![1](/Pictures/10vmhasip.png)

Ich kann die VM von meinem Host aus Pingen.

![1](/Pictures/11vmispingable.png)

Nun möchte ich einen Apache container installieren, mit folgenden Commands

![1](/Pictures/12installapachecontainerwebsite.png)
![1](/Pictures/13installapachecontainerwebsite.png)

leider kam zum schluss stetig einen "Unknown Error" welchen ich nicht zu lösen in der Lage war.

![1](/Pictures/14apacheerror.png)
