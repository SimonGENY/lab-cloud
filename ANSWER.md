# 1.
Qu'est-ce qu'une instance Virtual Machine ?

 Une instance est une machine virtuelle (VM) hébergée sur l'infrastructure de Google.

# 2.
Qu'est-ce qu'un VNET ?

Dans Microsoft Azure, un réseau virtuel, ou VNet (Virtual Network), est la continuité du réseau physique de l’entreprise, mais dans le cloud.

# 3.
A quoi sert un NSG ?

Les Network Security Group correspondent dans Azure à ce que l’on appelle des matrices de flux. Il s’agit  d’un pare-feu logiciel qui s’applique sur différents éléments azure:

- Cartes réseaux/serveurs
- Base de données
- Passerelle VPN
- Sous réseau
- Tag/balise (depuis le 15 janvier)

# 4.
Quelles sont les 5 propriétés désirables du cloud ?

Les cinq caractéristiques essentielles du Cloud computing
- Accès aux services par l'utilisateur à la demande. ...
- Accès réseau large bande. ...
- Réservoir de ressources (non localisées) ...
- Redimensionnement rapide (élasticité) ...
- Facturation à l'usage.

# 5.
Qu'est-ce que l'A/B Testing ?

Le test A/B est une technique de marketing qui consiste à proposer plusieurs variantes d'un même objet qui diffèrent selon un seul critère afin de déterminer la version qui donne les meilleurs résultats auprès des consommateurs

# 6.
Comment programmer le cloud ?

Avec le cloud computing (informatique en nuage est l'exploitation de la puissance de calcul ou de stockage de serveurs informatiques distants par l'intermédiaire d'un réseau, généralement internet.)

# 7.
Quelle est la technique pour faire un déploiement sans interruption de service ?

Le déploiement continu, qui est la suite de l'integration en continue:  il consiste pour l’équipe infrastructures à scripter et automatiser les étapes de déploiement afin qu’une version livrée par le serveur CI puisse être passée en production sans attendre.
Cela passe par :

Un serveur de configuration d’infrastructures qui centralise les modèles de configuration des serveurs (production et recette), ainsi tout nouveau serveur provisionné l’est bien selon le modèle en cours. Exemples : Chef, Puppet, SaltStalk, ou Ansible.
Une automatisation maximale des tests de recette, via un outil comme Selenium, qui permet d’enregistrer et dérouler des scénarios complets de test.
Un serveur de déploiement qui va orchestrer les opérations de déploiement sur le serveur de recette, déclencher les tests, puis lancer le passage en production si ces derniers sont positifs.  Exemple pour les applications web, Capistrano.
Tout ne sera pas automatisé à 100% et il est bon de conserver des validations manuelles, mais l’idée est bien de supprimer toute les ruptures de charge non indispensables en développant au maximum l’automatisation des déploiements.
Le déploiement en production bien organisé sur une application web peut ainsi se faire sans coupure de production ou en horaire décalé sans présence humaine.

# 8.
Qu'est-ce que le Canary release ?

Le canary release est un pattern qui permet de faire tester les dernières modifications réalisées (appelée version N+1) à une tranche de population restreinte avant de réaliser un déploiement général de cette version.

# 9.
Comment changer de taille de machine virtuelle ?

Pour modifier la taille d’un disque virtuel, ouvrez le gestionnaire de machine, selection le disque dur a modifier, et augmenter ça taille.

# 10.
Qu'est-ce que le Blue/Green deployment ?

Le Blue Green deployment devient un pattern de déploiement très répandu dans le monde du devops qui a été initialement proposé Jez Humble et David Farley dans leur livre Continuous Delivery datant de 2010. Cependant si ce pattern est devenu un classique des meetup Devops, on ne la rencontre qu’assez rarement dans les entreprises.

Le Blue Green deployment propose d'avoir un environnement de production identique à celui qui est utilisé par les utilisateurs qui recevra une nouvelle version.

# 11.
Citez deux avantages du PaaS sur le IaaS ?

économiser beaucoup de temps
plus rapide


# 12.
Quelle est la différence entre le PaaS et le Serverless ?


Les principales différences résident dans la portée des principaux avantages de la technologie Serverless par rapport au PaaS. Serverless prend tous les avantages PaaS un peu plus loin avec moins d'inconvénients.


# 13.
Que veut dire Serverless ?

L'informatique sans serveur ou serverless computing est un paradigme de cloud computing dans lequel le fournisseur de serveur gère dynamiquement les ressources allouées au service client.
Le terme 'sans serveur' ne signifie pas qu'il n'y a pas de serveurs impliqués. Cela signifie qu'ils sont gérés par les fournisseurs et non par les consommateurs. 

# 14.
Citez les trois propriétés désirable du Serverless ?

La structure de coûts Serverless est pilotée par les événements, vous ne payez donc pas de frais mensuels fixes pour les services non utilisés, ce qui la rend très efficace et réduit les coûts globaux.
Serverless est microgéré afin que les ressources administratives internes puissent être utilisées pour d'autres activités
Serverlessr offre de véritables capacités de mise à l'échelle automatique aux clients

# 15.
Comment s'appelle la plus petite unité de compute déployable en Serverless ?
