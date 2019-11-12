Ce fichier est un export du sujet disponible [ici](http://www-poleia.lip6.fr/~kant/Ens/M2/MOSIMA/Projet/MT-2019.html)

### ![](http://www-poleia.lip6.fr/~kant/Ens/M2/MOSIMA/Logo_SU.jpg)

### Master d'Informatique Spécialité [ANDROIDE](http://androide.lip6.fr/)  
Année 2019-2020

# Modélisation et Simulation Multi-Agents (MOSIMA)

# Projet : Marché du travail simplifié - Courbe de Beveridge

Ce projet porte sur un modèle simplifié du marché du travail à base d'agents hétérogènes. Il est fondé sur un article de Z. Lewkovicz, N. Stefanovitch et C. Sommer (2007) "Emergence of the Matching Function in Multi-Agent Based Simulations of the Labor Market", Worskhop LIP6/NII, Novembre 2007 ([pdf](http://www-poleia.lip6.fr/~kant/Ens/M2/MOSIMA/Projet/Lew.pdf)). _(on oubliera l'annexe A, supprimée du pdf car hors sujet du projet)_
 
**L'objectif est de réaliser une simulation complète du modèle en Netlogo et de reproduire tous les résultats de l'article. <u>Tout résultat non expliqué ou non commenté sera considéré comme nul.</u>**
 
 **Pour l'implémentation, vous avez le choix comme plateforme de simulation multi-agents entre**
 
 *   **Netlogo**
 
 *   **Repast Symphony avec Java** : voir leur [**site**](https://repast.github.io/repast_simphony.html) ; info sur le **couplage avec Java [ici](https://repast.github.io/docs/RepastJavaGettingStarted.pdf)**
 
 Le projet est à réaliser en binôme et devra être rendu pour le **dimanche 24 novembre 23h00 au plus tard**, sous forme d'un fichier zip (`_ProjetMOSIMA_binome1_binome2.zip_`) contenant :

1.  votre **code**, complet et commenté
2.  **Si vous avez choisi Repast / Java : un fichier install.txt décrivant les installations éventuelles (pour Repast notamment) afin que je puisse faire tourner votre code avec Eclipse**
3.  votre **rapport** en **pdf** qui répond aux questions ci-dessous. Pensez à y inclure des copies d'écran pour illustrer vos résultats (courbes obtenues notamment).

_**Le barême est indicatif et susceptible d'être modifié.**_

**Tout résultat non expliqué ou non commenté sera considéré comme nul .**

## 1\. Modèle de base
 
**1.1** **Etudier le modèle** de base proposé _(1 pt)_
 
 **1.1.1** Quels sont les agents ? Leurs attributs ? Leurs comportements ? _(1 pt)_
 
 **1.1.2** Ecrivez toutes les formules ou les algorithmes (en peudo-code) permettant de calculer l'ensemble du modèle. On décrira (en pseudo code) notamment la boucle principale ("tick") de la simulation. _(1 pt)_
 
 **1.2** **Programmer le modèle** en pensant également à l'utilisation de votre programme pour la simulation, i.e. la conception de l'interface.
 
**1.2.1** Quels sont les paramètres de la simulation ? _(1 pt)_

**1.2.2** On souhaite visualiser en temps réels les agents et leurs interactions. Que proposez-vous ? _(1 pt)_

**1.2.3** Comment reproduire la courbe de Beveridge de l'article (e.g. Fig. 2) directement à partir de l'interface en cliquant sur un bouton (sans passer par des fichiers extérieurs par exemple) ? _(1 pt)_
> 
**1.3** Faites tourner votre simulation pour **reproduire la courbe de Beveridge** de la Figure 2, en indiquant la valeur des paramètres utilisés et une copie d'écran du résultat. Décrivez en particulier votre procédure d'initialisation de la simulation. _(2 pts)_
> _Rappel : plus la courbe Beveridge se rapproche de l'origine, plus l'appariement entre chômeurs et postes vacants est efficace. Voir [ici](https://fr.wikipedia.org/wiki/Courbe_de_Beveridge) pour plus de précisions._
 
**1.4** Afin de mieux comprendre **l'efficacité de ce marché du travail** virtuel, nous allons maintenant l'étudier dans **4 configurations types** , en fonction de différentes valeurs de U et V à l'initialisation :
> A : U = V = 100
> 
> B : U = 100 V = 400
> 
> C : U = 100 V = 400
> 
> D: U = V = 400
>
> **Pour chacune de ces 4 configurations :**
> * Afficher **l'évolution dans le temps du taux de chômage** _(unempolyment rate_**), et du taux de vacance** _(vacancy rate)._
> * Ajoutez les **évolutions des taux d'embauches** (Hiring Rate) et de **licenciements** (Firing Rate):
    *   taux d'embauche : HR= (nombre de chômeurs embauchés / U) où U est le nombre de chômeurs
    *   taux de licenciemens : FR= (nombre d'employés / E) où E est le nombre d'employés
>
> **Décrire et expliquer les résultats.** Ces taux sont-ils stables à partir d'un certain temps ? Pourquoi ? _(2 pts)_

**1.5** Effectuez la **sensibilité aux paramètres** de votre simulation. Faites varier chaque paramètre (les autres fixés) et observez l'évolution des résultats (Beveridge, chômage,vacance, activité, embauche et licenciements). Expliquez les résultats. _(3 pts)_
 
## 2\. Extensions du modèle
 
Il s'agit d'étudier ici quelques extensions à ce modèle (trop) simple.
 
**2.1** On souhaite introduire un processus de **démission** des employés.
 
> Pour cela, proposez un _mécanisme de décision de la démission,_ en introduisant une variable de _satisfaction au travail de l'employé_ qui devra évoluer dans le temps selon des règles stochastiques simples que vous définirez.. Donner l'algorithme en pseudo code, implémentez, simulez et discutez les résultats. _(2 pts)_
 
**2.2** Quelles sont **autres limites du modèle** ? Quelles pistes suggérez-vous pour l'améliorer ? _(2 pts)_

**2.3** Parmi les améliorations suggérées, **en choisir deux, implémentez et testez en discutant les résultats.** _(4 pts)_

