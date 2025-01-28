Binary Search Tree (BST) aşamalarını adım adım oluşturalım. Root olarak ilk eleman olan 7'yi alacağız.

Root: 7

5 < 7, sola yerleşir:


    7
   /
  5
1 < 7 ve 1 < 5, sola yerleşir:

    7
   /
  5
 /
1
8 > 7, sağa yerleşir:

    7
   / \
  5   8
 /
1
3 < 7, 3 < 5, 3 > 1, 1'in sağına yerleşir:

    7
   / \
  5   8
 /
1
 \
  3
6 < 7, 6 > 5, 5'in sağına yerleşir:

    7
   / \
  5   8
 / \
1   6
 \
  3
0 < 7, 0 < 5, 0 < 1, 1'in soluna yerleşir:

    7
   / \
  5   8
 / \
1   6
/ \
0   3
9 > 7, 9 > 8, 8'in sağına yerleşir:

    7
   / \
  5   8
 / \   \
1   6   9
/ \
0   3
4 < 7, 4 < 5, 4 > 1, 4 > 3, 3'ün sağına yerleşir:

    7
   / \
  5   8
 / \   \
1   6   9
/ \
0   3
     \
      4
2 < 7, 2 < 5, 2 > 1, 2 < 3, 3'ün soluna yerleşir:

    7
   / \
  5   8
 / \   \
1   6   9
/ \
0   3
   / \
  2   4
Final BST yapısı yukarıdaki gibidir. Bu BST'de:

Root: 7
Sol alt ağaç: 5,1,6,0,3,2,4 (7'den küçük değerler)
Sağ alt ağaç: 8,9 (7'den büyük değerler)
