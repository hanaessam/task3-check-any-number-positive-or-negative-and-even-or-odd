## Programing by Dart - Control Flow - Check any number positive or negative and even or odd



**Task General Description**

Check any number positive or negative and even or odd using conditions and  
different operators

**Requirement 1**

**Title:** Check any number positive or negative and even or odd  
**Description:** Enter any integer number  
Use the condition to check it's positive or negative, then  
use the condition to check if it's even or odd

    import 'dart:io';
    
    void main() {
      print('Enter an integer number:');
      int? number = int.tryParse(stdin.readLineSync() ?? '');
    
      if (number == null) {
        print('Invalid input. Please enter a valid integer.');
        return;
      }
    
      // Check if the number is positive or negative
      if (number > 0) {
        print('$number is positive.');
      } else if (number < 0) {
        print('$number is negative.');
      } else {
        print('$number is zero.');
      }
    
      // Check if the number is even or odd
      if (number % 2 == 0) {
        print('$number is even.');
      } else {
        print('$number is odd.');
      }
    }


**Screenshots of output**
![alt text](screenshot.png)
