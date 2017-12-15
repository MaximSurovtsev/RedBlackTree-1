[![Build Status](https://travis-ci.org/BinaryTreesImplementation/RedBlackTree.svg?branch=master)](https://travis-ci.org/BinaryTreesImplementation/RedBlackTree) 

# Red black tree
---
## Краткое описание
Red-black-tree — это самобалансирующееся бинарное дерево поиска, гарантирующее логарифмический рост высоты дерева от числа узлов и быстрое выполнение основных операций дерева поиска: добавление, удаление и поиск узла. Сбалансированность достигается за счёт введения дополнительного атрибута узла дерева — «цвета». Этот атрибут может принимать одно из двух возможных значений — «чёрный» или «красный».

## Реализация
Данное бинарное дерево поиска реализовано на языке программирования С++. 

Методы доступные для использования: 
+ **Insert**
+ **Delete**
+ **Search**

Время работы методов от времени описывается формулами:

+ balance - **O(log2(N)) || O(1)** 
+ Search - **O(log2(N))**
+ Insert - **O(log2(N))**
+ Delete - **O(log2(N))**

## Сравнение с AVL-tree

### Поиск
Поскольку красно-чёрное дерево, в худшем случае, выше, поиск в нём медленнее, но проигрыш по времени не превышает 39 %.

### Вставка
Вставка требует до 2 поворотов в обоих видах деревьев. Однако из-за большей высоты красно-чёрного дерева вставка может занимать больше времени.

### Удаление
Удаление из красно-чёрного дерева требует до 3 поворотов, в АВЛ-дереве оно может потребовать большее число поворотов (до корня). Поэтому удаление из красно-чёрного дерева быстрее, чем из АВЛ-дерева. Тем не менее, тесты показывают, что АВЛ-деревья быстрее красно-чёрных во всех операциях. Но красно-чёрные деревья производительнее при больших объёмах памяти.

### Сбалансированность
Сбалансированность этих деревьев хуже, чем у AVL-tree, но работа по поддержанию сбалансированности в красно-чёрных деревьях обычно эффективнее. Для балансировки красно-чёрного дерева производится минимальная работа по сравнению с АВЛ-деревьями.
