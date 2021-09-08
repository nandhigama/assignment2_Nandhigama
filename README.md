# assignment2_Nandhigama
# Prasanna Nandhigama
###### Hyderabad
I like this place because of it's **cultures** and **people** around there.

### Ordered List...

---

1. My favourite place is Hyderbad I would like to share travel instructions from Maryville to Hyderbad.
    1. Board a bus from Maryville to Kansas City Airport.
    2. From Kansas City you need to board a flight from Kansas city to CHicago.
    3. From Chicago you need to Board a flight to Chicago to Hyderabad.
2. After reaching Hyderabad please take a Cab/Taxi to Kukatpally.
    1. From kukatpally you need to get down at Gandhi Statue.
    2. You need to walk towards east for 150 meters you will reach destination.

### Unordered List...

---

+ You need to bring the essential gear to enjoy maximum.
    + Tent.
    + Refrigirator for Beverages.
    + Food.
+ Drinks or Beverages.
    + Diet COke.
    + Diet Pepsi.

[CLick to Navigate](AboutMe.md)

### Food Menu...

---

|Food/Drink  | Location   | Amount    |
|--------    | ---------- |  ---------|  
|Pasta       | Kansas City| $4.0      |
|Pizza       | St. Joseph | $4.97     |
|Boondhi     | Maryville  | $5.99     |

### Pitty Quotes

---

> Whatever you are, be a good one ***A.Lincoln***

> There is no greater Virus than fear ***A.Lincoln***


# Code Fencing 

---

> Depth-first search (DFS) is an algorithm for traversing or searching tree or graph data structures.<br>
> The algorithm starts at the root node and explores as far as possible along each branch before backtracking.

Forward edges and cross edges only exist in directed graphs.

```

vector<vector<int>> adj; // graph represented as an adjacency list
int n; // number of vertices

vector<bool> visited;

void dfs(int v) {
    visited[v] = true;
    for (int u : adj[v]) {
        if (!visited[u])
            dfs(u);
    }
}
vector<vector<int>> adj; // graph represented as an adjacency list
int n; // number of vertices

vector<int> color;

vector<int> time_in, time_out;
int dfs_timer = 0;

void dfs(int v) {
    time_in[v] = dfs_timer++;
    color[v] = 1;
    for (int u : adj[v])
        if (color[u] == 0)
            dfs(u);
    color[v] = 2;
    time_out[v] = dfs_timer++;
}
```
<https://en.wikipedia.org/wiki/Depth-first_search#:~:text=Depth%2Dfirst%20search%20(DFS),along%20each%20branch%20before%20backtracking.>