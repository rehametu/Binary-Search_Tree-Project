# Binary-Search_Tree-Project
Patika.dev Binary Search Tree projesi


___[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

==> İlk değerimiz root değeri yani 7 dir.

|   | 7 |   |
|---|---|---|


==> 5, 7'den küçük olduğu için soluna yerleşir.



|   |   | 7 |   |   |
|---|---|---|---|---|
|   | / |   |   |   |
| 5 |   |   |   |   |

==> 1, 5'den küçük olduğu için soluna yerleşir.

|   |   |   |   | 7 |   |   |   |   |
|---|---|---|---|---|---|---|---|---|
|   |   |   | / |   |   |   |   |   |
|   |   | 5 |   |   |   |   |   |   |
|   | / |   |   |   |   |   |   |   |
| 1 |   |   |   |   |   |   |   |   |

==> 8, 7'den büyük olduğu için sağına yerleşir.

|   |   |   |   | 7 |   |   |   |   |
|---|---|---|---|---|---|---|---|---|
|   |   |   | / |   | \ |   |   |   |
|   |   | 5 |   |   |   | 8 |   |   |
|   | / |   |   |   |   |   |   |   |
| 1 |   |   |   |   |   |   |   |   |

==> 3, 7 ve 5'den küçük 1'den büyük olduğu için 1'in sağına yerleşir.


|   |   |   |   | 7 |   |   |   |   |
|---|---|---|---|---|---|---|---|---|
|   |   |   | / |   | \ |   |   |   |
|   |   | 5 |   |   |   | 8 |   |   |
|   | / |   |   |   |   |   |   |   |
| 1 |   |   |   |   |   |   |   |   |
|   | \ |   |   |   |   |   |   |   |
|   |   | 3 |   |   |   |   |   |   |

==> 6 7'den küçük 5'den büyük olduğu için 5'in sağına yerleşir.

|   |   |   |   | 7 |   |   |   |   |
|---|---|---|---|---|---|---|---|---|
|   |   |   | / |   | \ |   |   |   |
|   |   | 5 |   |   |   | 8 |   |   |
|   | / |   | \ |   |   |   |   |   |
| 1 |   |   |   | 6 |   |   |   |   |
|   | \ |   |   |   |   |   |   |   |
|   |   | 3 |   |   |   |   |   |   |

==> 0; 1, 5 ve 7'den küçük olduğu için 1'in soluna yerleşir.

|   |   |   |   |   |   | 7 |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   | / |   | \ |   |   |   |   |   |
|   |   |   |   | 5 |   |   |   | 8 |   |   |   |   |
|   |   |   | / |   | \ |   |   |   |   |   |   |   |
|   |   | 1 |   |   |   | 6 |   |   |   |   |   |   |
|   | / |   | \ |   |   |   |   |   |   |   |   |   |
| 0 |   |   |   | 3 |   |   |   |   |   |   |   |   |

==> 9, 7 ve 8'den büyük olduğu için 8'in sağına yerleşir.


|   |   |   |   |   |   | 7 |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   | / |   | \ |   |   |   |   |   |
|   |   |   |   | 5 |   |   |   | 8 |   |   |   |   |
|   |   |   | / |   | \ |   |   |   | \ |   |   |   |
|   |   | 1 |   |   |   | 6 |   |   |   | 9 |   |   |
|   | / |   | \ |   |   |   |   |   |   |   |   |   |
| 0 |   |   |   | 3 |   |   |   |   |   |   |   |   |

==> 4; 5 ve 7'den küçük , 1 ve 3'den büyük olduğu için 3'ün sağına yerleşir.


|   |   |   |   |   |   | 7 |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   | / |   | \ |   |   |   |   |   |
|   |   |   |   | 5 |   |   |   | 8 |   |   |   |   |
|   |   |   | / |   | \ |   |   |   | \ |   |   |   |
|   |   | 1 |   |   |   | 6 |   |   |   | 9 |   |   |
|   | / |   | \ |   |   |   |   |   |   |   |   |   |
| 0 |   |   |   | 3 |   |   |   |   |   |   |   |   |
|   |   |   |   |   | \ |   |   |   |   |   |   |   |
|   |   |   |   |   |   | 4 |   |   |   |   |   |   |

==> 2; 7,5,3'den küçük, 1'den büyük olduğu için 3'ün soluna yerleşir.


|   |   |   |   |   |   | 7 |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   | / |   | \ |   |   |   |   |   |
|   |   |   |   | 5 |   |   |   | 8 |   |   |   |   |
|   |   |   | / |   | \ |   |   |   | \ |   |   |   |
|   |   | 1 |   |   |   | 6 |   |   |   | 9 |   |   |
|   | / |   | \ |   |   |   |   |   |   |   |   |   |
| 0 |   |   |   | 3 |   |   |   |   |   |   |   |   |
|   |   |   | / |   | \ |   |   |   |   |   |   |   |
|   |   | 2 |   |   |   | 4 |   |   |   |   |   |   |














