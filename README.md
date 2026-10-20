# Modelarea Atacurilor Cibernetice și Apărare Automată (NetLogo)
**Proiect la disciplina Bazele Ciberneticii Economice**

* **Student:** Chiper Alina Alice
* **Instituție:** Academia de Studii Economice din București (ASE)
* **Facultate:** Cibernetică, Statistică și Informatică Economică (CSIE)
* **Grupa:** 1014 | Seria D

---

## 📌 Descrierea Proiectului
Proiectul explorează aplicarea sistemelor multi-agent (MAS) și a învățării prin consolidare (Reinforcement Learning) în domeniul securității cibernetice, fiind structurat în două părți:
1. **Analiza Critică a Literaturii de Specialitate:** Studiul a două articole de cercetare (MDPI Sensors 2023 și Nature Scientific Reports 2026) axate pe Deep Q-Networks (DQN) și detecția anomaliilor în Cyber Range.
2. **Implementarea unui Model de Simulare:** Model bazat pe agenți dezvoltat în mediul **NetLogo** pentru a reproduce dinamica dintre un atacator adaptiv și un sistem defensiv automatizat pe o rețea de calculatoare.

---

## 💻 Arhitectura Modelului NetLogo
* **Noduri de Rețea (`nodes`):** Calculatoare/servere cu stări discrete (`susceptible`, `compromised`, `isolated`) și număr variabil de vulnerabilități.
* **Red Agent (Atacatorul):** Agent autonom ce exploatează nodurile vulnerabile folosind fie o strategie aleatorie, fie una țintită (`targeted`).
* **Blue Agent (Apărătorul):** Agent autonom ce patrulează rețeaua și izolează nodurile compromise pe baza unei raze de scanare și a unei probabilități de detecție.

---

## ⚙️ Parametrii Principali de Simulare
* `num-nodes`: Numărul total de noduri din rețea (default: 20)
* `attack-rate`: Probabilitatea de compromitere a unui nod la fiecare pas de timp
* `detection-rate`: Probabilitatea de izolare a unui nod compromis de către Blue Agent
* `network-topology`: Tipul conexiunilor din rețea (`random`, `scale-free`, `lattice`)
* `attack-strategy`: Modul de operare al atacatorului (`random` vs `targeted`)

---

## 📂 Structura Fișierelor
* `Proiect_BCE.pdf` — Documentația teoretică completă, sinteza articolelor și analiza critică
* `cybersecurity_model.nlogo` — Codul sursă NetLogo executabil pentru simulare
