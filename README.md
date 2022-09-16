# AES_and_DES
## Intro
Data Encryption Standard (DES) and Advanced Encryption Standard (AES) implementation.
## Setting  
I use Crypto++ 8.6 version for this two cryptography algorithm, 
So you need to download this library from https://cryptopp.com/release860.html first and put it where you put all your library.  
  
If you use Microsoft Visual Studio as your IDE, you can follow this three step to set up:  
1. copy whole cryptopp860 dir to this project
2. In "Solution Explorer", right click your project, choose "Propertys"  
  &emsp;- In "C/C++", choose "Code Generation", change Runtime Library to "MTd"  
  &emsp;- In "C/C++", choose "General", add a path -the path of your ...\Crypto++\cryptopp860 file- into include library  
  &emsp;- In "Linker", add a path -the path of your ...\Crypto++\cryptopp860\Win32\Output\Debug\cryptlib.lib file- into AdditionalDependencies    
3. try this simple code to test if you are success
      ```c++
      #include "cryptopp860/aes.h"
      using namespace std;
      using namespace  CryptoPP;//這個不要忘記加ㄟ，不然你AES::不能用
      int main() {
        return 0;
      }
      ```
4.  If this still not work, follow this youtube video : https://www.youtube.com/watch?v=fDvbE7LQDqE
