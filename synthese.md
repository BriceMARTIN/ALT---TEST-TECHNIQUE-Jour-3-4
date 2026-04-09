# Synthèse

## **1. EXECUTIVE SUMMARY**

### **Vision produit**

Plateforme de gamification pour transformer l'expérience citoyenne des démarches administratives françaises en parcours motivant et ludique, réduisant l'abandon et augmentant l'engagement.

### **3 Objectifs business principaux**


1. **Réduire l'abandon** : Passer de 40% à 15% d'abandon sur les démarches complexes
2. **Améliorer l'engagement** : Créer une communauté active de citoyens motivés
3. **Moderniser l'administration** : Proposer une nouvelle approche digitale des services publics

### **Proposition de valeur**

* **Pour les citoyens** : Transformer l'obligation administrative en expérience gratifiante
* **Pour l'administration** : Réduire la charge support et améliorer la satisfaction
* **Pour l'État** : Moderniser l'image des services publics


---

## **2. TOP 10 QUESTIONS CRITIQUES**

| **Question** | **Impact** | **Justification** |
|----------|--------|---------------|
| **1. Intégration FranceConnect : niveau d'API disponible ?** | 🔴 Bloquant | Authentification unique critique pour l'adoption |
| **2. Données RGPD : quelles données personnelles collectées ?** | 🔴 Bloquant | Conformité légale obligatoire |
| **3. Hébergement : contraintes de souveraineté numérique ?** | 🔴 Bloquant | Données sensibles = territoire français |
| **4. API gouvernementales : disponibilité et documentation ?** | 🟡 Important | Faisabilité technique des intégrations |
| **5. Accessibilité : niveau WCAG requis ?** | 🟡 Important | Conformité service public |
| **6. Quêtes de groupe : mécanisme de partage de données ?** | 🟡 Important | Complexité technique familiale |
| **7. BureauBot : limite de l'IA dans les conseils légaux ?** | 🟡 Important | Risque juridique et responsabilité |
| **8. Monétisation : modèle économique à long terme ?** | 🟡 Important | Viabilité business |
| **9. Notifications push : canaux autorisés ?** | 🟢 Nice-to-have | Expérience utilisateur |
| **10. Thème sombre : priorité d'implémentation ?** | 🟢 Nice-to-have | Confort utilisateur |


---

## **3. ANALYSE MVP**

### **5 Fonctionnalités Core pour MVP**

#### **3.1 Matrice Effort/Valeur**

| **Fonctionnalité** | **Effort** | **Valeur** | **Priorité** |
|----------------|--------|--------|----------|
| **Authentification FranceConnect** | 3      | 5      | P0       |
| **Système de quêtes (3 démarches)** | 4      | 5      | P0       |
| **Gamification (XP, niveaux, badges)** | 3      | 4      | P0       |
| **BureauBot assistant basique** | 4      | 4      | P1       |
| **Sauvegarde auto formulaires** | 2      | 3      | P1       |

#### **3.2 Démarches MVP (3 quêtes prioritaires)**


1. **Demande de passeport** (priorité absolue suite aux retours)
2. **Déclaration d'impôts** (fort impact citoyen)
3. **Changement d'adresse** (cas d'usage fréquent)

#### **3.3 Timeline proposée (3 sprints)**

* **Sprint 1 (4 sem)** : Auth + Architecture + Quête passeport
* **Sprint 2 (4 sem)** : Gamification + BureauBot v1 + Quête impôts
* **Sprint 3 (4 sem)** : Sauvegarde auto + Quête adresse + Polish

#### **3.4 Features reportées en V2**

* **Quêtes de groupe** : Complexité juridique élevée
* **API ouverte** : Nécessite une base utilisateur stable
* **Mode famille** : Gestion des droits complexe


---

## **4. RISQUES MAJEURS & MITIGATION**

### **4.1 Risques techniques**

* **🔴 Complexité APIs gouvernementales**
  * *Mitigation* : POC sur API ANTS dès le sprint 1
  * *Fallback* : Saisie manuelle avec validation a posteriori

### **4.2 Risques légaux**

* **🟡 Conformité RGPD et données sensibles**
  * *Mitigation* : Audit DPO externe dès la conception
  * *Anonymisation* : Chiffrement AES-256 des données PII

### **4.3 Risques business**

* **🟡 Adoption utilisateur incertaine**
  * *Mitigation* : Beta test avec 100 utilisateurs volontaires
  * *Métriques* : Engagement J+7 > 40%


---

## **5. APPROCHE RECOMMANDÉE**

### **5.1 Méthodologie suggérée**

* **Lean Startup** : Build-Measure-Learn avec cycles courts
* **Design Thinking** : Co-conception avec citoyens beta-testeurs
* **DevOps** : Déploiement continu avec monitoring proactif

### **5.2 Équipe minimale requise**

* **1 Lead Dev Full-stack** (Node.js/React)
* **1 Dev Backend** (APIs + sécurité)
* **1 Designer UX/UI** (accessibilité)
* **1 Product Owner** (métier administratif)

### **5.3 3 Quick wins identifiés**


1. **Prototype gamification** sur démarche existante (2 sem)
2. **Integration FranceConnect** en bac à sable (1 sem)
3. **Thème sombre** pour différenciation immédiate (3 jours)

### **5.4 Next steps concrets**


1. **Workshop clarification** avec parties prenantes (J+2)
2. **Audit APIs disponibles** ANTS, DGFIP, API Particulier (J+7)
3. **Architecture technique** détaillée (J+14)


---

## **6. ARCHITECTURE HIGH-LEVEL**

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Frontend      │    │   Backend       │    │   Services      │
│   React/PWA     │◄──►│   Node.js/API   │◄──►│   Externes      │
│   - Gamification│    │   - Auth JWT    │    │   - FranceConnect│
│   - BureauBot   │    │   - Quêtes      │    │   - ANTS        │
│   - Thème sombre│    │   - Notification│    │   - DGFIP       │
└─────────────────┘    └─────────────────┘    └─────────────────┘
                                │
                       ┌─────────────────┐
                       │   Database      │
                       │   PostgreSQL    │
                       │   - Chiffrement │
                       │   - Backup      │
                       └─────────────────┘
```


---

## **7. ADAPTATION AUX IMPRÉVUS**

### **7.1 Contraintes identifiées**

* **Hébergement français** → OVH/Scaleway/Outscale
* **Accessibilité WCAG 2.1 AA** → Impact sur choix frameworks
* **Sécurité ANSSI** → Chiffrement BDD + audit documentation
* **Mobile native** → Recommandation PWA first, native V2

### **7.2 Impacts sur planning**

* **+20% effort** pour contraintes accessibilité
* **+15% effort** pour sécurité renforcée
* **+2 sprints** si mobile native immédiat

### **7.3 Solutions techniques**

* **Sauvegarde auto** : LocalStorage + API intervals 30sec
* **Notifications push** : Web Push API + Service Workers
* **Thème sombre** : CSS Variables + prefers-color-scheme


---

## **8. MÉTRIQUES DE SUCCÈS**

### **8.1 Techniques**

* **Performance** : Temps de chargement < 3s
* **Disponibilité** : Uptime > 99.5%
* **Sécurité** : 0 incident données

### **8.2 Fonctionnelles**

* **Adoption** : 1000 utilisateurs actifs en 3 mois
* **Engagement** : 60% complétion des quêtes commencées
* **Satisfaction** : NPS > 50

### **8.3 Business**

* **Réduction abandon** : -25% sur démarches pilotes
* **Support** : -30% tickets support administration
* **Évolutivité** : Architecture prête pour 10K utilisateurs