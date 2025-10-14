EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:
```
char stack[50];
int top,i;
void display()
{
    for(i=top;i>=0;i--)
    {
        printf("%c ",stack[i]);
    }
    
}
```



Output:


<img width="510" height="248" alt="493152352-2cac8207-f545-42c1-b7b5-73017e873e79" src="https://github.com/user-attachments/assets/b15ffe83-6699-42f3-81f6-c0d6abe82de1" />



Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:
```
int size=3,top=-1;
float stack[100];
void push (float data)
{
    if(top==size-1)
    {
        printf("stack is full");
    }
    else
    {
        top++;
        stack[top]=data;
    }
}
```



Output:

<img width="512" height="251" alt="493152495-5fcadddf-e6b4-4f96-bb20-5e909f2aa268" src="https://github.com/user-attachments/assets/ee5a429c-5e4b-4958-b6e1-e1e1910773dc" />





Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:
```
int front,rear;
char queue[50];
void display()
{
    if(front==-1 || front>rear)
    {
        printf("No elements to display\n");
    }
    else
    {
    for(int i=front;i<=rear;i++)
    {
        printf("%c\n",queue[i]);
    }
    }
}
```



Output:
<img width="809" height="679" alt="493152684-2b82736c-5317-45da-b0d5-968f21c55d3f" src="https://github.com/user-attachments/assets/3b83f510-02b4-4af7-8877-0ad8fe191146" />




Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:
```
int size=10, rear=-1, front=-1;
float queue[50];
void enqueue(float data)
{
    if(rear<size)
    {
        if(front==-1)
        {
            front=0;
        }
        rear=rear+1;
        queue[rear]=data;
    }
}
```



Output:

<img width="804" height="469" alt="493152880-4d6ba6f6-0d66-468e-8d34-31d86b26fa67" src="https://github.com/user-attachments/assets/ba2e7205-ac01-40a9-bef5-e1b40fb3514b" />


Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:

```
float queue[50];
int front, rear;
void dequeue()
{
    if(front==-1||front>rear)
    {
        printf("\nNo elements to display");
    }
    else
    {
        front++;
    }
}
```



Output:

<img width="805" height="482" alt="493153059-2bae1fa7-f33c-47ab-826a-faff41c2278a" src="https://github.com/user-attachments/assets/498734fc-76d0-4ce4-a7d9-63c5954bb274" />



Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
