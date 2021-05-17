# Verilog
Verilog Learning 
                                                                      Verilog
       *Verilog is used for Digital Hardware design or It is used for describing behavior of hardware.
       *IEEE Standard 1364-1995
       *IEEE Standard 1800(in 2009)
       *First Appeared 1984
 Properties of Verilog 
 *Abstraction 
      ---Independent of technology
 *Concurrency
      ---Speed up the performance 
 *Vendor Neutrality 
      ---No monoploy
      ---code independency 
 *Re-Usability
      ---Reduce design cycle 
 *Scalability 
      ---Flexibilty in design 
 *Ease of Debugging 
      ---Flexibility in Coding 
   
   
                                                      Operators in Verilog 
                          Verilog Operators 
      1 : BitWise Operators (Unary and Binary )
               A: Unary Operators ( Reduction Operators )   ( used left of Operand)
                 y = &a , y = ~a , y = ~&a , y = ~|a , y = ^a 
          Eg: a = 5'b10101 
              &a = 1b'0  //AND  all bits 
              ^a = XOR all bits = 1^0^1^0^1
              ~&a = NAND all bits 
              ~|a = NOR all bits 
      
               B: Binary Operators (Used Between Operands )
                          a = 3'b101  , b =3'b110
                     y = a & b (Binary AND = 3'b100)
                     y = a | b (Binary OR = 3'b111)
                     y = a^b (Binary XOR )
                     y = a~^b (Binary XNOR )
                     y = a~&b (Binary NAND)
                 
      2: Arithmetic Operators 
               ( + , - , * , / , % )
         a = 3'b101 , b = 3'b100
         y = a + b , a * b , a - b;
         
      3: Relative Operators 
          It compares two Values and return either 
          1 & 0    a = 3'b010 , b = 3'b100
          a > b = 1'b0 (false) ( a is greater than b : a > b)
          a < b = 1'b1 (true) (a is less than b : a < b )
          a >= b = 1'b0 (false) ( a is greater than or equal to b : a >=b )
          a <= b = 1'b1 (true) (a is less than or equal to  b : a <=b )
          
       4: Equality Operators ( Used to Compare values and return true or false )
         a = 3'b010   ,   b = 3'b100    ,   c = 3'b111    ,   d =  3'b01Z ( Z High Impedence )   ,  e  =  3'b01X 
         == (equality ) -----  a == c ( false = 1'b0)
         != ( not equality ) ----- e ! = e ( false = 1b'0)
         === (case equality ) ----- e ==== e (true = 1'b1) ( Check Whether each bit equal )
         !== (case inequality ) ----- e!==d ( true = 1'b1) 
                   5 == 10 (1'b0) , 5 == 5 (1) , 5!=5 ( 0 )  ,  5 != 6 ( 1 )
                   4'bX001 === 4'bX001 ---- 1
                   4'bX0X1 === 4'bX001 ---- 0
                   4'bZ0X1 = 4'bZ0X1 ---- 1 
                   4'bX0X1 != 4'bX001 ---- 1
                   
       5: Logical operations (return 1 or 0)
          ! (Not true), && (both expression true), || (One or both expression true)
                  a = 3'b10l (not zero) 
                  b = 3'b000 (zero = false)
                  !a - false (0),
                  a && b --- false (0)
                  a || b --- true (1'b1)  
           if any is Z or X result is unknown

       6: Shift operators 
          >> (right shift)  ,  << (left shift) 
          shifted bits are lost and zero is filled
          a = 4'b1010   ,   b  = 4b'10X0 
          b >> 1 ---- 010X      a << 2 ---1000 

       7: Concatenation Operators { }
          It Combines bits of 2 or  more data
          a = 3'b101  ,  b = 2'b10   ,  c = 4b'1001
          y = {a,b} --- 5'b10101     y = {c,b,a}   ---- 9'b100110101

       8: Replicate Operators {{}}
       It replicates a group of bits n times.
       The number in front of the brackets is known as the repetition multiplier.
       y = {3{2'b10}} = 6b'101010
       y = {2{3'b101}} = 6'b101101

       9: Conditional Operators
          It evaluates condition or logical operation and then assign
             Syntax:
           output = Condition to be checked ? True Value : false Valuse
           a = 3'b101  (5)    ,    b = 3'b100  (4)
           y = (a > b) ? (a+b) :(a-b)          y = 4'b1001
           y = (a == b) ? (~a) : (a & b)       y = 3'b100

                                                              _Syntax_ in _VERILOG_

       1: Comments
           It makes the code more readable so use many .
           Two types of comments
              Single line comments //           
              Multiline Comments /*              */
              
       2: Whitespace
            It is used to separate variable, Key words, identifiers etc. If it makes the verilog codes look clean and more readable
            Eg: input a ;   
            output q;
            module diff (d, q);

      3: Cose- Sensitive
            Verilog is case sensitive. All the Keywords lower case.
                 input a; and input A; are different
                 reg and REG are different

      4:Keyword
            These are special words used in verilog

            always

            and

            assign

            begin

            buf

            bufif0

            bufif1

            case

            casex

           cmos

           casez
 
          deassign

          default

          defparam

          disable

          end 

          else

          endcase

          end module

          end function

          end primitive

          endspecify

          endtable 

          endtask

          event

          for 

          force

          forever

          function

          higz0

          higz1

          if

          if none 

          inital

          inout

          input

          integer

          join

          large

          macromodule

          medium

          module

          nand

          nmos

          not

          notif 0

          notif 1

          of

          output

          parameter

          pmos

          posedge

          primitive

          pull 0

          pull 1

          pull up

          pull down

          remos 

          real

          real time

          reg

          release

          repeat

          rpmos

          rnmos

          rtran

          rtranif 0

          rtranif 1

          scalared

          small

          specify

          specparam

          strong 0

          strong 1

          suppy 0  

          supply 1

          table 

          tran

          task

          time

          tranif 0

          tranif 1

          tri

          tri 0

          tri 1

          triand

          trireg

          vectored

          wait

          wand

          weak 0

          weak 1

          while 

          wire

          wore

          xnor

          xor

      5: Identifier
               It is used to identify an object like variable, input or output port, module etc.
                 Points to remembes
                 1. Identifies must begin with a-z ,A-Z,_
                 2. It may contain a-z,A-Z,_,$
              Eg: adderpro, DFF_ver, _counter$10
                  NOT ALLOWED : 10counter, @srff,$decoder, #rammodule

     6: Number Specification
              Number can be represented in decimal binay,octal,hexadecimal
              By default all numbers are decimal in verilog. 
                    Two format is followed :
                           A: SIZED : WITH BASE FORMAT
                                    SYNTAX:
                                    <size>'<base format><number> 
                                    Base format (b-binary, d-decimal, o-Octal, h-hexadecimal)
                             Size is written in decimal only
                                  Eg: 4'b0100; // size = 4, base format is binary, number 0100 = 4
                                      3'd6; // decimal 6
                                      8'b1010_l0ll; // for easy reading 
                                      16'h16ad; // hexadecimal
                                      16'd255; // decimal
                                      8'o12; // Octal
                                      32'h12F5_DCB5; // _separates 16 bit numbers Ox123 = 16'h123

                            B: UNSIZED : NUMBERS WITHOUT BASE FORMAT

Number without base format is decimal numbers by default...

Eg: Integis a= 2347; // no base format so value - decimal 2347

Integer = '012 :// no size 30 a-3200000012

integer a='h1234; // no pia

h0000-1234



Code for

module

Youtput

D

flip flop

Indatifies

diff -p (q, d, clk, rst); // module dif

drst

11 aways @ (posedge alli or posedge ast))

begin

if (ist)

end

endmodule

multiple comment

(keyword) predefined


DATA Types in Veritag

nata types tell the type of data in variable can have (in digital world its mostly bits) A Hardware ekt can have one 4 Values

represents logic zolo, false condition.

represents logic one, true condition

un known logic (can be 1 x 0) High impedance floating value

Represents voltage anywhere between 0.80 to 5v.

(depends of fabrication technology) represente voltage less than 0.8V to ov

(diperds on fabrication technology used) X- unknown value instally and can be either 1040 2- any unconneded cut gives high impedance (need to be taken care)

Yerilog data type are types

Net data ↳ Register data type Net (wise

thier, trand etc..) Register (reg, Integel, seal, time)

These are all keyword


Net data type

There are wed to connect logic gates. It doesn't Store valve any on its own u digital logic wire is used. It is wand schen... design mostly there is a continious assignment on to dolwe a acosande circuit. His most Ilke a clistical wise to connect 2 componente.

-By default all the data types are whre (default) 9 wire ai // single not
wire [2:0) a: 11 multiple net 11a (2), a[1],9[0] combined together

AN

Out

FF

out

ed

Register data type

3: it is used to present a valiable and can store data beturen assigments. So it is used to Model hardware registars (constructed from

flip flop) to store I or more hits. It can allo stope combinational logie. It's default value is X and unsigned integue.

Number of bits it can store depende architecture

reg a', // gove I bit // so I bit flip flop reg. [io] a // ton 4 bit /14 no. of 1 bit tip flop

To hold data →g Continuces assimmet Date "Lowite (no

Integes:

It is signed integes variable of en bit wide. It's a general purpose registes data type for

manipulating quantities. default met width is boot maching stze (at least 32 bit) 6.

Eg: integer countes: tritiel intitial Same

counter = 1;

real:

It stores signed floating point value and Loff to nearest integer when assigned

to an integer. It's default value = 0;

Eg: real float; avariable initial

float = 4e10; // 4x 10 b

time:

Its an unsigned integu valiable and 64 bit wicke It is used to store simulation time during debugging

Eg: time sim time: 1/4 stores simulation time in

test barch • Homing parameter.


strings:

It is nothing but a sequence of character enclosed. in double "") H is stored in mag variable Here each char. Is s byte to reg be large enough to hold data.

module strings (); reg

Me declare a register Lavable of 28 byte (alshyt initial (24

begin

string="hello verilog world", $ display ("1.s n", string); end

endmodule

Output: hello verilog world


Vector and Array in Veriny

Vector in Verily

digital design flipflop is used to store & bit data and if more no. of bits then it is syiste.. -Key word (reg) and (wife) is used to declare

reg (30) a 11 Solene I bit dato and called se ALAR 11 stay 4 bit data and called VECTOR

11MSB = 3, LSB=0 // we start with rightmost (0) and more to left most (3)

reg [3:0] a; // store 4 bit data and called vectop 11 HSB=0 LSB=3 11 we start with leftmest [3] and move to right mouth

wise a; // stose I bit and called Scalar wise [4:0] as stove 5 bit and called [vected wix [0:4) a; // stail 5 bit and called vector

Syntax: wire [MSB: LSB] O jeg [MSB: LSB). The lift number is always MSB -HSB and LSB should be constant and can't he

Ⓒ reg [0:0]; // not allowed // variable niside 1

a[1] [2) alú alo)

MSB [258] alya(y) 9 (1)


F2

b₂

bs=gr

by = b 084

bg= 4 ga

b₁ = ₂ gi

bo = "²bi@go

module Gray binary # (parameke N=*)

imput (N-1:0] gadg

3 output wire [N-1: 0]b_8 wire [N-1:0] Jemp.

assign temp (N-1) = 2_1(N-1); gerivar P

generate

for (i-N- 2; 1>= 0; i = 1-1)

begin assign tempo (i) = tmmplit() og i();

end end generales


Any individual bit of a vectal can be sepat selected and assigned to a new Var. [g: reg [8:0] count;

Count [3] =j'b1; //assigned to I MBB Count [2] = 1'60; ll assigned to o to bit nos Even some portion of vector can also be selected and

assigned

Eg: reg 17:0] count;

Count [6:4] =3¹b110;

Xesto: Arraycy choy

A vector is a single element that is bits wide but arrays are multiple elements that are I bit or n-bit wide.

It is allowed for kg, integal, time and real

data typer.

Eg: integer count [o:7 ] ; 11 array having

Integer [0:7] count; // Vector 01234567 Integer matrix [2:0] [70] // array² [

reg [20] mem [0:1] // 2

xg Hem [2] =g² bl10; //

9

23

101

R C

[2:0] mem [0:¹] [0: 2] 11 away

veg = 6000

mem [1] [2] = 8' boll mem [2][1] = 3 bol;

Yevlog Code

module pracarray(); reg [2:0] a [d²3] [0²4];

initial

begin

a 10 (0) = 3' bood; a[0][1] = 3²6001; a[0) (2)=116011

a [1][0] 3'b 101 a [12 (1) = 31 b | 10,

[1] [2] =3611; 9/1) (3) - 3000

all][4] = 3 bool;

9[2][6] =36010 a(²) (1) = 1² boll a[2][2] =31b 100; a[2][2] = 3 6 101

a [2][4] = 36 110

[3][0]-gb 111; a[3] [1] = 3 1000

a (3) 12) = 36001) a[3] [3] = ?' xxx;

$display (a (o) (1) = vibu & display ( 9 (²

& display (9[3] [3) = 1.b. 93 { display are 4) = 4. b, a (1)

end

endmodule

AR SO

Date Page

یا

XXX

[1] [4] 001


Module in Verilog (stucture in Verllog)

Moctub :

This to the basic building blocks in velilog. It can be a single element or collection of bactes. # hides internal Implementation

Syntax: module <name of module> <terminal portlist?).

< post declaration>

a functionality)

endmodule // mo at the end

keyword Module and endmodule are - Module represents the design that implements the certai

behavioral chas.

- All vovable declaration, terminal port, functionality dings are defined within module and endmodule
wo can include module within module is called module instantiation

Module can be seusedus

Eg: module counter ();

end module


Modules are connected by ports. A part can be input output on Inout Rame name not used for different ports,

£g: module and get (a, b,y); garf mput ANDOT Yout

input by //mput a, b, output modil y's ll output pourt b-D y assign y=a&b; "gives sexult

end module: module and gt (Input a infot , tht ()

assign y-a&b: 11 given result and mochile

Port are used to send or receive data from outsid, she world.

Syntax: input (not type> <rage> input bout name: in out (not type> <rayey thout port sans outfit < not typey <manger outfact pat name",

Input- design modul recolves from outfurt ung
