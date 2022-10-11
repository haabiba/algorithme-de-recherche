 recherche binaire:la recherche par intervalles divise 
la recherche en deux en ciblant à plusieurs reprises le centre de l'ensemble de données
Algorithme de recherche binaire : les étapes de base pour effectuer une recherche binaire sont :

Commencez par l'élément médian de l'ensemble du tableau comme clé de recherche.
Si la valeur de la clé de recherche est égale à l'élément, renvoie un index de la clé de recherche.
Ou si la valeur de la clé de recherche est inférieure à l'élément au milieu de l'intervalle, réduisez l'intervalle à la moitié inférieure.
Sinon, réduisez-le à la moitié supérieure.
Vérifiez à plusieurs reprises à partir du deuxième point jusqu'à ce que la valeur soit trouvée ou que l'intervalle soit vide.
L'algorithme de recherche binaire peut être implémenté des deux manières suivantes

#Méthode itérative

binarySearch(arr, x, low, high)
        repeat till low = high
               mid = (low + high)/2
                   if (x == arr[mid])
                   return mid
   
                   else if (x > arr[mid]) // x is on the right side
                       low = mid + 1
   
                   else                  // x is on the left side
                       high = mid - 1
Méthode récursive
Time Complexity: O(log n)
Auxiliary Space: O(1)
