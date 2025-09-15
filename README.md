# Conteneur-TPBash-1

1) Mise en place
CMD : PWD

Réponse : (rajout clue.txt)
chemin courant = /workspaces/Conteneur-TPBash-1/workshop/alpha/clue.txt

2) Multiples indices

CMD : grep -x "PING" hints.txt | wc -l

Réponse :

2

3) Le bon ordre
CMD : sort order.txt | uniq

Réponse :
cloud
devops
docker
linux

4) Filtrage précis

CMD : cut -c 1 stack.txt

Réponse :
d
l
d
l
c
d

5) Une histoire de casse 

CMD : cat motto.txt | tr '[:upper:]' '[:lower:]'

Réponse : 

devops loves linux

6) Les bords comptent

CMD : tail -n 1 clue.txt

Réponse : 

Le deuxième mot est IS

7) Remontée de logs

CMD : head -n 3 logs.txt
      tail -n 2 logs.txt

Réponse : 

@AlexandreAnc ➜ /workspaces/Conteneur-TPBash-1/workshop/bravo (main) $ head -n 3 logs.txt
GIANTS Engine Runtime 5.0.1 (build date: Oct 18 2012)
Copyright (c) 2008-2012, GIANTS Software GmbH (www.giants-software.com), All Rights Reserved.
Copyright (c) 2003-2012, Christian Ammann and Stefan Geiger, All Rights Reserved.
@AlexandreAnc ➜ /workspaces/Conteneur-TPBash-1/workshop/bravo (main) $ tail -n 2 logs.txt
  OS: Windows NT 6.1 64-bit
Physics System

8) Permissions (mini-énigme)

CMD : chmod go-r secret.txt
      ls -l secret.txt

Réponse : 

-rw--w--w- 1 codespace codespace 26 Sep 15 09:54 secret.txt

9) Reconstitution de la phrase

CMD : 