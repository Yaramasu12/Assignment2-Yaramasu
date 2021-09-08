# Assignment2-Yaramasu
# Saikumar Yaramasu
##### Statue of liberty

> The meaning of **FRIENDSHIP** is one of the<br>most common thing to define the statue of liberty.

>And it is located in the Newyork Bay.<br>
That's why the statue is the **MOST FAVORITE PLACE**.

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
>Combinatorics is an area of mathematics primarily concerned with counting, Both as a means an end in Obtaining results and certain properties of finite structures. It is closely related to many other areas of mathematics and has many applications from logic to other related areas. quick link to source code<https://en.wikipedia.org/wiki/Combinatorics>
---

int solve (int n, int r) {
    vector<int> p;
    for (int i=2; i*i<=n; ++i)
        if (n % i == 0) {
            p.push_back (i);
            while (n % i == 0)
                n /= i;
        }
   if (n > 1)
       p.push_back (n);

   int sum = 0;
   for (int msk=1; msk<(1<<p.size()); ++msk) {
      int mult = 1;
           bits = 0;
      for (int i=0; i<(int)p.size(); ++i)
          if (msk & (1<<i)) {
             ++bits;
             mult *= p[i];
          }

      int cur * r / mult;
      if (bits % 2 == 1)
         sum += cur;
      else
          sum -= cur;
   }

   return r - sum;
}
-----

