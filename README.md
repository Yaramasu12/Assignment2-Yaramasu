# Assignment2-Yaramasu
# Saikumar Yaramasu
##### Statue of liberty

> The meaning of **FRIENDSHIP** is one of the<br>most common thing to define the statue of liberty.

>And it is located in the Newyork Bay.<br>
That's why the statue is the **MOST FAVORITE PLACE**.

-----
# Heading for access to reach the place with order list and unordered list
1. Go to then St.Louis Lambert international Airport.
2. To go to John F. Kennedy international Airport.
   1. Newark Harbour
   2. Liberty Island
3. Statue of Liberty National Monument.
 * Ellis Island
 * Brooklyn Bridge
   * City Tour Hub
   * Rockefeller Center
**[LinktoAboutme.md](Aboutme.md)**

------
# Heading for the  creating a Table foods and drinks

**Introduction:**
 The following is to create a table with atleast 4 food/drinks that you would recommend someone try. Include a short paragraph that introduces the table.

|Mandatory   |fav1            |fav2             |fav3             |fav4            |
|:--------:  |:---------:     |:---------:      |:----------:     |:----------:    |
|Food        |Mandi           |Dosa             |Ladies Finger    |Coke            |
|Location    |Hyderabad       |Ongole           |Home             |Any             |
|Amount      |800             |80               |30               |100             |

-----
# Section of Quotes
>"Many of life’s failures are people who did not realize how close they were to success when they gave up."
>**Author:** *Thomas A. Edison*<br>
>“If you want to live a happy life, tie it to a goal, not to people or things.”
>**Author:** *Albert Einstein*

-----
# New Section about Code Fencing
>A maximal matching can be found with a simple greedy algorithm. A maximum matching is also a maximal matching, and hence it is possible to find a largest maximal matching in polynomial time. However, no polynomial-time algorithm is known for finding a minimum maximal matching, that is, a maximal matching that contains the smallest possible number of edges. A maximal matching with k edges is an edge dominating set with k edges. Conversely, if we are given a minimum edge dominating set with k edges, we can construct a maximal matching with k edges in polynomial time. Therefore, the problem of finding a minimum maximal matching is essentially equal to the problem of finding a minimum edge dominating set. Both of these two optimization problems are known to be NP-hard; the decision versions of these problems are classical examples of NP-complete problems. Both problems can be approximated within factor 2 in polynomial time: simply find an arbitrary maximal matching M.Quick link to source code<https://en.wikipedia.org/wiki/Matching_(graph_theory)>
````
int n, k;
vector<vector<int>> g;
vector<int> mt;
vector<bool> used;

bool try_kuhn(int v) {
    if (used[v])
        return false;
    used[v] = true;
    for (int to : g[v]) {
        if (mt[to] == -1 || try_kuhn(mt[to])) {
            mt[to] = v;
            return true;
        }
    }
    return false;
}

int main() {
    //... reading the graph ...

    mt.assign(k, -1);
    for (int v = 0; v < n; ++v) {
        used.assign(n, false);
        try_kuhn(v);
    }

    for (int i = 0; i < k; ++i)
        if (mt[i] != -1)
            printf("%d %d\n", mt[i] + 1, i + 1);
}
````
quick link to source code <https://cp-algorithms.com/graph/kuhn_maximum_bipartite_matching.html>

