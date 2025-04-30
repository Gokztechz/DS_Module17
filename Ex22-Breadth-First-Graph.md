# Ex22 Breadth First Graph
## DATE:15.04.25
## AIM:
To write a printQueue C function of the given graph that is to be traversed in the breadth first manner.

![image](https://github.com/user-attachments/assets/f483f48c-6af0-4027-a993-01c108a50933)


## Algorithm
1. Start the program.
2. Start from the front index of the queue.
3. If the queue is empty, print "Queue is empty".
4. Otherwise, print "Queue contains" and display all items from front to rear.
5. Return after printing the queue contents.
6. End the program.


## Program:
```
/*
Program to traverse graph using BFS
Developed by: GOKUL SHARAN R
RegisterNumber: 212223040052
*/
```
```
#include <stdio.h>
#include <stdlib.h>

#define SIZE 40

struct queue {
    int items[SIZE];
    int front;
    int rear;
};

struct queue* createQueue();
void enqueue(struct queue* q, int);
int dequeue(struct queue* q);
void display(struct queue* q);
int isEmpty(struct queue* q);
void printQueue(struct queue* q);

struct node {
    int vertex;
    struct node* next;
};

struct node* createNode(int);

struct Graph {
    int numVertices;
    struct node** adjLists;
    int* visited;
};

void printQueue(struct queue* q) {
    int i = q->front;
    if (isEmpty(q)) {
        printf("Queue is empty");
    } else {
        printf("Queue contains ");
        for (i = q->front; i <= q->rear; i++) {
            printf("%d", q->items[i]);
        }
    }
}
```

## Output:
![image](https://github.com/user-attachments/assets/8b2f32fd-7876-492d-ae1b-fca4bcb5a782)




## Result:
Thus, the code for the printQueue function of the following graph that is to be traversed in the breadth first manner is implemented successfully.
