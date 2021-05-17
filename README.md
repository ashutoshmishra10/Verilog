# Verilog
   wanna learn Verilog ??? 
   
   
                                                        Verilog
       *Verilog is used for Digital Hardware design or It is used for describing behavior of hardware.
       *IEEE Standard 1364-1995
       *IEEE Standard 1800(in 2009)
       *First Appeared 1984
       -------------------------------------------------------------------------------------------------------------------------------
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
   -------------------------------------------------------------------------------------------------------------------------------------
   
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
        ---------------------------------------------------------------------------------------------------------------------------------------
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
                                         Eg: Integer a= 2347; // no base format so value = decimal 2347
                                             Integer a= 'o12 ;// no size so a=32'o0000_0012
                                             Integer a= 'h1234; // no size a = 32'h0000_1234
                                             
                       CODE FOR D FLIP_FLOP
                               module diff_p(q,d,clk,rst);  // Module def. d (identifier)
                               input  clk,d,rst;            //Input
                               output q;                    //Output
                               reg q;
                                 //always @ (posedge clk or posedge rst)
                                 /*
                                 begin
                                 if (rst)
                                 q<=1b'0;                            multiple comment
                                 else
                                 q<=d
                                 end
                                 endmodule                      (keyword) predefined
                                 */
           --------------------------------------------------------------------------------------------------------------------------------------------

                                DATA Types in Verilog
             Data types tell the type of data variable can have (in digital world its mostly bits)
             A Hardware circuit can have one of four values
                         ----------------------------------------------------
                            0     represents logic zero, false condition.
                            1     represents logic one, true condition
                            X     unknown logic (can be 1 or 0) 
                            Z     High impedance floating value
                         ------------------------------------------------------
                            1      represents voltage anywhere between 0.8v to 5v (depends of fabrication technology)
                            0      represents voltage less than 0.8V to ov (depends on fabrication technology used)
                            X      unknown value initally and can be either 1 or 0 
                            Z     any unconnected circuit gives high impedance (need to be taken care)

                      Verilog data type are types
                                  ↳ 1: Net data 
                                  ↳ 2: Register data type
                                             Net (Wire, trior, triand etc..) 
                                             Register (reg, Integer, real, time)
                                      These are all keyword

                      Net data type
                These are used to connect logic gates. It doesn't Store any value on its own in digital logic design mostly wire is used.
                It is used when there is a continious assignment or to drive a circuit. It is most like a electrical wire to connect 2 component.
         -By default all the data types are wire (default value = z) 
           Eg: wire a; // single net
           wire [2:0] a; // multiple net
                        // a [2], a[1],a[0] combined together

                     Register data type
                reg: it is used to represent a variable and can store data between assigments. 
                     So it is used to Model hardware registers (constructed from flip flop) to store 1 or more bits.
                     It can also store combinational logie. 
           It's default value is X and unsigned integer.
           Number of bits it can store depends on the system architecture
               Eg: reg a; // gove 1 bit
                   reg [3:0] a; // store 4 bit
                                // 4 number of 1 bit flip flop 
          To hold data →reg 
             Continuces assignment
                         ↳ wire (no data storage )

         Integer:
            It is signed integer variable of 32 bit wide. It's a general purpose register data type for manipulating quantities.
            Its default width is host machine word size (at least 32 bit)
               Eg: integer countes; 
               intitial
               counter = 1;

         Real:
            It stores signed floating point value and rounded off to nearest integer when assigned to an integer.
            It's default value = 0;                               [a = 4.3]
                Eg: real float;                                   [a = 4  ]
                initial                                           [a = 4.8]
                float = 4e10; // 4X10 ^10                         [a = 5  ]

         Time:
            Its an unsigned integer variable and 64 bit wide. It is used to store simulation time during debugging.
               Eg: time sim_time; // it stores simulation time in ns or ps
                                                     test bench • timing parameter
         Strings:
            It is nothing but a sequence of character enclosed in double "". It is stored in reg variable 
            Here each char is 1 byte so reg variable should be large enough to hold data.
                            module strings ();
                            reg[8*28:0] string;  // declare a register variable of 28 byte
                            initial
                            begin
                            string = "hello verilog world", 
                            $ display ("%s \n", string); 
                            end
                            endmodule
                    Output: hello verilog world
            ---------------------------------------------------------------------------------------------------------------------------------------------------------------
                             Vector and Array in Verilog
                                 Vector in Verilog
      In digital design flipflop is used to store 1 bit data and if more no. of bits then it is register.
            -Key word (reg) and (wire) is used to declare vector
         Eg: reg a; // Store 1 bit data and called SCALAR 
             reg [3:0] a; // store 4 bit data and called VECTOR
                          // MSB = 3, LSB=0 
                          // we start with right most (0) and move to left most (3)
             reg [3:0] a; // store 4 bit data and called vector
                          // MSB=0, LSB=3 
                          // we start with leftmost [3] and move to right most[0]
             wire a; // store 1 bit and called Scalar 
             wire [4:0] a; // store 5 bit and called vector
             wire [0:4] a; // staore 5 bit and called vector
                     Syntax: 
                          wire [MSB: LSB] or reg [MSB: LSB];
                       --The left number is always MSB 
                       --MSB and LSB should be constant and can't be variable;
                           reg [a:0]; //not allowed
                                     //variable inside[]
                    module gray2binary #(parameter N=4)
                    {
                       input [N-1:0] g_1;
                       output wire [N-1: 0] b_0;
                    }
                       wire [N-1:0] Temp;
                       assign temp [N-1] = g_i[N-1]; 
                       genvar i;
                       generate
                       for (i=N-2; 1>= 0; i = i-1)
                           begin 
                           assign temp(i) = temp(i+1)*g_i[1];
                           end
                           end generates
         Any individual bit of a vector can be selected and assigned to a new Var. 
                      Eg: reg [3:0] count;
                          count [3] = 1'b1; //assigned to 1 MSB 
                          count [2] = 1'b0; //assigned to 0 to bit no. 3
              Even some portion of vector can also be selected and assigned
                      Eg: reg [7:0] count;
                          count [6:4] =3'b110;
     -------------------------------------------------------------------------------------------------------------------------------                     
                           Array in Verilog
         A vector is a single element that is n bits wide but arrays are multiple elements that are 1 bit or n-bit wide.
         It is allowed for reg, integer, time and real data type.
               Eg: integer count [o:7] ; // array having 8 rows
                   integer [0:7] count; // Vector                                01234567 
                   integer matrix [2:0][3:0] // array                         2  [  |    |    |   ]
                                                                              1  [  |    |    |   ]
                                                                              0  [  |    |    |   ] 
                                                                                  3   2    1    0
                                                                                
                   reg [2:0] mem[0:3] //                                      3  [  |    |    ]
                                                                              2  [  |    |    ]
                                                                              1  [  |    |    ]      
                                                                              0  [  |    |    ]
                                                                                  2   1    0
                                                                                
                   mem [2] = 3'b110; //                                       0  [  |    |    ]
                                                                              1  [  |    |    ]
                                                                              2  [  |    |    ]
                                                                              3  [  |    |    ]
                                                                                  0   1    2
                                    R     C
                    reg [2:0] mem[0:2] [0: 2] // array
                    mem [0][0] = 3'b001;
                    mem [1][2] = 3'b0ll;
                    mem [2][1] = 3'bl01;
          ------------------------------------------------------------------------------------------------------------------------------------
                      Module in Verilog (stucture in Verilog)
          Module:
             This is the basic building blocks in verilog.It can be a single element or collection of lower design blocks.It hides internal Implementation.
                   Syntax: 
                   module <name of module> (<terminal portlist>);
                          <post declaration>
                          <functionality>
                   endmodule // no ( ; )  at the end
         ----Module and endmodule are Keyword
         ----Module represents the design that implements the certain behavioral char.
         ----All variable declaration,terminal port,functionality of design are defined within module and endmodule 
         ----We can include module within module is called module instantiation
         ----Module can be reused
                          Eg: module counter ();
                              _ _ _ _ _ _ _ _ _ _ 
                              _ _ _ _ _ _ _ _ _ _
                             end module
               ----------------------------------------------------------------------------------------------------------------------------------
           Port : 
                 Modules are connected by ports. A part can be input output or inout 
                 Same name not used for different ports.
                         Eg: module andgt(a, b,y);
                             input a;
                             input b; //input a, b;
                             output y; //output port
                             assign y = a & b; //gives result
                             end module
                          Eg : module andgt (input a,input b,output y);
                               assign y = a&b ; // given result
                               endmodule
                 Port are used to send or receive data from outside world.
                 
           Syntax:
                    input <net type> <rage> input port name;
                    inout <net type> <rage> inout port name;
                    output <net type> <range> output port name;
                Input - design module receives from output using 
                
                
                to be continue........
