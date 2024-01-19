# Roman-Nummeral-Converter
Convert the given number into a roman numeral.

Roman numerals	Arabic numerals
M	1000
CM	900
D	500
CD	400
C	100
XC	90
L	50
XL	40
X	10
IX	9
V	5
IV	4
I	1
All roman numerals answers should be provided in upper-case.


## Demo

https://mohicodings.github.io/Roman-Nummeral-Converter/

## Technologies Used
- JavaScript
- HTML
- CSS


## Acknowledgments
This project was developed as an Certification task for FreeCodeCamp- Javascript and Data Structure Certification.



## About Freecodecamp Certification 
FreeCodeCamp Roman Numeral conerter - JavaScript Algorithms and Data Structures Projects (https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/javascript-algorithms-and-data-structures-projects/roman-numeral-converter )


## Test cases

convertToRoman(2) should return the string II.

Waiting:convertToRoman(3) should return the string III.

Waiting:convertToRoman(4) should return the string IV.

Waiting:convertToRoman(5) should return the string V.

Waiting:convertToRoman(9) should return the string IX.

Waiting:convertToRoman(12) should return the string XII.

Waiting:convertToRoman(16) should return the string XVI.

Waiting:convertToRoman(29) should return the string XXIX.

Waiting:convertToRoman(44) should return the string XLIV.

Waiting:convertToRoman(45) should return the string XLV.

Waiting:convertToRoman(68) should return the string LXVIII

Waiting:convertToRoman(83) should return the string LXXXIII

Waiting:convertToRoman(97) should return the string XCVII

Waiting:convertToRoman(99) should return the string XCIX

Waiting:convertToRoman(400) should return the string CD

Waiting:convertToRoman(500) should return the string D

Waiting:convertToRoman(501) should return the string DI

Waiting:convertToRoman(649) should return the string DCXLIX

Waiting:convertToRoman(798) should return the string DCCXCVIII

Waiting:convertToRoman(891) should return the string DCCCXCI

Waiting:convertToRoman(1000) should return the string M

Waiting:convertToRoman(1004) should return the string MIV

Waiting:convertToRoman(1006) should return the string MVI

Waiting:convertToRoman(1023) should return the string MXXIII

Waiting:convertToRoman(2014) should return the string MMXIV

Waiting:convertToRoman(3999) should return the string MMMCMXCIX


## Solution

function convertToRoman(num) {
 var decimalValue = [1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4, 1];
  var romanNumeral = ['M', 'CM', 'D', 'CD', 'C', 'XC', 'L', 'XL', 'X', 'IX', 'V', 'IV', 'I'];

  var romanized = "";

  for (var index = 0; index < decimalValue.length; index++) {
    while (decimalValue[index] <= num) {
      romanized += romanNumeral[index];
      num -= decimalValue[index];
    }
  }

  return romanized;
};

convertToRoman(36);
  


