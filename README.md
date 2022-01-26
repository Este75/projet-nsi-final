# projet-nsi-final
projet final, Esteban, Jilan, Yanis
"""
#Projet de Esteban , Yanis, Jilan
#Livre où vous êtes le héros

"""

# Imports
import sys

p1 = "Vous êtes dans votre vaisseaux, un Megadeth -XW, une drôle de sensation vous submerge, vous sentez peu à peu vos forces se vider jusqu'à tomber dans les pommes."
p2 = "Vous vous réveillez et regardez un peu partout, vous êtes encore dans votre vaisseaux, mais totalement détruit. Vous devriez trouver de quoi survivre."
p3 = "Vous attrapez une carabine et une sacoche avec des munitions. le vaisseau va bientôt s'effondrer. Il serait préférable de ne pas rester là."
p4 = "Vous accourez vers la cuisine et rassemblez le plus de nourriture possible. Il serait préférable de ne pas rester là."
p5 = "Vous vous dirigez vers les rangements qui se trouve à côté de l’entrée de la cabine. Vous trouvez enfin le fameux quite de survie. Il serait préférable de ne pas rester là."
p6 = "Vous décidez de monter sur un petite montagne. Une fois arrivé en haut, vous constatez l'immensité du désert qui vous entoure, vous scruter les horizons dans l’espoire de voir un signe de vie, malheureusement vous ne voyez rien. Votre voyage ne fait que commencer..."
p7 = "Vous descendez dans la grotte. Au bout d’une ou deux minutes à errer dans la grotte, soudain vous tombez sur une chose innatendu. Votre voyage ne fait que commencer..."


#Résumé de l'histoire
print("Vous êtes dans votre vaisseaux, un Megadeth -XW.")
print("Vous vous réveiller et regardez un peu partout, vous êtes encore dans votre vaisseaux, mais totalement détruit et au bord de se faire consumer par les flammes.")
print("...")
#listes
liste_mots = ["de prendre l'arme", "de prendre un stock de nourriture", "de rester près du vaisseaux", "de quitter"]
liste_messages = ["Vous avez votre objet. Génial !", "Vous avez votre reserve de nourriture. Génial !", "Vous avez choisi la facilité", "A bientôt..."]

choix = ''
#Faites votre choix
while choix == '':
    print ("POUR PRENDRE UNE ARME TAPPER 1 !")
    print ("POUR PRENDRE UN STOCK DE NOURRITURE TAPPER 2 !")
    print ("POUR RESTER PRèS DU VAISSEAUX TAPPER 3 !")
    print ("Taper sur 0 pour quitter")
    choix = int(input('> Faites un choix : '))
    
print("vous avez choisi : ", liste_mots[choix-1])
print(liste_messages[choix-1])
    
if choix == 0:
        sys.exit()

if choix == 1:
    print(p3)
    choix1 = ''
    while choix1 == '':
        print ("POUR MONTER SUR LA PETITE MONTAGNE JUSTE A VOTRE DROITE TAPPER 1 !")
        print ("POUR ALLER DANS LA GROTTE QUI SE TROUVE A UNE DIZAINE DE MINUTES TAPPER 2 !")
        print ("Taper sur 0 pour quitter")
        choix1 = int(input('Faites un choix : '))
    if choix1 == 0:
        print('A bientôt...')
        sys.exit()
    if choix1 == 1:
        print(p6)
    if choix1 == 2:
        print(p7)
if choix == 2:
    print(p4)
    choix2 = ''
    while choix2 == '':
        print ("POUR MONTER SUR LA PETITE MONTAGNE ET SCRUTER LES HORIZONS TAPPER 1 !")
        print ("POUR ALLER DANS UNE GROTTE QUI SE TROUVE A QUELQUES METRES TAPPER 2 !")
        print ("Taper sur 0 pour quitter")
        choix2 = int(input('Faites un choix : '))
    if choix2 == 0:
        print('A bientôt...')
        sys.exit()
    if choix2 == 1:
        print(p6)
    if choix2 == 2:
        print(p7)
if choix == 3:
    print(p5)
    choix3 = ''
    while choix3 == '':
        print ("POUR MONTER SUR LA PETITE MONTAGNE ET SCRUTER LES HORIZONS TAPPER 1 !")
        print ("POUR POUR ALLER DANS UNE GROTTE QUI SE TROUVE A QUELQUES METRES TAPPER 2 !")
        print ("Taper sur 0 pour quitter")
        choix3 = int(input('Faites un choix : '))
    if choix3 == 0:
        print('A bientôt...')
        sys.exit()
    if choix3 == 1:
        print(p6)
    if choix3 == 2:
        print(p7)


