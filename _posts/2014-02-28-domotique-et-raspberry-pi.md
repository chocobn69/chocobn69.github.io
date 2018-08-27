---
id: 123
title: Domotique et Raspberry Pi
date: 2014-02-28T11:36:32+00:00
author: admin
layout: post
guid: http://www.choco-bn.net/?p=123
categories:
  - diy
  - domotique
  - electronique
tags:
  - diy
  - domotique
  - electronique
  - raspberry pi
---
![Plus de 50 idées pour votre Raspberry Pi](http://korben.info/wp-content/uploads/2013/01/raspberrypi.jpg)

Ça fait un moment que je souhaite installer un peu de domotique dans ma maison que j'occupe depuis déjà un an (ça passe vite !). J’ai découvert que ce serait possible avec l’ordinateur qui fait la taille d’une carte de crédit, le Raspberry Pi, qui est sorti en 2012 et a de plus en plus d’usages pour les enthousiastes du DIY. On s’en est servi pour les liaisons radio, la construction de drones, de consoles de jeux rétro…

Pour moi, l'idée serait de mettre en place un ordinateur central, basé sur une carte Raspberry Pi, qui servirait à la fois de NAS, de terminal de contrôle de température intérieur, de station météo extérieure, de gestion du chauffage, de contrôle de luminaire, etc...

Je sais qu'il existe également des projets Open Source de mise en place d'alarme avec un Raspberry Pi, ça pourrait permettre de faire de sacrées économies sur ce poste.

Le principe serait de compléter [l'achat de la carte par un raspberry pi boitier ](http://radiospares-fr.rs-online.com/web/generalDisplay.html?id=raspberrypi)puis de stocker le tout dans un placard et ne m'en servir qu'en tant que serveur (ethernet ou wifi).

Pour plus d'infos sur le Raspberry Pi, vous pouvez visiter le site officiel de la carte : <http://www.raspberrypi.org/> (toutes les infos sont en anglais).

Pour avoir un aperçu de l'historique de la conception de la carte, voici une infographie sympa que j'ai trouvée sur le [blog de korben](http://korben.info/laventure-raspberry-pi.html).

[![InfographieHistoireRPIV2 kubii Laventure Raspberry Pi](http://korben.info/wp-content/uploads/2014/02/InfographieHistoireRPIV2-kubii.jpg)](http://korben.info/laventure-raspberry-pi.html)

Il me semble que Intel est entrain de développer un équivalent en plus puissant, mais je ne crois pas qu'il soit déjà en vente pour le grand public (edit : plus d'info sur la carte d'Intel, qui est beaucoup chère, [ici](http://arstechnica.com/information-technology/2013/09/199-4-2-computer-is-intels-first-raspberry-pi-competitor/)).

Concernant les entrées et sorties électroniques, vous vous doutez que je ne souhaite pas utiliser de connexions filaires : le coût et le temps d'installation seraient vraiment trop contraignants, et je ne me vois pas faire courir des fils partout dans le salon (j'en connais une qui ne serait pas d'accord…). Je pense donc utiliser des ondes radio en 433 mhz, avec un émetteur / récepteur + antenne côté serveur, et de plus petits du côté des sondes et interrupteurs.

Pour le software, vu que la carte est en fait un pc complet (processeur ARM1176JZF-S, décodeur Broadcam VideoCore IV, 512Mo de RAM, ports USB, etc..), on peut tout à fait programmer toutes les interactions en Python, ce que je ferais surement car je connais bien le langage.

Il existe un large choix de système d'exploitation incluant Raspbian, basé sur Debian, Pidora, basé sur Fedora, ainsi que plusieurs distrib à base de xbmc pour utiliser le Raspberry Pi en mode media center.

Pour ma part je partirais bien sur [Raspbian](http://www.raspbian.org/) qui me paraît bien maintenu et stable. La doc est plutôt bien fournie et le nombre de packages déjà prêts à l'emploi assez conséquent.

Il ne reste plus qu'à attaquer le projet, ce qui va être un peu dur, vu les nouveautés à la maison, on verra dans les prochains 6 mois comment mini me se porte 😉
