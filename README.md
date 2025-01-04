#Projet d'Injection de Dépendances en Java  

**Réalisé par : Firdawsse Ahchouche

---

## Introduction  
Ce projet met en œuvre les concepts fondamentaux d'injection de dépendances (IoC - Inversion of Control) en Java.  
L'objectif principal est de démontrer comment réduire le couplage entre les composants d'une application en utilisant :  
- **L'instanciation statique**.  
- **L'instanciation dynamique**.  
- **L'utilisation du framework Spring** (avec configurations XML et annotations).  

---

## Structure du Projet  

### 1. **Package `dao`**  
- **`IDao`** : Interface définissant une méthode `getData()` pour récupérer des données.  
- **`DaoImpl`** : Implémentation de l'interface `IDao`.  
- Extensions :  
  - **`ext.DaoImpl2`** et **`ext.DaoImplVWS`** : Autres implémentations de `IDao`.  

### 2. **Package `metier`**  
- **`IMetier`** : Interface définissant une méthode `calcul()` pour effectuer un calcul basé sur les données fournies par `IDao`.  
- **`MetierImpl`** : Implémentation de `IMetier` utilisant un couplage faible avec `IDao`.  

### 3. **Package `pres` (présentation)**  
- **`Presentation`** : Exemple d'injection de dépendances par instanciation statique.  
- **`pres2`** : Exemple d'injection par instanciation dynamique.  
- **`presSpringXML`** : Exemple d'utilisation de Spring avec configuration XML.  
- **`presSpringAnnotations`** : Exemple d'utilisation de Spring avec annotations.  

### 4. **Classe principale**  
- **`ma.mundia.Main`** : Classe principale pour tester les différentes techniques d'injection.  

