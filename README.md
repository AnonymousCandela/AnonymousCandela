# Bonjour, je suis Durrice Léa Tahoc Wokam 👋

Étudiante au **baccalauréat en génie informatique** à l'Université du Québec en Outaouais (UQO).
Je m'intéresse à la **conception numérique sur FPGA**, aux **systèmes embarqués** et à l'**intégration matériel-logiciel**.

## 🔧 Compétences

| Domaine | Outils et technologies |
|---|---|
| Conception numérique | VHDL, machines à états, UART, Intel Quartus Prime, Cyclone V (DE1-SoC) |
| Vérification | Bancs d'essai VHDL, Questa / ModelSim |
| Embarqué | Arduino (C/C++), acquisition de capteurs, commande PWM, interruptions |
| Instrumentation | Calibration expérimentale, analyse statistique des mesures |
| Documentation | Rédaction technique, cohérence entre la documentation et l'implantation |

## 📌 Projet à la une

### [Surveillance d'un moteur CC — Arduino + FPGA](https://github.com/AnonymousCandela/surveillance-moteur-fpga)

Système embarqué temps réel qui classe l'état d'un moteur à courant continu en **NORMAL**, **DÉGRADÉ** ou **DÉFAUT** à partir de sa vitesse et de son courant.

- Chaîne FPGA complète en VHDL : réception UART, décodage et vérification de trame, classifieur à seuils, émission de l'état.
- Confirmation des changements d'état sur 3 mesures, mais défaut appliqué immédiatement pour des raisons de sécurité.
- Liaison UART à 115 200 bauds entre un Arduino Mega 2560 (5 V) et une DE1-SoC (3,3 V).

*Stage GEN5001 · UQO · Été 2026*

## 🌐 Langues

Français
