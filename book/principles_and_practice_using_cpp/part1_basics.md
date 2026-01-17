# A Brief History of C++
----------

Basic idea of C++ was to combine C's ability to utilize hardware efficently (e.g., device
drivers, memory managers, and process schedulers) with facilaties for organizing code (notably classes and derived classes). 

## ISO Standard for C++

In 1989, several large corporations decided that we needed an ISO standard for C++. Together
with Margaret Ellis, I wrote the book that became the base document for C++’s standardization
‘‘The ARM’’ [ARM]. The ﬁrst ISO standard was approved by 20 nations in 1998 and is known as
C++98. 

## PPP Support 

All the code in this book is ISO standard C++. To start compiling and running the examples, add
two lines at the start of the code:

~~~
impor t std;
using namespace std;
~~~

** This makes the standard library available.

Unfortunately, the standard does not guarantee range checking for containers, such as the stan-
dard vector, and most implementations do not enforce it by default.  Typically, enforcement must be enabled by options that differ between different compilers. We consider range checking essential to
simplify learning and minimize frustration. So, we supply a module PPP_suppor t that makes a ver-
sion of the C++ standard library with guaranteed range checking for subscripting available (see
www.stroustrup.com/programming.html). So instead of directly using module std directly, use:

~~~
#include "PPP.h"
~~~

----------

# The Basics 

## ** 1 - Hello, World!

~~~
// This program outputs the message "Hello, World!" to the monitor
impor t std;
 // gain access to the C++ standard library
int main()
 // C++ programs start by executing the function main
{
std::cout << "Hello, World!\n";
 // output "Hello, World!"
return 0;
}
~~~

~~~
import std;
~~~


Standard module making all facilities from the C++ standard
library available. 

Every C++ program must have a function called main to tell it where to start executing. A function
is basically a named sequence of instructions for the computer to execute in the order in which they
are written. A function has four parts:
• A return type, here int (meaning ‘‘integer’’), which speciﬁes what kind of result, if any, the
function will return to whoever asked for it to be executed. The word int is a reserved word
in C++ (a keyword), so int cannot be used as the name of anything else.
• A name, here main.
• A parameter list enclosed in parentheses (see §7.2 and §7.4), here (); in this case, the param-
eter list is empty.
• A function body enclosed in a set of ‘‘curly braces,’’ { }, which lists the actions (called state-
ments) that the function is to perform.


## 2 - Objects, Types, and Values

### Input

Somewhere in the computer memory to place what we read. Call that place an object. 
An object is a region of memory with a type that speciﬁes what kind of information can be be placed within it.
Named object is called a variable. For example, character strings are put into string variables and integers are put into int variables. 

Think of an object as a "box" into which you can put a value of the objects type. 

#### cin stands for character Input



### variables
"places" in which we store data are called objects. To access an object, we need a name. A named object is called a variable and has a speciﬁe type (int,string,...) that determines what can be put into the object and which operations can be applied. 

The data items we put into variables are called Values. A statement that defines a variable is called a definition. 

int number_of_steps = 39; int for integers
double ﬂying_time = 3.5; double for floating point numbers
char decimal_point = '.'; char for individual characters 
string name = "Annemarie"; strings for character strings
bool tap_on = true; bool for logical variables


