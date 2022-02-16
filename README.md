# Mixer_analog_DJB3

15 juin 2020 - 30 décembre 2020

Sommaire

Schema bloc, introduction
Tranche Phono/line
Autres éléments
PCB design
Montage
Démonstration
Sources

## Introduction

Voici le schéma du mixer V1 DJB3, pensé pour ressembler à un rotary mixer professionnel tel que la E&S DJR-400 ou la  Rane MP2015. 
Elle comprend 3 entrées Phono/Line pour tout type de signaux. De la platine vinyle aux drums machines et synthétiseurs. La première étape a été la modélisation 3d effectuée sur Blender
Chaque tranche est composée d’un equalizer 2 bandes grave/aigu sur les modèles de Baxandall.
Ensuite il y a un préamplificateur doté d’un switch selon la source entrante. Le coté phono se chargera d’appliquer la courbe RIAA et le gain est fixe (environ +40 dB à 20 Hz et +20 dB à 1 kHz). Le coté line sera doté d’un potentiomètre de gain à régler selon les besoins. 

Il y aura une carte amplificatrice BF en kit en sortie pour assurer la sommation et une puissance sonore convenable.
À celui ci sera relié un Vu mètre pour vérifier le niveau sonore en temps réel.

L’alimentation pour fournir le +12/-12v reste encore à déterminer lors de la phase de test pour connaitre la consommation réelle de l’appareil. Les tests devront s’effectuer avec une alimentation stabilisée réglable de laboratoire.

## Tranche phono/line

Nous allons détailler la composition de la tranche (encadré saumon du schéma bloc). Le schéma électronique est le suivant. C’est la partie du projet qui est à réaliser.

### Remarque
La courbe RIAA et donc le switch Phono/line devra être placé avant le correcteur de tonalité pour ne pas fausser la correction mais avant la résistance de sommation.

## PCB design

Le choix du type de mixer : modulaire
À partir du schéma, il faut choisir les bonnes empreintes correspondant aux composants préalablement achetés. Ensuite j’ai dessiné un premier schéma pas très concluant et pas très stratégique, après quelques révisions et modifications comme la largeur des pistes d’alimentation ainsi que la lecture plus logique du schéma on obtient le gerber présent dans le repository

## Montage

Entre temps je me suis rendu compte que j’avais fait une erreur dans le design du pcb et le potentiomètre qui règle l’égalisation des basses est à l’envers. Quelques heures de soudures et les soucis arrivent. Après avoir terminé les soudures sur la première tranche, je teste le son. Première bonne nouvelle, il y a du son ! Ensuite le gain en LINE fonctionne. Maintenant je branche un casque et là malheureusement je me rends compte que le son ne sort que d’un côté.
Je passe à la deuxième tranche qui marche en stéréo sans soucis puis à la 3e ou j’ai encore ce problème d’absence de son d’un côté, je soupçonne un problème de masse lié à mon alimentation ou aux connecteurs audio bas de gamme.
La partie montage pur débute avec la préparation d’une boite (à partir d’une plaque d’acier pliée avec une plieuse à zinc) et de trous pour les potentiomètres sur la face avant 

## Sources

https://www.sonelec-musique.com/electronique_realisations.html 

http://www.musicarius.com/blog/le-guide-dachat/le-guide-dachat-de-la-sono/le-guide-de-la-sonorisation/la-table-de-mixage 

http://users.otenet.gr/~athsam/2ch_mixer_eng.htm 



