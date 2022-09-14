# CPP-STL
Cheat sheet for C++ STL

## Pair
```
pair<int, int> p1, p2, p3, p4(1, 2), p5(p4);
p1.first = 10;
p1.second = 20;
p2 = make_pair(30, 40);
p3 = {50, 60};
//
```

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
vector<int>::iterator it1 = v.begin();
vector<int>::iterator it2 = v.end();
vector<int>::iterator it3 = v.rbegin();
vector<int>::iterator it4 = v.rend();
vector<int>::iterator it5 = v.cbegin();
vector<int>::iterator it6 = v.cend();
vector<int>::iterator it7 = v.crbegin();
vector<int>::iterator it8 = v.crend();
vector<int> v1(x, y); //creates a vector of size x of which each element is y
vector<int> v2 = {1, 2, 3};
vector<int> v3 = {10, 20, 30};
v3.insert(v3.begin(), v2.begin(), v2.end()); //v3 is now {1, 2, 3, 10, 20, 30};
vector<int> v4(v3.begin() , v3.begin()+3); // v4 is now {1, 2, 3}
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
stack<int> s;

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

