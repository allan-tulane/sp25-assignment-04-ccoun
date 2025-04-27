# CMPS 2200 Assignment 5
## Answers

**Name:** Charlie Coun






- **1a.** For n elements in a d-ary heap, the maximum depth h of the heap is the length of the root to the deepest leaf. So, the number of nodes up to the depth h would be $d^{h+1}-1/{d-1}$, which would be $d^{h}$ for any large h. So the maximum depth for n nodes would be $d^{h} <= n$, giving a maximum depth h of $log{_d}{n}$.


- **1b.** For insert, in the worst case the new element may have to swap all the way up to the root node, so the work would be proportional to the depth, meaning insert work = $O(log{_d}{n})$. For delete, we need to compare the node with its d children to find the smallest, and in the worst case we have to go from root to a leaf. Each level requires O(d) work for $log{_d}{n}$ levels, so delete work = $O(d⋅log{_d}{n})$


- **1c.** For a d-ary heap, the work for delete-min would be $O(d|V|⋅log{_d}{|V|})$ since the heap size is O(|V|), and the work for insert would be $O(|E|⋅log{_d}{|V|})$. This means the total work would be $O((|V|⋅d+|E|)log{_d}{|V|})$, which can be simplified into $O(((|V|⋅d+|E|)log|V|)/log{d})$

- **1d.** First we substitue $|E| = |V|^{1+ϵ}$ into the total work we derived in 1c, giving $O(((|V|⋅d+|V|^{1+ϵ})log|V|)/log{d})$. We then substitute $d = |V|^{ϵ}$ back into the runtime equation, giving us $O(((|V|^{1+ϵ}+|V|^{1+ϵ})log|V|)/log|V|^{ϵ})$, which simplifies down to $O(|V|^{1+ϵ}) = O(|E|). So to achieve a running time of O(|E|), the optimal choice is $d = O(|V|^{ϵ})$.


- **2a.**


- **2b.**


- **2c.**

- **2d.**

- **2e.**



- **3a.**


- **3b.**


- **3c.**
