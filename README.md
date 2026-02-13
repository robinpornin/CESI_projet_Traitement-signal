# Projet Traitement du Signal - Simulation d'une transmission de signaux discrète

## 🎯 Contexte

Dans un scénario fictif, un agent captif ne dispose que d’un microphone connecté au réseau de communication de la base.  
L’objectif est de transmettre un message de manière **discrète**, en utilisant uniquement des **ultrasons**, afin d’éviter toute détection.

Nous avons donc conçu un **POC (Proof of Concept)** capable de reconstituer entièrement une chaîne de transmission numérique, de l’entrée texte jusqu’à la reconstruction finale du message.

---

## 🧠 Objectif du projet

Implémenter en Python une chaîne complète de transmission comprenant :

- Conversion ASCII
- Encodage numérique (NRZ, Miller, Manchester)
- Modulation (FSK / FM)
- Transmission simulée
- Démodulation
- Décodage
- Reconstruction du message

Le système doit fonctionner pour :

- Texte court
- Texte volumineux
- Fichier binaire
- Signal audio

---

## 🏗️ Chaîne de transmission

### Texte court

1. Conversion ASCII  
2. Encodage NRZ  
3. Modulation FSK  
4. Transmission  
5. Démodulation FSK  
6. Décodage NRZ  
7. Conversion ASCII  

---

### Texte long / Fichier binaire

1. Conversion ASCII  
2. Encodage Miller  
3. Modulation FSK  
4. Transmission  
5. Démodulation  
6. Décodage Miller  
7. Reconstruction  

---

### Transmission audio

1. Encodage Manchester  
2. Modulation FM  
3. Transmission  
4. Démodulation FM  
5. Décodage  

---

## 🔬 Paramètres techniques

- Fréquences FSK :  
  - f0 = 18 kHz  
  - f1 = 22 kHz  

- Fréquence d’échantillonnage : 44.1 kHz  
- Bande passante approximative : 26 kHz  

La modulation FSK est choisie pour sa robustesse au bruit et sa simplicité d’implémentation.

---

## 🛠️ Technologies utilisées

- Python
- NumPy
- SciPy
- Matplotlib

#


