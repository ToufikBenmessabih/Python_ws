# Python_ws: Calcul du Temps et de la Vitesse à une Distance Donnée

## Étapes

1. **Calcul de la distance cumulative**  
   - Utilisation de `cumulative_trapezoid` pour intégrer la vitesse (`speed`) par rapport au temps (`time`) via la règle du trapèze.  
   - `initial=0` initialise la distance à 0.

2. **Création des fonctions d'interpolation**  
   - `interp1d` estime :
     - **`distance_interp`** : le temps pour une distance donnée.  
     - **`speed_interp`** : la vitesse pour une distance donnée.  
   - `fill_value="extrapolate"` permet l'estimation hors des bornes initiales.

3. **Calcul à 31 mètres**  
   - `distance_interp(31)` : estime le **temps**.  
   - `speed_interp(31)` : estime la **vitesse**.

## Résultats  
Obtenez temps et vitesse pour toute distance spécifiée (ex. : 31 mètres).
