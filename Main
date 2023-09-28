

Page

of 6
ZOOM
////
// Author: Serhiy Leonchyk
// Section: A
// Assignment: P1 Stack Class
//
// This Program creates a stack of nodes that contain integers values,
// there are also functions to add items to the top of the stack (push), remove
// items from the top of the stack (pop), return a copy of the top item in the
// stack (top) to be output to the console, to return the amount of items in
// the stack (getCount), and to return a boolean value of whether or not the stack
// is empty (isEmpty)
////
#include <iostream>
using namespace std;
class Node {
public:
Node(int num) {
data = num;
next = nullptr;
}
int data; // purposely public
Node* next;
}; // end of Node class
class Stack {
public:
Stack() {
head = nullptr;
}
~Stack() {
while (!isEmpty()) {
pop();
}
}
void push(int num) {
Node* tmpNode = new Node(num);
tmpNode->next = head;
head = tmpNode;
count += 1;
}
int pop() {
if (head != nullptr) {
count = count - 1;
Node* tempNode = head;
head = head->next;
return tempNode->data;
delete tempNode;
}
else {
return -999;
}
}
int top() {



if (head != nullptr) {
return head->data;
}
else
{
return -999;
}
}
bool isEmpty() {
if (head == nullptr) {
return true;
}
else
{
return false;
};
}
int getCount() {
return count;
}
private:
Node* head = nullptr;
int count = 0;
}; // end of Stack class
int main() {
Stack stack;
cout << "Before pushing \n" << boolalpha;
cout << "Stack size: " << stack.getCount() << endl;
cout << "Stack is " << (stack.isEmpty() == true ? "empty\n" : "not empty\n");
stack.push(1);
stack.push(2);
stack.push(3);
stack.push(4);
stack.push(5);
cout << "\nAfter pushing 1-5 \n";
cout << "Stack size: " << stack.getCount() << endl;
cout << "Stack is " << (stack.isEmpty() == true ? "empty\n" : "not empty\n");
cout << "Top of the stack is: " << stack.top() << "\n\n";
cout << "\nPopping off the stack: " << stack.pop() << endl;
cout << "Popping off the stack: " << stack.pop() << endl;
cout << "Stack size: " << stack.getCount() << endl;
cout << "Stack is " << (stack.isEmpty() == true ? "empty\n" : "not empty\n");
cout << "Top of the stack is: " << stack.top() << "\n\n";
stack.push(6);
stack.push(7);
cout << "After pushing 6-7 \n";
cout << "Stack size: " << stack.getCount() << endl;
cout << "Stack is " << (stack.isEmpty() == true ? "empty\n" : "not empty\n");
cout << "Top of the stack is: " << stack.top() << "\n\n";
stack.push(8);
stack.push(9);
cout << "After pushing 8-9 \n";
cout << "Stack size: " << stack.getCount() << endl;
cout << "Stack is " << (stack.isEmpty() == true ? "empty\n" : "not empty\n");
cout << "Top of the stack is: " << stack.top() << "\n\n";
while (stack.isEmpty() == false) {
cout << "Popping off the stack: " << stack.pop() << endl;
}
cout << "Stack size: " << stack.getCount() << endl;
cout << "Stack is " << (stack.isEmpty() == true ? "empty\n" : "not empty\n");
cout << "Top of the stack is: " << stack.top() << "\n\n";
}
//Answer
/*Stack size: 5
Stack is not empty
Top of the stack is: 5
Popping off the stack: 5
Popping off the stack: 4
Stack size: 3
Stack is not empty
Top of the stack is: 3
After pushing 6-7
Stack size: 5
Stack is not empty
Top of the stack is: 7
After pushing 8-9
Stack size: 7
Stack is not empty
Top of the stack is: 9
Popping off the stack: 9
Popping off the stack: 8
Popping off the stack: 7
Popping off the stack: 6
Popping off the stack: 3
Popping off the stack: 2
Popping off the stack: 1
Stack size: 0
Stack is empty
Top of the stack is: -999*/









