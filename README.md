# Modèles NuSMV pour la vérification formelle
##Description du projet
Ce projet applique les techniques de vérification formelle et de model checking CTL à un système de contrôle de feux de circulation pour un carrefour en T. L'objectif est de garantir mathématiquement la sûreté et la vivacité d'un contrôleur gérant une route principale et une route secondaire équipée d'un capteur de véhicules.
Méthodologie
Le système a été modélisé formellement à partir de quatre variables d'état (feux principal et secondaire, capteur, présence de véhicule), générant un espace de 36 états possibles. Dix propriétés temporelles ont été spécifiées en logique CTL, réparties en deux catégories :

* Propriétés de sécurité : exclusion mutuelle des feux verts, cohérence des états
* Propriétés de vivacité : réactivité du système, accessibilité de l'état par défaut

L'implémentation a été réalisée avec NuSMV, exploitant les Binary Decision Diagrams (BDD) pour optimiser la vérification symbolique.

### Résultats
La vérification a confirmé que le modèle initial satisfait l'ensemble des propriétés spécifiées. Une extension avec un état intermédiaire (deux feux rouges simultanément) a permis d'analyser l'impact des modifications structurelles et de démontrer la capacité du model checking à détecter automatiquement les violations de spécifications.
Compétences développées

* Modélisation formelle de systèmes réactifs
* Spécification de propriétés en logique temporelle CTL
* Utilisation d'outils de model checking (NuSMV)
* Analyse critique et optimisation par représentation symbolique


### Technologies : NuSMV, CTL, BDD, Vérification Formelle
