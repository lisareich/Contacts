# Contacts
## Description
A program to create contacts (like on the mobile phone) and search for people or organizations by name.   
## Features
- Command pattern
- Regexps
- Java Reflection API
- Java I/O Streams  
## Running the project
To run the program you will need The Java Development Kit (JDK) installed.

To run the program from CMD:

  1. Open CMD and go to ./Contacts/task/src/contacts/
  2. Compile the Java code: ./Contacts/task/src/contacts javac *.java
  3. Change directory to ./Contacts: cd ../../..
  4. Run the program: ./Contacts java -cp task\src contacts.Main

## Usage
**Example 1**   

The symbol ```>``` represents the user input.
```
Enter action (add, remove, edit, count, info, exit): > add
Enter the type (person, organization): > person
Enter the name: > John
Enter the surname: > Smith
Enter the birth date: >
Bad birth date!
Enter the gender (M, F): >
Bad gender!
Enter the number: > +0 (123) 456-789-ABcd
The record added.

Enter action (add, remove, edit, count, info, exit): > add
Enter the type (person, organization): > organization
Enter the organization name: > Pizza Shop
Enter the address: > Wall St. 1
Enter the number: > +0 (123) 456-789-9999
The record added.

Enter action (add, remove, edit, count, info, exit): > info
1. John Smith
2. Pizza Shop
Enter index to show info: > 2
Organization name: Pizza shop
Address: Wall St. 1
Number: +0 (123) 456-789-9999
Time created: 2018-01-01T00:00
Time last edit: 2018-01-01T00:00

Enter action (add, remove, edit, count, info, exit): > edit
1. John Smith
2. Pizza Shop
Select a record: > 1
Select a field (name, surname, birth, gender, number): > number
Enter number: > (123) 234 345-456
The record updated!

Enter action (add, remove, edit, count, info, exit): > info
1. John Smith
2. Pizza Shop
Select a record: > 1
Name: John
Surname: Smith
Birth date: [no data]
Gender: [no data]
Number: (123) 234 345-456
Time created: 2018-01-01T00:00
Time last edit: 2018-01-01T00:01

Enter action (add, remove, edit, count, info, exit): > edit
1. John Smith
2. Pizza Shop
Select a record: > 2
Select a field (address, number): > address
Enter address: > Wall St. 7
The record updated!

Enter action (add, remove, edit, count, info, exit): > info
1. John Smith
2. Pizza Shop
Enter index to show info: > 2
Organization name: Pizza shop
Address: Wall St. 7
Number: +0 (123) 456-789-9999
Time created: 2018-01-01T00:00
Time last edit: 2018-01-01T00:02

Enter action (add, remove, edit, count, info, exit): > exit
```  
**Example 2**  

The symbol ```>``` represents the user input.
```
open phonebook.db

[menu] Enter action (add, list, search, count, exit): > count
The Phone Book has 6 records.

[menu] Enter action (add, list, search, count, exit): > search
Enter search query: > cent
Found 3 results:
1. Central Bank
2. Centurion Adams
3. Decent Pizza Shop

[search] Enter action ([number], back, again): > again
Enter search query: > shop
Found 2 results:
1. Decent Pizza Shop
2. Car shop

[search] Enter action ([number], back, again): > 2
Organization name: Car shop
Address: Wall St. 3
Number: +0 (123) 456-789-9999
Time created: 2018-01-01T00:03
Time last edit: 2018-04-29T11:34

[record] Enter action (edit, delete, menu): > edit
Select a field (name, address, number): > name
Enter name: > New Car Shop
Saved
Organization name: New Car Shop
Address: Wall St. 3
Number: +0 (123) 456-789-9999
Time created: 2018-01-01T00:03
Time last edit: 2018-11-20T11:04

[record] Enter action (edit, delete, menu): > menu

[menu] Enter action (add, list, search, count, exit): > search
Enter search query: > new
Found 1 result:
1. New Car Shop

[search] Enter action ([number], back, again): > back

[menu] Enter action (add, list, search, count, exit): > list
1. New Car Shop
2. Decent Pizza Shop
3. Central Bank
4. Centurion Adams
5. John Smith
6. Alice Wonderlanded

[list] Enter action ([number], back): > 6
Name: Alice
Surname: Wonderlanded
Birth date: [no data]
Gender: F
Number: +123123 (123) 12-23-34-45
Time created: 2018-03-12T11:21
Time last edit: 2018-03-12T11:21

[record] Enter action (edit, delete, menu): > edit
Select a field (name, surname, birth, gender, number): > number
Enter number: > +23 (321) 12-12 12 12
Saved
Name: Alice
Surname: Wonderlanded
Birth date: [no data]
Gender: F
Number: +23 (321) 12-12 12 12
Time created: 2018-03-12T11:21
Time last edit: 2018-11-20T11:07

[record] Enter action (edit, delete, menu): > menu

[menu] Enter action (add, list, search, count, exit): > exit
```
## Additional info
To find more about this project, please visit https://hyperskill.org/projects/43.


