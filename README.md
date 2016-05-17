# my_lessons
my_lessons
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package exmples;

/**
 *
 * @author huang
 */
class Box {
    double width;
    double height;
    double depth;
}
public class Exmples {

    /**
     * @param args the command line arguments
     */
    
    

    public static void main(String[] args) throws java.io.IOException{
        int num; // this declares a variable called num
        System.out.println("This is a simple Java program.");
        num = 100; // this assigns num the value 100
        System.out.println("This is num: " + num);
        num = num * 2;
        System.out.print("The value of num * 2 is ");
        System.out.println(num);
        //*******************************************
        int x, y;
        x = 10;
        y = 20;
        if(x < y) System.out.println("x is less than y");
            x = x * 2;
        if(x == y) System.out.println("x now equal to y");
            x = x * 2;
        if(x > y) System.out.println("x now greater than y");
        // this won't display anything
        if(x == y) System.out.println("you won't see this");
        //*******************************************
        int xy;
        for(xy = 0; xy<10; xy = xy+1)
            System.out.println("This is xy: " + xy);
        
        
        //*******************************************
        int xz, yz;
        yz = 20;
        // the target of this loop is a block
        for(xz = 0; xz<10; xz++) {
        System.out.println("This is xz: " + xz);
        System.out.println("This is yz: " + yz);
        yz = yz - 2;}
        //*******************************************
        
        
        int lightspeed;
        long days;
        long seconds;
        long distance;
        // approximate speed of light in miles per second
        lightspeed = 186000;
        days = 1000; // specify number of days here
        seconds = days * 24 * 60 * 60; // convert to seconds
        distance = lightspeed * seconds; // compute distance
        System.out.print("In " + days);
        System.out.print(" days light will travel about ");
        System.out.println(distance + " miles.");
        //*******************************************
        double pi, r, a;
        r = 10.8; // radius of circle
        pi = 3.1416; // pi, approximately
        a = pi * r * r; // compute area
        System.out.println("Area of circle is " + a);
        //*******************************************
        char ch1, ch2;
        ch1 = 88; // code for X
        ch2 = 'Y';
        System.out.print("ch1 and ch2: ");
        System.out.println(ch1 + " " + ch2);
        //*******************************************
        char chy;
        chy = 'X';
        System.out.println("chy contains " + chy);
        chy++; // increment chy
        System.out.println("chy is now " + chy);
        //*******************************************
        boolean b;
        b = false;
        System.out.println("b is " + b);
        b = true;
        System.out.println("b is " + b);
        // a boolean value can control the if statement
        if(b) System.out.println("This is executed.");
            b = false;
        if(b) System.out.println("This is not executed.");
        // outcome of a relational operator is a boolean value
        System.out.println("10 > 9 is " + (10 > 9));  
        //*******************************************
        double numx = 9_423_497_862.0;
        //*******************************************
        double aa = 3.0, ba = 4.0;
        // c is dynamically initialized
        double ca = Math.sqrt(aa * aa + ba * ba);
        System.out.println("Hypotenuse is " + ca);
        //*******************************************
        int xa; // known to all code within main
        xa = 10;
        if(xa == 10) { // start new scope
        int ya = 20; // known only to this block
        // xa and ya both known here.
        System.out.println("xa and ya: " + xa + " " + ya);
        xa = ya * 2;
        }
        // ya = 100; // Error! y not known here
        // xa is still known here.
        System.out.println("xa is " + xa);
        //go to page 46
        
        int x1;
        for(x1 = 0; x1 < 3; x1++) {
        int y1 = -1; // y is initialized each time block is entered
        System.out.println("y1 is: " + y1); // this always prints -1
        y1 = 100;
        System.out.println("y1 is now: " + y1);}
        
        //next code
        byte b1;
        int i = 257;
        double d = 323.142;
        System.out.println("\nConversion of int to byte.");
        b1 = (byte) i;
        System.out.println("i and b1 " + i + " " + b1);
        System.out.println("\nConversion of double to int.");
        i = (int) d;
        System.out.println("d and i " + d + " " + i);
        System.out.println("\nConversion of double to byte.");
        b1 = (byte) d;
        System.out.println("d and b " + d + " " + b1);
        //type promotion
        byte a2 = 40;
        byte b2 = 50;
        byte c2 = 100;
        int d2 = a2 * b2 / c2;
        System.out.println(d2);
        //more
        byte b3 = 42;
        char c3 = 'a';
        short s3 = 1024;
        int i3 = 50000;
        float f3 = 5.67f;
        double d3 = .1234;
        double result = (f3 * b3) + (i3 / c3) - (d3 * s3);
        System.out.println((f3 * b3) + " + " + (i3 / c3) + " - " + (d3 * s3));
        System.out.println("result = " + result);
        //
        int month_days[];
            month_days = new int[12];
            month_days[0] = 31;
            month_days[1] = 28;
            month_days[2] = 31;
            month_days[3] = 30;
            month_days[4] = 31;
            month_days[5] = 30;
            month_days[6] = 31;
            month_days[7] = 31;
            month_days[8] = 30;
            month_days[9] = 31;
            month_days[10] = 30;
            month_days[11] = 31;
        System.out.println("April has " + month_days[3] + " days.");
        //autoarray
        int month_days1[] = { 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31 };
        System.out.println("April has " + month_days1[3] + " days.");
        //
        double nums1[] = {10.1, 11.2, 12.3, 13.4, 14.5};
        double result1 = 0;
        int i1;
        for(i1=0; i1<5; i1++)
            result1 = result1 + nums1[i1];
        System.out.println("Average is " + result1 / 5);
        //
        int twoD[][]= new int[4][5];
        int i4, j, k = 0;
        for(i4=0; i4<4; i4++)
            for(j=0; j<5; j++) {
                twoD[i4][j] = k;
        k++;
        }
        for(i4=0; i4<4; i4++) {
            for(j=0; j<5; j++)
                System.out.print(twoD[i4][j] + " ");
            System.out.println();
                            }
        //
        int twoDD[][] = new int[4][];
            twoDD[0] = new int[1];
            twoDD[1] = new int[2];
            twoDD[2] = new int[3];
            twoDD[3] = new int[4];
        int icount, jcount, kcount = 0;
        for(icount = 0; icount <4; icount++)
            for(jcount = 0; jcount < icount+1; jcount++) {
                twoDD[icount][jcount] = kcount;
                kcount++;
             }
                for(icount=0; icount<4; icount++) {
                for(jcount=0; jcount<icount+1; jcount++)
                    System.out.print(twoDD[icount][jcount] + " ");
                System.out.println();
            }   
                
          // Initialize a two-dimensional array.
         double m[][] = {
            { 0*0, 1*0, 2*0, 3*0 },
            { 0*1, 1*1, 2*1, 3*1 },
            { 0*2, 1*2, 2*2, 3*2 },
            { 0*3, 1*3, 2*3, 3*3 } 
             };
            int ixxx, jxxx;
            for(ixxx=0; ixxx<4; ixxx++) {
                for(jxxx=0; jxxx<4; jxxx++)
                    System.out.print(m[ixxx][jxxx] + " ");
                System.out.println();
                }
            //
            int threeDyyy[][][] = new int[3][4][5];
            int iyyy, jyyy, kyyy;
            for(iyyy = 0; iyyy < 3; iyyy++)
                for(jyyy = 0; jyyy < 4; jyyy++)
                    for(kyyy = 0; kyyy < 5; kyyy++)
                        threeDyyy[iyyy][jyyy][kyyy] = iyyy * jyyy * kyyy;
            for(iyyy = 0; iyyy < 3; iyyy++) {
               for(jyyy = 0; jyyy < 4; jyyy++) {
                  for(kyyy = 0; kyyy < 5; kyyy++)
                     System.out.print(threeDyyy[iyyy][jyyy][kyyy] + " ");
                           System.out.println();
                    }
                    System.out.println();
        }//page 58
          // arithmetic using integers
System.out.println("Integer Arithmetic");
int a_opex = 1 + 1;
int b_opex = a_opex * 3;
int c_opex = b_opex / 4;
int d_opex = c_opex - a_opex;
int e_opex = -d_opex;
System.out.println("a_opex = " + a_opex);
System.out.println("b_opex = " + b_opex);
System.out.println("c_opex = " + c_opex);
System.out.println("d_opex = " + d_opex);
System.out.println("e_opex = " + e_opex);
// arithmetic using doubles
System.out.println("\nFloating Point Arithmetic");
double da_opex = 1 + 1;
double db_opex = da_opex * 3;
double dc_opex = db_opex / 4;
double dd_opex = dc_opex - a_opex;
double de_opex = -dd_opex;
System.out.println("da_opex = " + da_opex);
System.out.println("db_opex = " + db_opex);
System.out.println("dc_opex = " + dc_opex);
System.out.println("dd_opex = " + dd_opex);
System.out.println("de_opex = " + de_opex);  

//******************************************
int x_modulus_example = 42;
double y_modulus_example = 42.25;
System.out.println("x_modulus_example mod 10 = " + x_modulus_example % 10);
System.out.println("y_modulus_example mod 10 = " + y_modulus_example % 10); 

//page 64 demonstrate several assignment operators
int a_OpEquals = 1;
int b_OpEquals = 2;
int c_OpEquals = 3;
a_OpEquals += 5;
b_OpEquals *= 4;
c_OpEquals += a_OpEquals * b_OpEquals;
c_OpEquals %= 6;
System.out.println("a_OpEquals = " + a_OpEquals);
System.out.println("b_OpEquals = " + b_OpEquals);
System.out.println("c_OpEquals = " + c_OpEquals);

//_incrementor page 65
int a_incrementor = 1;
int b_incrementor = 2;
int c_incrementor;
int d_incrementor;
c_incrementor = ++b_incrementor;
d_incrementor = a_incrementor++;
c_incrementor++;
System.out.println("a_incrementor = " + a_incrementor);
System.out.println("b_incrementor = " + b_incrementor);
System.out.println("c_incrementor = " + c_incrementor);
System.out.println("d_incrementor = " + d_incrementor);

//_bitwise operators
String binary_bitwise[] = {
"0000", "0001", "0010", "0011", "0100", "0101", "0110", "0111",
"1000", "1001", "1010", "1011", "1100", "1101", "1110", "1111"
};
int a_bitwise = 3; // 0 + 2 + 1 or 0011 in binary
int b_bitwise = 6; // 4 + 2 + 0 or 0110 in binary
int c_bitwise = a_bitwise | b_bitwise;
int d_bitwise = a_bitwise & b_bitwise;
int e_bitwise = a_bitwise ^ b_bitwise;
int f_bitwise = (~a_bitwise & b_bitwise)|(a_bitwise & ~b_bitwise);
int g_bitwise = ~a_bitwise & 0x0f;
System.out.println(" a_bitwise = " + binary_bitwise[a_bitwise]);
System.out.println(" b_bitwise = " + binary_bitwise[b_bitwise]);
System.out.println(" a_bitwise|b_bitwise = " + binary_bitwise[c_bitwise]);
System.out.println(" a_bitwise&b_bitwise = " + binary_bitwise[d_bitwise]);
System.out.println(" a_bitwise^b_bitwise = " + binary_bitwise[e_bitwise]);
System.out.println("~a_bitwise&b_bitwise|a_bitwise&~b_bitwise = " 
        + binary_bitwise[f_bitwise]);
System.out.println(" ~a_bitwise = " + binary_bitwise[g_bitwise]);

//the _left_shift
byte a_left_shift = 64, b_left_shift;
int i_left_shift;
i_left_shift = a_left_shift << 2;
b_left_shift = (byte) (a_left_shift << 2);
System.out.println("Original value of a_left_shift: " + a_left_shift);
System.out.println("i_left_shift and b_left_shift: " + i_left_shift 
        + " " + b_left_shift);
//Left shifting as a quick way to multiply by 2.
int i_MultByTwo;
int num_MultByTwo = 0xFFFFFFE;
for(i_MultByTwo=0; i_MultByTwo<4; i_MultByTwo++) {
num_MultByTwo = num_MultByTwo << 1;
System.out.println(num_MultByTwo);}

//Masking sign extension.
char hex_HexByte[] = {
'0', '1', '2', '3', '4', '5', '6', '7',
'8', '9', 'a', 'b', 'c', 'd', 'e', 'f'
};
byte b_HexByte = (byte) 0xf1;
System.out.println("b_HexByte = 0x" + hex_HexByte[(b_HexByte >> 4) & 0x0f] 
        + hex_HexByte[b_HexByte & 0x0f]);

//page 72 Unsigned shifting a byte value.
char hex_ByteUShift[] = {
'0', '1', '2', '3', '4', '5', '6', '7',
'8', '9', 'a', 'b', 'c', 'd', 'e', 'f'
};
byte b_ByteUShift = (byte) 0xf1;
byte c_ByteUShift = (byte) (b_ByteUShift >> 4);
byte d_ByteUShift = (byte) (b_ByteUShift >>> 4);
byte e_ByteUShift = (byte) ((b_ByteUShift & 0xff) >> 4);
System.out.println(" b_ByteUShift = 0x"
+ hex_ByteUShift[(b_ByteUShift >> 4) & 0x0f] 
        + hex_ByteUShift[b_ByteUShift & 0x0f]);
System.out.println(" b_ByteUShift >> 4 = 0x"
+ hex_ByteUShift[(c_ByteUShift >> 4) & 0x0f] 
        + hex_ByteUShift[c_ByteUShift & 0x0f]);
System.out.println(" b_ByteUShift >>> 4 = 0x"
+ hex_ByteUShift[(d_ByteUShift >> 4) & 0x0f] 
        + hex_ByteUShift[d_ByteUShift & 0x0f]);
System.out.println("(b_ByteUShift & 0xff) >> 4 = 0x"
+ hex_ByteUShift[(e_ByteUShift >> 4) & 0x0f] 
        + hex_ByteUShift[e_ByteUShift & 0x0f]);

//page 76 _Bitwise_Operator Compound Assignments
int a_Bitwise_Operator = 1;
int b_Bitwise_Operator = 2;
int c_Bitwise_Operator = 3;
a_Bitwise_Operator |= 4;
b_Bitwise_Operator >>= 1;
c_Bitwise_Operator <<= 1;
a_Bitwise_Operator ^= c_Bitwise_Operator;
System.out.println("a_Bitwise_Operator = " + a_Bitwise_Operator);
System.out.println("b_Bitwise_Operator = " + b_Bitwise_Operator);
System.out.println("c_Bitwise_Operator = " + c_Bitwise_Operator);

//_Relational Operators
boolean a_Relational = true;
boolean b_Relational = false;
boolean c_Relational = a_Relational | b_Relational;
boolean d_Relational = a_Relational & b_Relational;
boolean e_Relational = a_Relational ^ b_Relational;
boolean f_Relational = (!a_Relational & b_Relational) | (a_Relational & !b_Relational);
boolean g_Relational = !a_Relational;
System.out.println(" a_Relational = " + a_Relational);
System.out.println(" b_Relational = " + b_Relational);
System.out.println(" a_Relational|b_Relational = " + c_Relational);
System.out.println(" a_Relational&b_Relational = " + d_Relational);
System.out.println(" a_Relational^b_Relational = " + e_Relational);
System.out.println("!a_Relational&b_Relational|a_Relational&!b_Relational = " + f_Relational);
System.out.println(" !a_Relational = " + g_Relational);

//The ? Operator _question
int i_question, k_question;
i_question = 10;
k_question = i_question < 0 ? -i_question : i_question; // get absolute value of i
System.out.print("Absolute value of ");
System.out.println(i_question + " is " + k_question);
i_question = -10;
k_question = i_question < 0 ? -i_question : i_question; // get absolute value of i
System.out.print("Absolute value of ");
System.out.println(i_question + " is " + k_question);

// chapter 5 control statements page 81
int month = 4; // April
String season;
if(month == 12 || month == 1 || month == 2)
season = "Winter";
else if(month == 3 || month == 4 || month == 5)
season = "Spring";
else if(month == 6 || month == 7 || month == 8)
season = "Summer";
else if(month == 9 || month == 10 || month == 11)
season = "Autumn";
else
season = "Bogus Month";
System.out.println("April is in the " + season + ".");

//page 85 control statements _switch
for(int i_switch=0; i_switch<6; i_switch++)
switch(i_switch) {
case 0:
System.out.println("i is zero.");
break;
case 1:
System.out.println("i is one.");
break;
case 2:
System.out.println("i is two.");
break;
case 3:
System.out.println("i is three.");
break;
default:
System.out.println("i is greater than 3.");}

// page 86 _switch2
for(int i_switch2=0; i_switch2<12; i_switch2++)
switch(i_switch2) {
case 0:
case 1:
case 2:
case 3:
case 4:
System.out.println("i_switch2 is less than 5");
break;
case 5:
case 6:
case 7:
case 8:
case 9:
System.out.println("i_switch2 is less than 10");
break;
default:
System.out.println("i_switch2 is 10 or more");
}
// page 86 part II _switch3
String season_switch3;
int month_switch3 = 4;
switch (month_switch3) {
case 12:
case 1:
case 2:
season_switch3 = "Winter";
break;
case 3:
case 4:
case 5:
season_switch3 = "Spring";
break;
case 6:
case 7:
case 8:
season_switch3 = "Summer";
break;
case 9:
case 10:
case 11:
season_switch3 = "Autumn";
break;
default:
season_switch3 = "Bogus Month";
}
System.out.println("April is in the " + season_switch3 + ".");

//page 87

String str = "two";
switch(str) {
case "one":
System.out.println("one");
break;
case "two":
System.out.println("two");
break;
case "three":
System.out.println("three");
break;
default:
System.out.println("no match");
break;
}

// page 88
/*
switch(count) {
case 1:
switch(target) { // nested switch
case 0:
System.out.println("target is zero");
break;
case 1: // no conflicts with outer switch
System.out.println("target is one");
break;
}
break;
case 2: // ...
*/

//pg 90 _while
int i_while, j_while;
i_while = 100;
j_while = 200;
// find midpoint between i and j
while(++i_while < --j_while); // no body in this loop
System.out.println("Midpoint is " + i_while);

//pg 91 Demonstrate the do-while loop.
int n = 10,n_ext=19;
do {
System.out.println("tick " + n_ext+" !");
n_ext++;
} while(n_ext < 100);
// more efficient
do {
System.out.println("tick " + n);
} while(--n > 0);
// Using a do-while to process a menu selection
 
char choice;
do {
System.out.println("Help on: ");
System.out.println(" 1. if");
System.out.println(" 2. switch");
System.out.println(" 3. while");
System.out.println(" 4. do-while");
System.out.println(" 5. for\n");
System.out.println("Choose one:");
choice = (char) System.in.read();
} while( choice < '1' || choice > '5');
System.out.println("\n");
switch(choice) {
case '1':
System.out.println("The if:\n");
System.out.println("if(condition) statement;");
System.out.println("else statement;");
break;
case '2':
System.out.println("The switch:\n");
System.out.println("switch(expression) {");
System.out.println(" case constant:");
System.out.println(" statement sequence");
System.out.println(" break;");
System.out.println(" //...");
System.out.println("}");
break;
case '3':
System.out.println("The while:\n");
System.out.println("while(condition) statement;");
break;
case '4':
System.out.println("The do-while:\n");
System.out.println("do {");
System.out.println(" statement;");
System.out.println("} while (condition);");
break;
case '5':
System.out.println("The for:\n");
System.out.print("for(init; condition; iteration)");
System.out.println(" statement;");
break;
}
//pg_93 demonstration of the for loop
int npg_93;
for(npg_93=10; npg_93>0; npg_93--)
System.out.println("tick " + npg_93);
//_pg_94 Declare a loop control variable inside the for.
// here, n is declared inside of the for loop
    for(int n_pg_94=10; n_pg_94>0; n_pg_94--)
        System.out.println("tick " + n_pg_94);

// Test for_primes.
    int num_for_primes;
    boolean isPrime;
    num_for_primes = 14;
    if(num_for_primes < 2) isPrime = false;
    else isPrime = true;
    for(int i_for_primes=2; i_for_primes <= num_for_primes/i_for_primes; i_for_primes
        ++) {
    if((num_for_primes % i_for_primes) == 0) {
    isPrime = false;
    break;
    }
    }
    if(isPrime) System.out.println("Prime");
    else System.out.println("Not Prime");

//pg_95
int a_pg_95, b_pg_95;
b_pg_95 = 4;
for(a_pg_95=1; a_pg_95<b_pg_95; a_pg_95++) {
System.out.println("a = " + a_pg_95);
System.out.println("b = " + b_pg_95);
b_pg_95--;
}
//Using the comma. _comma
int a_comma, b_comma;
for(a_comma=1, b_comma=4; a_comma<b_comma; a_comma++, b_comma--) {
System.out.println("a_comma = " + a_comma);
System.out.println("b_comma = " + b_comma);
}

//pg 96 Some for Loop Variations _SFLV
int i_SFLV;
boolean done_SFLV = false;
i_SFLV = 0;
for( ; !done_SFLV; ) {
System.out.println("i_SFLV is " + i_SFLV);
if(i_SFLV == 10) done_SFLV = true;
i_SFLV++;
}
//pg 98 use a for-each style for loop. _UFFES
int nums_UFFES[] = { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };
int sum_UFFES = 0;
// use for-each style for to display and sum the values
for(int x_UFFES : nums_UFFES) {
System.out.println("Value is: " + x_UFFES);
sum_UFFES += x_UFFES;
}
System.out.println("Summation: " + sum_UFFES);

//Use break with a for-each style for. _UseNWFESF
int sum_UseNWFESF = 0;
int nums_UseNWFESF[] = { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };
// use for to display and sum the values
for(int x_UseNWFESF : nums_UseNWFESF) {
System.out.println("Value is: " + x_UseNWFESF);
sum_UseNWFESF += x_UseNWFESF;
if(x_UseNWFESF == 5) break; // stop the loop when 5 is obtained
}
System.out.println("Summation of first 5 elements: " + sum_UseNWFESF);

//pg 99 The for-each loop is essentially read-only. _P99FELERO
int nums_P99FELERO[] = { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };
for(int x_P99FELERO: nums_P99FELERO) {
System.out.print(x_P99FELERO + " ");
x_P99FELERO = x_P99FELERO * 10; // no effect on nums
}
System.out.println();
for(int x_P99FELERO : nums_P99FELERO)
System.out.print(x_P99FELERO + " ");
System.out.println();

//pg 100 Iterating Over Multidimensional Arrays
// Use for-each style for on a two-dimensional array. _U4ES2D
int sum_U4ES2D = 0;
int nums_U4ES2D[][] = new int[3][5];
// give nums some values
for(int i_U4ES2D = 0; i_U4ES2D < 3; i_U4ES2D++)
for(int j_U4ES2D = 0; j_U4ES2D < 5; j_U4ES2D++)
nums_U4ES2D[i_U4ES2D][j_U4ES2D] = (i_U4ES2D+1)*(j_U4ES2D+1);
// use for-each for to display and sum the values
    for(int x_U4ES2D[] : nums_U4ES2D) {
        for(int y_U4ES2D : x_U4ES2D) {
            System.out.println("Value is: " + y_U4ES2D);
            sum_U4ES2D += y_U4ES2D;
        }
    }
System.out.println("Summation: " + sum_U4ES2D);

//pg 101 Applying the Enhanced for
// Search an array using for-each style for. _pg101
int nums_pg101[] = { 6, 8, 3, 7, 5, 6, 1, 4 };
int val_pg101 = 5;
boolean found_pg101 = false;
// use for-each style for to search nums for val
for(int x_pg101 : nums_pg101) {
    if(x_pg101 == val_pg101) {
    found_pg101 = true;
break;
    }
}
if(found_pg101)
    System.out.println("Value found_pg101!");

//page 102 nested loops. loops may be nested. _pg102
int i_pg102, j_pg102;
for(i_pg102=0; i_pg102<10; i_pg102++) {
for(j_pg102=i; j_pg102<10; j_pg102++)
System.out.print("r");
System.out.println();
}

//_pg103 using break to exit a loop

for(int i_pg103=0; i_pg103<100; i_pg103++) {
if(i_pg103 == 10) break; // terminate loop if i is 10
System.out.println("i_pg103: " + i_pg103);
}
System.out.println("Loop complete.");

// Using break to exit a while loop.
//_break_while_loop
int i_break_while_loop = 0;
while(i_break_while_loop < 100) {
if(i_break_while_loop == 10) break; // terminate loop if i is 10
System.out.println("i_break_while_loop: " + i_break_while_loop);
i_break_while_loop++;
}
System.out.println("Loop complete.");

//_pg104
for(int i_pg104=0; i_pg104<3; i_pg104++) {
System.out.print("Pass " + i_pg104 + ": ");
for(int j_pg104=0; j_pg104<100; j_pg104++) {
if(j_pg104 == 10) break; // terminate loop if j is 10
System.out.print(j_pg104 + " ");
}
System.out.println();
}
System.out.println("Loops complete.");

//_pg105 Using break as a civilized form of goto.
boolean t = true;
first: {
second: {
third: {
System.out.println("Before the break.");
if(t) break second; // break out of second block
System.out.println("This won't execute");
}
System.out.println("This won't execute");
}
System.out.println("This is after second block.");
}

//_pg105 Using break to exit from nested loops
outer: for(int i_pg105=0; i_pg105<3; i_pg105++) {
System.out.print("Pass " + i_pg105 + ": ");
for(int j_pg105=0; j_pg105<100; j_pg105++) {
if(j_pg105 == 10) break outer; // exit both loops
System.out.print(j_pg105 + " ");
}
System.out.println("This will not print");
}
System.out.println("Loops complete. _pg105");

//_pg106 This program contains an error.
/*one: for(int i_pg106=0; i_pg106<3; i_pg106++) {
System.out.print("Pass_pg106 " + i_pg106 + ": ");
}
for(int j_pg106=0; j_pg106<100; j_pg106++) {
if(j_pg106 == 10) break one; // WRONG
System.out.print(j_pg106 + " ");
}*/

// _pg106_107 using continue
// Demonstrate continue.
for(int i_pg106_107=0; i_pg106_107<10; i_pg106_107++) {
System.out.print(i_pg106_107 + " ");
if (i_pg106_107%2 == 0) continue;
System.out.println("");
}

//_pg107 Using continue with a label.
outer: for (int i_pg107=0; i_pg107<10; i_pg107++) {
for(int j_pg107=0; j_pg107<10; j_pg107++) {
if(j_pg107 > i_pg107) {
System.out.println();
continue outer;
}
System.out.print(" " + (i_pg107 * j_pg107));
}
}
System.out.println();

//_pg108 return
// demonstrate return.
/*boolean t_pg108 = true;
System.out.println("Before the return._pg108");
if(t_pg108) return; // return to caller
System.out.println("This won't execute._pg108");*/

//_pg111 chapter 6 introducing classes

Box mybox = new Box();
double vol;
// assign values to mybox's instance variables
    mybox.width = 10;
    mybox.height = 20;
    mybox.depth = 15;
// compute volume of box
vol = mybox.width * mybox.height * mybox.depth;
System.out.println("Volume is " + vol);

//_pg112


System.out.println("Can I see this?");

//_pg112 this program declares two box objects

Box mybox1 = new Box();
Box mybox2 = new Box();
double vol_pg112;
// assign values to mybox1's instance variables
mybox1.width = 10;
mybox1.height = 20;
mybox1.depth = 15;
/* assign different values to mybox2's
instance variables */
mybox2.width = 3;
mybox2.height = 6;
mybox2.depth = 9;
// compute volume of first box
vol_pg112 = mybox1.width * mybox1.height * mybox1.depth;
System.out.println("Volume_pg112 is " + vol_pg112);
// compute volume of second box
vol_pg112 = mybox2.width * mybox2.height * mybox2.depth;
System.out.println("Volume_pg112 is " + vol_pg112);

//_pg113 declaring objects

    }
   
}
