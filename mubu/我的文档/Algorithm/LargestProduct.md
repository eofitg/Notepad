# LargestProduct

10
- 5 5
  - 2 3
    - 1 2
    - 2 1
  - 3 2
- 6 4
  - 2 2
  - 3 1

14
- 7-n1 + 7-n2
  - 3-n1 + 4-n2
    - 2 2
    - 3 1
  - 4n1 + 3n2
    - 1 2
    - 2 1
- 8-n1 + 6-n2
  - 3 + 3
    - 1 2
    - 2 1
  - 4 + 2
    - 1 1
    - 2 0

FIND
- find(0, n)
  - find(n/2, n-n/2)
    - find((n-n/2)/2, (n-n/2)-(n-n/2)/2))
    - find((n-n/2)/2+1, (n-n/2)-(n-n/2)/2-1)
  - find(n/2+1, n-n/2-1)
    - find((n-n/2-1)/2, (n-n/2-1)-(n-n/2-1)/2)
    - find((n-n/2-1)/2+1, (n-n/2-1)-(n-n/2-1)/2-1)

25
- 12 13
  - 6 7
    - 3 4
      - 2 2
      - 3 1
    - 4 3
  - 7 6
    - 3 3
    - 4 2
- 13 12
  - 6 6
    - 3 3
    - 4 2
  - 8 4
    - 2 2
    - 3 1

INIT
- bool exist[N] = false;
- stack<int> ans = empty;
- int a = n / 2, b = a + 1;
- find(a, n - a), find(b, n - b);

SEARCH
- void find (int n1, int n2)
- IF-ELSE
  - !exist[n1]
    - ans.push(n1);
    - exist[n1] = true;
  - exist[n1]
    - return;
- int a = n2 / 2, b = a + 1;
- find(a, n2 - a);
- exist[b] = true, find(b, n2 - b), exist[b] = false;

CHECK
-

---

[Algorithm/LargestProduct](https://mubu.com/app/edit/home/7YiU0aa_YvE)