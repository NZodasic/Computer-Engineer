***
#### Decimal System

- 10 digit: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
- Combine **multiple** digit to represent value higher than 9
	- Assign weight (10^{i}) to each digit in the string of numeric signatures
	- Represent 269 in decimal: $$\left(2\times10^2\right)+\left(6\times10^1\right)+\left(9\times10^0\right)=200+60+9=269$$
	- Represent 158 has 5 digit in decimal system is? ABCDE ?

$$158=Ax10^4+Bx10^3+Cx10^2+Dx10^1+Ex10^0$$
$$A = 0,B=0,C=1,D=5,E=8 \ ->00158$$
***
#### Binary System
- 2 digit: 0, 1
- Information unit is bit (binary digit)

| 1B | 8 bit
:--:|:--:
|1 KB| $1024B(2^{10}B)$|
|1 MB| $1024KB(2^{10}MB)$|
|1GB | $1024MB(2^{10}MB)$|
|1TB | $1024GB(2^{10}GB)$|
***
#### Positive Number(Unsigned Numbers)
- Represent unsigned numbers in bit array
	- Reverse proccess to count the value of unsigned number
		- Analyze unsigned numbers into sumary of 2 to the power of n
	- The power is the location that bit represent 1

**Example:23**
$$23=2^4+2^2+2^1+2^0$$

$2^4$$|$2^3$|$2^2$|$2^1$|$2^0$
:--:|:--:|:--:|:--:|:--:|
1|0|1|1|1
***
#### Hexadecimal system
**Converting table**

|Decimal System|0|1|2|3|4|5|6|7|
:--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:
|Binary System|0000|0001|0010|0011|0100|0101|0110|0111|
|Hexadecimal System|0|1|2|3|4|5|6|7|

|Decimal System|8|9|10|11|12|13|14|15|
:--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:
|Binary System|1000|1001|1010|1011|1100|1101|1110|1111|
|Hexadecimal System|8|9|10|A|B|C|D|E|

![[Pasted image 20231203160805.png]]
* * * 
- Each digit in hexadecimal correspond to 4 bit


$$2^{11}$$|$$2^{10}$$|$$2^{9}$$|$$2^{8}$$|$$2^{7}$$|$$2^{6}$$|$$2^{5}$$|$$2^{4}$$|$$2^{3}$$|$$2^{2}$$|$$2^{1}$$|$$2^{0}$$
:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:
0|0|1|0|1|1|1|0|1|0|0|1

<--------------><-----------><------------>
		    2                     E                     9

$$001011101001(2)=2E9=0x2E9$$
***
##### Two's complement method

* To perform general integer(Positive, 0 ,Negative)
	* Add 1 bit for sign (Sign and value): 0 is plus sign, 1 is minus sign.
	* ![[Pasted image 20231203163627.png]]
	* Easy to understand
	* To represen 0:
		* + 0
		* - 0
	- Operation to count 745 +(-745)
	- ![[Pasted image 20231203164535.png]]
* * *
### **BCD(Binary Coded Decimal)**

- Using 4 bit to decode a single digit of binary
|Decimal digit| Binary code|
:--:|:--: 
|0|0000
|1|0001
|2|0010
|3|0011
|4|0100
|5|0101
|6|0110
|7|0111
|8|1000
|9|1001
### Example

| Value | Binary | BCD |
:--:|:--:|:--:
4| 0100 | 0100
8| 1000 | 1000
10| 1010 | 0001_0000
15| 1111 | 0001_0101
16| 10000 | 0001_0110
25| 11001 | 0010_0101
31| 11111 | 0011_0001
32| 100000 | 0011_0010
99| 1100011 | 1001_1001
100| 1100100 | 0001_0000_0000
![[Pasted image 20231203170322.png]]
