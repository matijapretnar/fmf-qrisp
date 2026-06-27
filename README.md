# Visokonivojsko kvantno programiranje

Gradivo za sklop o **visokonivojskem kvantnem programiranju** v jeziku
[Qrisp](https://www.qrisp.eu). Namenjen je dijakom in obsega **štiri
šolske ure**, razdeljene na dva dneva.

Delavnica je del delavnice o kvantnem računalništvu na [poletni šoli
FRI](https://www.fri.uni-lj.si/sl/poletna-sola-fri), kjer udeleženci
drugje spoznajo še ZX-račun, osnove klasičnih algoritmov in Qiskit. Tu
to znanje nadgradimo z mislijo, da kvantnih programov ni treba pisati
le s sestavljanjem vrat (nizkonivojsko, kot v Qiskitu), ampak tudi
prek spremenljivk, tipov in funkcij (visokonivojsko, kot v Qrispu).

Celotno gradivo je v zvezku [index.ipynb](index.ipynb).

## Vsebina

### 1. dan: Uvod v Qrisp

Spoznamo Qrisp in njegove gradnike ter se srečamo s problemom, ki ga bo naslednji
dan rešil naš prvi kvantni algoritem.

- **Kvantne spremenljivke**
  ([`QuantumVariable`](https://www.qrisp.eu/reference/Core/QuantumVariable.html)) -
  ustvarjanje spremenljivk in registrov, dostop do posameznih kubitov, osnovna
  kvantna vrata (`x`, `h`, `cx`) ter izpis vezja in stanja. Naloga: priprava stanja
  GHZ.
- **Kvantni tipi**
  ([`QuantumFloat`](https://www.qrisp.eu/reference/Quantum%20Types/QuantumFloat.html),
  [`QuantumBool`](https://www.qrisp.eu/reference/Quantum%20Types/QuantumBool.html)) -
  predznačena in decimalna števila, računske operacije nad njimi ter logične
  operacije in primerjave, vse v superpoziciji. Naloge: lastni računi s floati.
- **Motivacija - Deutsch–Jozsev problem** - prek igrice »je niz konstanten ali
  uravnotežen?« pokažemo, zakaj klasično potrebujemo več vprašanj, kvantno pa bo
  dovolj eno samo.

### 2. dan: Kvantni algoritmi

Izpolnimo včerajšnjo obljubo in zgradimo prva kvantna algoritma.

- **Klasična rešitev** Deutsch–Jozse v Pythonu - namesto nizov uporabimo funkcije in
  štejemo, kolikokrat jih moramo poklicati.
- **Kvantni Deutsch–Jozsa** - korak za korakom od naivnega preverjanja prek
  **superpozicije** vseh vhodov, **vračanja faze** (phase kickback) in
  **interference** do rešitve z eno samo uporabo funkcije.
- **Groverjev algoritem** - iskanje v neurejeni množici v približno √M korakih, z
  interaktivno animacijo amplitud (orakelj in zrcaljenje prek povprečja) ter polno
  implementacijo.
- **Bločno kodiranje** *(napredni dodatek, odvisno od časa)* - pogled naprej k
  sodobnejšim tehnikam, pri katerih kvantni register zakodira tudi neunitarne
  operacije.

## Zagon

Zvezek lahko brez nameščanja odpreš kar v brskalniku prek storitve Binder
(prvi zagon traja nekaj minut, da se okolje zgradi):

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/matijapretnar/fmf-qrisp/main?labpath=index.ipynb)

Binder okolje zgradi iz [environment.yml](environment.yml), tako da je Qrisp že
nameščen.

### Lokalni zagon

Ustvari okolje iz [environment.yml](environment.yml):

```sh
conda env create -f environment.yml
conda activate qrisp-env
```

in zaženi JupyterLab (če ga v okolju še ni: `pip install jupyterlab`):

```sh
jupyter lab index.ipynb
```

Zvezek je zasnovan za zaporedno izvajanje od vrha navzdol; celice z `...` so
namenoma nedokončane in jih udeleženci dopolnijo sami.
