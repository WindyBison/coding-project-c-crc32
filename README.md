# Windy Bison CRC32 Coding Project

## Windy Bison Coding Projects
<https://windybison.net/codingprojects.html>

## A Coding Project for the CRC32 Algorithm Written in C

This code is intended to be a practical implementation of the CRC32 algorithm for learning purposes

### The CRC32 Polynomial for this implementation:
>x32 + x26 + x23 + x22 + x16 + x12 + x11 + x10 + x8 + x7 + x5 + x4 + x2 + x + 1

Which can can also be represented as:
>0x04C11DB7

and inverted:
>0xEDB88320

### Running the code

1. Create a directory
2. Place windybisoncrc32.c and any files wanted for generating a CRC32 in the directory
3. Compile windybisoncrc32.c
4. Use the generated executable and pass the filename as the argument

Example Output:
>windybisoncrc32.exe TestFile.txt

>Reading File: TestFile.txt</br> 
>Total Size of File: 79 bytes</br>
>CRC32 of file is: 78c77a6b

### Possible Errors
- Having the input file locked\open by another program will cause errors on fopen
- Allocating the file into memory will be dependent on how much system memory is available
- File sizes larger than the value of an unsigned long long would probably break the code or give unintended results. Use appropriately sized files