# task3.githup.io
Used of const keyword:
1.	specifies that a variable's value is constant and tells the compiler to prevent the programmer from modifying it.
>Ex: const int data=5;
>(This value of variable data wouldn’t change)
>
2.	A pointer to a variable declared as const can be assigned only to a pointer that is also declared as const.
>Ex: const int *ptr=&value;
   value=5;
>(Value wouldn’t change)
>
3.const pointer pointing to a const variable
>Ex: Const int *const ptr=&value;
>(Value and pointer (ptr) both are constant)
>
4. const pointer variable point to the value
>Ex:int *const ptr=&value;
>(Pointer (ptr) is constant).
>
5.const-function Declaration
>Ex:const void push(){
 //code of the function
}
>int main (){
>push(5)
}

6. const member function of the class
>Ex:class linked_list{
>int y;
>public:
>void push()const
{
//code of function 
}
};
>
7.  const return type 
>Ex:const void push(){
 //code of the function
}
>int main (){
push(5)
}
>
8. Const function parameters
>Ex:void add(const int y){
>cout<<y<<endl;
}
>int main (){
>y=10;
>z=0;
>add(z);
}
>
9. you can use the const keyword instead of the #define preprocessor directive to define constant values.
>Ex: const int size=100;
    > instead of #define size 100
>
Used of &:
1.	(address) operator yields a pointer to its operand.
>Ex:Ptr=&y;
>2.	a reference declarator in addition to being the address operator
>
>3.	with overloaded functions only in an initialization or assignment where the left side uniquely determines which version of the overloaded function is used.
>4.	Bitwise AND
>Ex:int main (){
>int a=9,b=5;
>int c;
>c=a&b;
>cout<<”a&b= ”<<c<<endl;
}
>Output->a&b=1
5.	Logical AND
>Ex:1-> int main (){
>int x=3,y=7;
>if(y>1&&y>x){
>cout<<”y greater than x and 1 ”<<endl;
}
>else{
>cout<<”y is smaller than x or 1”<<endl; }
> 2->int main (){
>int x=5,y=2;
>cout<<x&&y<<endl;
>return 0;
}
>Output-> 1
>(The logical condition is true because 5&&2=true)
>or 
>int main (){
>int x=0,y=5;
>cout<<x&&Y<<endl;
>return 0;
}
>Output-> 0
>(The logical condition is false because x=0 so 0&&5=false)
