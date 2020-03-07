---
title: "Linked list"
date: "2020-03-02T22:12:03.284Z"
template: "post"
draft: false
slug: "linked-list"
category: "Data Structure"
tags:
  - "linked list"
  - "algorithm"
description: "자료구조 - 링크드 리스트에 대해 알아보자."
socialImage: "#"
---

## 

![linked list (출처: wikipedia)](/media/linkedlist.png)

+ 우리가 배열이라고 하는 기본적인 자료구조(선형 리스트)는 메모리를 연속적으로 할당받는다. 따라서 중간에 값을 삭제하는 경우 값들의 자리교체가 필요해지므로 많은 오버헤드가 발생한다.   
+ 연결리스트는 분산된 메모리속에서 링크를 통해 다음 값을 알아내므로 중간 값이 삭제되는 경우 링크만 바꿔주면 된다는 장점이 있다.   
+ 연결 리스트를 알기전에 노드라는 것에 대해서 언급해야 하는데, 노드는 값 + 링크의 형태를 갖추고 있는 구조를 말한다. 링크는 포인터로 구현되어 다른 노드를 참조하는 값이다.   
+ 연결리스트의 3가지 형태   
    - 단순 연결 리스트 : 단순 연결 리스트는 헤더 노드가 존재하며 헤더 노드는 다음 노드를 그리고 다음 노드는 그 다음 노드를 가리킨다. 한 방향으로 연결되어 단순 연결 리스트라고 부른다.   
    - 원형 연결 리스트 : 원형 연결 리스트는 헤더 노드와 테일 노드가 존재하며 단순 연결 리스트와 구조상 동일하지만 테일 노드가 헤더 노드를 가리키고 있다는 것이 차이점이다.   
    - 이중 연결 리스트 : 이중 연결 리스트는 헤더 노드만 존재하며 각 노드는 다음 노드를 가리키는 링크를 가지는 동시에 이전 노드를 가리키는 링크를 가지고 있다.      
+ 파이썬에서 노드 구현   
```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
```   



