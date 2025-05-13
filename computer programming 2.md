*bug* - an error in a computer program that causes it to behave incorrectly.

*Describe three senerios where an exeption can occur in programming*
- Dividing by zero
- Accessing an invalid array index
- Openning a missing file

*Write a short C++ program that asks the user to enter two numbers, obtain the numbers from the user and print the product of the two numbers entered by the user*
```c++
#include <iostream>
using namespace std;

int main() {
int a,b
cout << "Enter two numbers: ";
cin >> a >> b;
cout << "Product: " << a * b << endl;
return 0;
}
```

*Write the advantages of OOP over procedual programming*
- It is easier to maintain
- Data hiding through encapsulation
- Reusability
- Better real-world modelling

*Describe the system development life cycle*
1. Planning
2. Analysis
3. Design
4. Implementation
5. Testing
6. Maintainance

*Differenciate between a local and a class variable*
A __Local__ variable is inside a function and for temporary use while a __Class__ variable is inside a class and shared by methods.

*Discuss the guidelines on access modifiers as a good prorgamming practice*
- Use `private` to hide internal data.
- Use `public` only when needed.
- Use `protected` for inheritance.

*Describe any six control flow structures in C++*
- if
- else
- switch
- for
- while
- do-while

*Using a diagram distinguish between bidirectional and composition type of assosiation*
![[computer programming 2 2025-05-07 08.41.44.excalidraw]]
In compsition, the class b dies if class A dies.

*Benefits of Object-oriented programming*
1. Code reusability
2. Easier maintainance
3. Improve modularity
4. Real world modelling

*Distingish between the following*
*Objects and classes* - Objects consist of instances while classes are blueprints.
*Abstraction and encapsulation* - Abstraction is the act of representing features without including the background details while encapsulation is wrapping up of data and function into a single unit.
*Dynamic binding and message passing* - Dynamic binding links calls at runtime while message passing is calling methods on objects.

*Define inheritance in OOP*
Inheritance allows a class to acquire features from another class promoting reuse.

*Polymorphism*
This is the ability of an object to take more than one form

*Explain how data functions are organised in object-oriented programming*
Data and functions are grouped inside classes, ensuring encapsulation and structure.

*What is the use of a constructor in OOP*
Automatically initialized objects when created and setting default or passed values.

*operators in C++*
<<  - Insertion operator
">>" - Extraction operator
`*` - pointer to a member operator
`delete` - memory release operator
`New` - Memory allocation operator

**(a) Early vs Late Binding [4 marks]:**

- **Early Binding**: Function call is resolved at compile time.
    
- **Late Binding**: Function call is resolved at runtime (used in polymorphism).
    

---

**(c) Inline Function Example [4 marks]:**

```cpp
#include <iostream>
using namespace std;

inline int square(int x) {
    return x * x;
}

int main() {
    cout << "Square: " << square(5) << endl;
    return 0;
}
```

**Explanation:** Function code is inserted directly at call site, reducing overhead.

---

**(d) Three Forms of Constructors [6 marks]:**

1. **Default Constructor** – no parameters.
    
2. **Parameterized Constructor** – takes arguments.
    
3. **Copy Constructor** – copies from another object.
    

---

**QUESTION FOUR**

**(a) Encapsulation vs Polymorphism [4 marks]:**

- **Encapsulation**: Hiding data inside classes.
    
- **Polymorphism**: One interface, many forms (method overloading/overriding).
    

---

**(b) `main()` in C++ vs `main()` in C [3 marks]:**

- **C++ main()** supports object-oriented code.
    
- **C main()** is procedural.
    
- C++ may return `int`; older C used `void`.
    

---

**(c) C++ Program for Fahrenheit to Celsius [2 marks]:**

```cpp
#include <iostream>
using namespace std;

int main() {
    float f, c;
    cout << "Enter Fahrenheit: ";
    cin >> f;
    c = (f - 32) * 5 / 9;
    cout << "Celsius: " << c << endl;
    return 0;
}
```

---

**(d) Promising Areas for OOP [4 marks]:**

1. GUI apps
    
2. Game development
    
3. Simulations
    
4. Web and mobile apps
    

---

**(e) Characteristics of Real-World Objects [4 marks]:**

1. **Identity** – unique existence
    
2. **State** – properties/attributes
    
3. **Behavior** – actions/functions
    
4. **Encapsulation** – data + behavior bundled

**(a) Five Data Types in C++ [5 marks]:**

1. **int** – stores integers (e.g. `int age = 25;`)
    
2. **float** – stores decimals (e.g. `float price = 10.5;`)
    
3. **char** – stores single characters (e.g. `char grade = 'A';`)
    
4. **bool** – stores true/false (e.g. `bool passed = true;`)
    
5. **string** – stores text (e.g. `string name = "Alex";`) *(requires `<string>`)
    

---

**(b) Rules for Naming Identifiers [6 marks]:**

1. Must begin with a letter or underscore (`_`).
    
2. Cannot start with a digit.
    
3. Can contain letters, digits, and underscores.
    
4. No spaces or special characters.
    
5. Cannot use C++ reserved keywords.
    
6. Case-sensitive.
    

**Two Approaches to Defining Methods in C++:**

**1. Inside the class (inline):**

```cpp
class Car {
public:
    void start() {
        cout << "Car started!" << endl;
    }
};
```

**2. Outside the class:**

```cpp
class Car {
public:
    void stop();
};

void Car::stop() {
    cout << "Car stopped!" << endl;
}
```

---

**(c) Arrays in C++ [6 marks]:**

**i) One-Dimensional Array:**

```cpp
int numbers[3] = {10, 20, 30};
cout << numbers[1];  // Output: 20
```

**ii) Two-Dimensional Array:**

```cpp
int matrix[2][2] = {
    {1, 2},
    {3, 4}
};
cout << matrix[1][0];  // Output: 3
```

---

**(d) Four Areas Where C++ Is Applicable:**

1. **Game development** – for performance.
    
2. **System/software tools** – like compilers.
    
3. **Embedded systems** – small device programming.
    
4. **Finance systems** – fast, efficient processing.
    

---

**Inheritance Examples with Diagrams:**

**i) Single Inheritance:**

```cpp
class Animal {
public: void speak() {}
};

class Dog : public Animal {};
```

```
Animal → Dog
```

**ii) Multiple Inheritance:**

```cpp
class Flyable { public: void fly() {} };
class Swimmable { public: void swim() {} };

class Duck : public Flyable, public Swimmable {};
```

```
Flyable ─┐
         ├─> Duck
Swimmable┘
```

**iii) Hierarchical Inheritance:**

```cpp
class Animal {
public: void eat() {}
};

class Dog : public Animal {};
class Cat : public Animal {};
```

```
       Animal
       /    \
    Dog     Cat
```