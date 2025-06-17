# Qrisp delavnica

## Načrt

### 1. ura

- zgodovina prehoda klasičnega računalništva od pretikanja kablov do danes, vzporednice s trenutnim stanjem kvantnih računalnikov
- odprejo online Jupyter z nameščenim Qrispom in poženejo testni primer
- osnovni koraki v Qrispu, zapis vezij prek spremenljivk in funkcij, meritve, …
- Qrisp preizkusijo na vezjih, ki so jih do sedaj videli na šoli ter to primerjajo s pisanjem/risanjem v Qiskitu

### 2. ura

- prikaz dodatnih kvantnih tipov (QuantumBool, QuantumInt, QuantumFloat, …), operacij na njih, ter izračunanih vezij
- v Qrispu pišejo svoje račune in kratke programe ter gledajo, kakšna vezja dobijo
- pisanje kvantnih funkcij in samodejno dodajanje ancile, razračunanja, preklapljanje med implementacijami seštevalnikov, …
- pišejo svoje funkcije, simulirajo rezultate, in opazujejo ustvarjena vezja
- skupaj napišemo svoj lastni kvantni tip, npr. vržemo dve kvantni kocki in dobimo superpozicijo možnih vsot, pri obratu faze pa se nekateri izničijo

### 3. ura

- motivacija Deutsch-Joszevega problema prek igrice, kjer poskušajo s čim manj vprašanji ugotoviti, kakšne vrste število sem si izmislil
- dopolnijo predlogo klasično rešitve v Pythonu ter v njej preizkušajo različne funkcije (konstantno, levi-desni biti, sodi-lihi biti, …)
- prepis klasične rešitve v Qrisp in preizkus z različnimi funkcijami (tu in po vsakem od naslednjih korakov do algoritma)
- skupaj pridemo do tega, da bi računali s superpozicijami, zato vhodne kubite pripravimo s Hadamardom

### 4. ura

- spomnimo se, da je s ponovno uporabo Hadamarda treba povrniti vhodne kubite
- skupaj pridemo do tega, da želimo vrednosti izničiti, zato izhodni kubit pripravimo s Hadamardom
- kaj so naslednji koraki v programiranju (Bernstein-Vazirani, QPE, Grover, Shor, kvantne simulacije, …)
