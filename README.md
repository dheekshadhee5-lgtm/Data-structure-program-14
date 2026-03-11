# Data-structure-program-14
#include<stdio.h>
#include<stdlib.h>
Struct Node{
 Int ticket;
 Struct Node *next;
};
Struct Node *front=NULL;
Struct Node *rear=NULL;
Void enqueue(int num){
 Struct Node 
*newNode=(struct 
Node*)malloc(sizeof(struct 
Node));
 newNode->ticket=num;
 newNode->next=NULL;
 if(rear==NULL){
 front=rear=newNode;
 }
 Else{
 Rear->next=newNode;
 Rear=newNode;
 }
}
Void dequeue(){
 If(front==NULL){
 Printf(“Queue is 
empty\n”);
 Return;
 }
 Struct Node *temp=front;
 Printf(“Serving ticket: 
%d\n”,temp->ticket);
 Front=front->next;
 If(front==NULL)
 Rear=NULL;
 Free(temp);
}
Void display(){
 Struct Node *temp=front;
 Printf(“Waiting Queue:\n”);
 While(temp!=NULL){
 Printf(“%d “,temp-
>ticket);
 Temp=temp->next;
 }
 Printf(“\n”);
>OUTPUT
Waiting Queue:
101 102 103
Serving ticket: 101
Waiting Queue:
102 103
