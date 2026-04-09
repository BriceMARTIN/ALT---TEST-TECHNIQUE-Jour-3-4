# Livrable attendu - TEST TECHNIQUE Jour 3-4

`**TABLE DES MATIÈRES**`


1. [`Vue d'ensemble`](#1-vue-densemble)
2. [`Document de Conception Technique`](#2-document-de-conception-technique)
3. [`Format et Présentation`](#3-format-et-pr%C3%A9sentation)
4. [`Modalités de Remise`](#4-modalit%C3%A9s-de-remise)
5. [`Critères d'Évaluation`](#5-crit%C3%A8res-d%C3%A9valuation)


---

**1. VUE D'ENSEMBLE**

**1.1 Objectif du Test**

Ce test technique évalue votre capacité à :

* **Concevoir** une solution technique robuste et évolutive
* **Architecturer** un système complexe avec les bonnes pratiques
* **Modéliser** des données cohérentes
* **Concevoir** des interfaces utilisateur fonctionnelles
* **Communiquer** efficacement vos choix techniques

### **1.2 Durée et Organisation**

| **Livrable** | **Durée** | **Pages** |
|----------|-------|-------|
| **Conception Technique** | 2 jours | 5-6 pages max |

### **1.3 Ressources Disponibles**

* **Documentation** : Cahier des charges fourni
* **Outils** : Libres (diagrammes, maquettes, etc.)
* **Recherche** : Internet autorisé


---

## **2. DOCUMENT DE CONCEPTION TECHNIQUE**

### **2.1 Objectif**

Concevoir une solution technique complète et justifier vos choix.

### **2.2 Approche Recommandée**

**⚠️ IMPORTANT** : Compte tenu du temps limité, nous vous recommandons de :


1. **CHOISIR EN PRIORITÉ** l'une des deux approches suivantes :
   * **Option A** : Architecture Système + Modèle de Données (approche Backend)
   * **Option B** : Wireframes/UI + Modèle de Données (approche Frontend)
2. **SI IL VOUS RESTE DU TEMPS** : Compléter avec l'autre approche

Cette stratégie vous permettra de produire un livrable de qualité plutôt que de survoler tous les aspects.

### **2.3 Structure Proposée (5-6 pages max)**

#### **2.3.1 Option A : Architecture Système (2-3 pages)**

* **1 schéma d'architecture globale** (obligatoire)
* Description des **composants principaux** (modules fonctionnels)
  * Ex: module Auth, module Documents, module Paiement
* **Flux de données critiques** (auth, paiement, documents) / Diagramme de séquence
* **Choix de patterns** (Event-driven, CQRS, MVC, etc.)
* **Stack technique choisie** et justification

#### **2.3.2 Option B : Wireframes & Conception UI (2-3 pages)**

* **3-4 écrans principaux** en wireframes (obligatoire)
  * Page d'accueil/dashboard
  * Formulaire principal
  * Page de résultats/confirmation
  * Page de gestion (admin/user)
* **Parcours utilisateur** (User Journey) principal
* **Responsive design** : adaptation mobile/desktop
* **Choix d'UI/UX** justifiés (frameworks CSS, librairies, etc.)
* **Accessibilité** : RGAA/WCAG pris en compte

#### **2.3.3 Modèle de Données (2 pages) - OBLIGATOIRE**

* **Schéma au choix** : ERD, MERISE (MCD/MLD), UML ou autre notation
* **10-12 entités principales** avec relations minimum
* **Indexation et optimisations** prévues

#### **2.3.4 Annexe (1 page optionnelle)**

* **POC code snippet** d'une fonctionnalité clé
* Ou **benchmark comparatif** des solutions
* Ou **Maquette interactive** (si wireframes choisis)


---

## **3. FORMAT ET PRÉSENTATION**

### **3.1 Exigences Techniques**

#### **3.1.1 Format de Document**

* **Format** : PDF ou Markdown
* **Numérotation** : Pages numérotées

#### **3.1.2 Éléments Visuels**

* **Diagrammes** : Obligatoires pour l'architecture
* **Wireframes** : Obligatoires si option B choisie
* **Tableaux** : Privilégiés pour les comparaisons
* **Schémas** : Encouragés pour la clarté
* **Couleurs** : Autorisées mais sobres

#### **3.1.3 Structure Rédactionnelle**

* **Titres** : Hiérarchisés et numérotés
* **Paragraphes** : Courts et structurés
* **Listes** : À puces ou numérotées
* **Références** : Sources citées si nécessaire

### **3.2 Bonnes Pratiques**

#### **3.2.1 Contenu**

✅ **Synthétique** : Aller à l'essentiel\n✅ **Structuré** : Plan logique et cohérent\n✅ **Justifié** : Argumenter les choix\n✅ **Pragmatique** : Solutions réalistes

❌ **À éviter** :\n❌ Remplissage inutile\n❌ Jargon technique excessif\n❌ Solutions sur-complexes\n❌ Manque de justification

#### **3.2.2 Présentation**

* **Lisibilité** : Mise en page aérée
* **Cohérence** : Style uniforme
* **Professionnalisme** : Présentation soignée
* **Accessibilité** : Compréhensible par tous


---

## **4. MODALITÉS DE REMISE**

### **4.1 Délais**

| **Livrable** | **Échéance** | **Heure Limite** |
|----------|----------|--------------|
| **Conception Technique** | Jour J+1 | Jeudi 18H    |

### **4.2 Support et Questions**

#### **4.2.1 Types de Questions Autorisées**

✅ **Clarifications** sur le cahier des charges\n✅ **Précisions** sur les attentes techniques\n✅ **Questions techniques** sur l'environnement\n✅ **Problèmes** de compréhension

❌ **Non autorisé** :\n❌ Demande de solution\n❌ Validation des choix d'architecture\n❌ Aide à la conception


---

## **5. CRITÈRES D'ÉVALUATION**

### **5.1 Architecture Système** (si Option A)

* **Pertinence** des choix techniques
* **Respect** des bonnes pratiques
* **Cohérence** de l'architecture globale
* **Justification** des décisions techniques

### **5.2 Conception UI/UX** (si Option B)

* **Ergonomie** et facilité d'usage
* **Cohérence** des wireframes
* **Responsive design** pris en compte
* **Accessibilité** intégrée

### **5.3 Modélisation des Données**

* **Cohérence** du modèle
* **Normalisation** appropriée
* **Optimisation** anticipée

### **5.4 Documentation Technique**

* **Clarté** des diagrammes/wireframes
* **Exhaustivité** des spécifications
* **Professionnalisme** de la présentation
* **Qualité** de la communication

### **5.5 Ce qui est Évalué**

#### **5.5.1 Compétences Valorisées**

✅ **Conception technique** : Architecturer une solution robuste et évolutive\n✅ **Modélisation** : Concevoir des structures de données cohérentes\n✅ **UX/UI Design** : Créer des interfaces utilisateur intuitives\n✅ **Communication technique** : Documenter clairement ses choix\n✅ **Esprit critique** : Justifier et argumenter ses choix techniques\n✅ **Pragmatisme** : Proposer des solutions réalistes et réalisables

#### **5.5.2 Ce qui N'est PAS Évalué**

❌ **Connaissance d'un framework spécifique** : Pas de technologie imposée\n❌ **Expérience d'un langage particulier** : Choix libre de la stack\n❌ **Capacité à coder rapidement** : Pas de développement attendu\n❌ **Compétences graphiques** : Wireframes fonctionnels suffisants

### **5.6 Conseils pour Réussir**

#### **5.6.1 Stratégie Recommandée**


1. **Choisir** votre approche prioritaire (Backend OU Frontend)
2. **Analyser** le cahier des charges pour identifier les contraintes
3. **Concevoir** une solution claire et cohérente
4. **Modéliser** les données avec soin (obligatoire)
5. **Documenter** clairement chaque choix
6. **Compléter** par l'autre approche si le temps le permet

#### **5.6.2 Pièges à Éviter**

⚠️ **Vouloir tout faire** : Mieux vaut une partie excellente que tout en surface\n⚠️ **Sur-complexité** : Éviter les solutions trop sophistiquées\n⚠️ **Manque de justification** : Toujours expliquer ses choix techniques\n⚠️ **Architecture incohérente** : Vérifier la cohérence globale\n⚠️ **Modèle de données défaillant** : Soigner la modélisation\n⚠️ **Documentation pauvre** : Privilégier la clarté et les schémas


---

## **CONCLUSION**

Ce test technique vise à évaluer votre capacité à concevoir une solution technique complète, que ce soit côté architecture système ou interface utilisateur. L'accent est mis sur la **qualité de la conception**, la **pertinence des choix techniques** et la **clarté de la documentation**.

**Rappel important** : Privilégiez la qualité à la quantité. 

**Bonne chance !**