# [USACO15JAN] Moovie Mooving G

## 题目描述

Bessie is out at the movies.  Being mischievous as always, she has decided to hide from Farmer John for L (1 <= L <= 100,000,000) minutes, during which time she wants to watch movies continuously. She has N (1 <= N <= 20) movies to choose from, each of which has a certain duration and a set of showtimes during the day.  Bessie may enter and exit a movie at any time during one if its showtimes, but she does not want to ever visit the same movie twice, and she cannot switch to another showtime of the same movie that overlaps the current showtime.

Help Bessie by determining if it is possible for her to achieve her goal of watching movies continuously from time 0 through time L.  If it is, determine the minimum number of movies she needs to see to achieve this goal (Bessie gets confused with plot lines if she watches too many movies).

奶牛贝西想连续看 $L$（$1 \le L \le 10^8$）分钟的电影，有 $N$（$1 \le N \le 20$）部电影可供选择，每部电影会在一天的不同时段放映。


贝西可以在一部电影播放过程中的任何时间进入或退出放映厅。但她不愿意重复看到一部电影，所以每部电影她最多看到一次。她也不能在看一部电影的过程中，换到另一个正在播放相同电影的放映厅。


请帮贝西计算她能够做到从 $0$ 到 $L$ 分钟连续不断地观看电影，如果能，请计算她最少看几部电影就行了。

## 输入格式

INPUT: (file movie.in) 

The first line of input contains N and L.

The next N lines each describe a movie.  They begin with its integer duration, D (1 <= D <= L) and the number of showtimes, C (1 <= C <= 1000).  The remaining C integers on the same line are each in the range 0..L, and give the starting time of one of the showings of the movie.  Showtimes are distinct, in the range 0..L, and given in increasing order.

## 输出格式

UTPUT: (file movie.out) 

A single integer indicating the minimum number of movies that Bessie

needs to see to achieve her goal.  If this is impossible output -1

instead.

## 样例 #1

### 样例输入 #1

```
4 100 
50 3 15 30 55 
40 2 0 65 
30 2 20 90 
20 1 0
```

### 样例输出 #1

```
3
```

## 提示 
SOLUTION NOTES:

Bessie should attend the first showing of the fourth movie from time 0

to time 20.  Then she watches the first showing of the first movie

from time 20 to time 65.  Finally she watches the last showing of the

second movie from time 65 to time 100.