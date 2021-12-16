# CPP-STL
Cheat sheet for C++ STL


## Vector
```
#include <vector>
vector<int> v;
int n=10;
v.push_back(n);
v.pop_back();
v.sort(v.begin(), v.end());
v.size();
v.empty();
v.clear();
//creates a vector of size x of which each element is y
vector<int> v(x, y);

```
## List
```
#include <list>
list<int> l;
l.push_front(10);
l.pop_front();
l.push_back(20);
l.pop_back();
//No operator like [] for random access
l.size();
l.clear();
l.empty();
//merge splice unique

```

## Forward List
Introduced in C++11
Keeps track of next element only, like singly linked list

## Stack

## Queue
```
#include <queue>
//can be built on deque or list
queue<int> q;//uses deque by default
queue<int, list<int>> q2;//built on list
```
## Dequeue
```
#include <deque>
deque<int> q;
q.push_front(a); //no push
q.push_back(b);
q.pop_front();
q.pop_back();
q.size();
q[i];
q.insert();//insert in middle
q.erase();//erase in middle
q.at(i);
q.front;
q.empty();
q.back;
q.clear();
```

## Priority Queue
```
#include <queue>
//can be built on vector or deque
priority_queue<int> pq; //uses a vector by default
priority_queue<int, deque<int>> q; //built on deque

```
## Unordered Set

## Set

## Unordered Map

## Map

