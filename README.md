# Experiment 2 

# Aim: 
To study and implement C++ Program Structure (Data Types)

# software used
VS code 

# Theory: 
"sizeof" is a unary operator that finds the size of data types of variables and constants. The sizes of data types are the same in all the cases usually, for example int always is 4 bytes and so on. 
in the first code, we find the size of character, int, float, short int, long int, bool, long double. 

In the second code, it is user defined. The user will enter an integer, float, short int and long int and the program will find the size of it. 

In the third code, we use the stroage classes, auto and register. However there are 4 storage classes in c++. They are auto, extern, register, static and mutable.
Auto class uses the global variable as its default. 

register defies local variables and has max size as the register size 

static is not user defined since it only takes one value 

extern uses global files which are visible to ALL programs 

# codes
 1. first code

#include< iostream >

using namespace std;

int main()

{

    cout<< "size of char: " <<sizeof(char) << "byte(s)" <<endl;
    
     cout<< "size of int: " <<sizeof(int)<< "byte(s)" <<endl;
     
     cout<< "size of short int: " <<sizeof(short int) << "byte(s)" <<endl;
     
     cout<< "size of long int: " <<sizeof(long int) << "byte(s)" <<endl;
     
     cout<< "size of float : " <<sizeof(float) << "byte(s)" <<endl;
     
     cout<< "size of double: " <<sizeof(double) << "byte(s)" <<endl;
     
     cout<< "size of long double: " <<sizeof(long double) << "byte(s)" <<endl;
     
     cout<< "size of bool: " <<sizeof(bool) << "byte(s)" <<endl;
     
     return 0;
     
}

output:
![image](https://github.com/user-attachments/assets/ea901ae5-aedb-496c-83a1-5c3906674ab4)

2. second code

#include < iostream >

using namespace std;

int main()

{

    int a;
    
    cout<<"enter any integer: ";
    
    cin>>a;
    
    cout<<"\n integer = "<<a<<" and size is "<<sizeof(a)<<" bytes";
    
    float b;
    
    cout<<"\n enter a number: ";
    
    cin>>b;
    
    cout<<"\n Float= "<<b<<" and size is "<<sizeof(b)<<" bytes";
    
    short int c;
    
    cout<<"\nenter an interger: ";
    
    cin>>c;
    
    cout<<"\nShort integer = "<<c<<" and size is "<<sizeof(c)<<" bytes";
    
    return 0;
    
}

![image](https://github.com/user-attachments/assets/eed71c05-278f-45c9-aa61-3484372a9ecb)



3. code 3 

#include < iostream >

using namespace std;

int main()

{

    int a;
    cout<<"enter any integer: ";
    cin>>a;
    cout<<"\n integer ="<<a<<" and size is "<<sizeof(a)<<" bytes";
    
    int register b;
    cout<<"\n enter a number: ";
    cin>>b;
    cout<<"\n REGISTER= "<<b<<" and size is "<<sizeof(b)<<" bytes";
    
    int auto c;
    cout<<"\n enter an interger: ";
    cin>>c;
    cout<<"\n Auto = "<<c<<" and size is "<<sizeof(c)<<" bytes";
    return 0;
}

![image](https://github.com/user-attachments/assets/4a9ac1b8-6aab-4f31-9222-18b75c5aa701)
