<div align="center">

## Flawless Bug in C\+\+


</div>

### Description

Logical Bug in C++. C++ contradicts its own errors by saying that p is a constant, and in the next line says that p is not a constant.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Nitin Gupta](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/nitin-gupta.md)
**Level**          |Beginner
**User Rating**    |4.7 (42 globes from 9 users)
**Compatibility**  |C\+\+ \(general\), Borland C\+\+
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/nitin-gupta-flawless-bug-in-c__3-1636/archive/master.zip)





### Source Code

Consider the following program
<BR><BR>
#include <iostream.h><BR>
#include <conio.h><BR>
<BR><BR>
void main()<BR>
{<BR>
 int n;<BR>
 cin>>n;<BR>
 const int p = n;<BR>
 p++;  <B>// C++ gives error that p is a const</B><BR>
 int a[p]; <B>// C++ gives error that p is not a const</B><BR>
}<BR>
Now how can c++ give an error for p being a constant in first commented line and also an error for p not being a constant in the second commented line.....logical huh? And the program compiled perfectly till the line<BR>
  const int p=n;<BR>
(This line is accepted).<BR><BR>
Anyone with a way out, plz write a message. And if u feel that this discovery is worth a credit, plz vote.

