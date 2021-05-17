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
            to be continue.... 
