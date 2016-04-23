# RSAroutines

To build the program please run the following command

    $ g++ BigInt.cpp RSA.cpp hm6.cpp -o hm6

To Execute the program
    $./hm6

-----------------------------------------------------------------------

<<<<<<< HEAD
Observations:
1.
-We found that all the non prime numbers above 30,000 were unsuccessful in running RSA.

    if we select a number n=p x q where p,q are both prime, we will have selected a number we can factor but, if it is large enough, no one else can factor. The reason for this is because, using known factorization algorithms for arbitrary integers, the running time of such algorithms depends on the relative size of the second largest prime factor of the input. This means that given the public exponent e only you can determine the private exponent d.

2.
-Challenge response scheme worked on the 16 bit random numbers which were generated.

3.
-Blind signature worked on the 16 bit random numbers.
=======
>>>>>>> 571c990358d959646cff8cf9677b14233f3b5e8e

--------------------------------------------------------------------------

Sample run hm6 : ( we have used time delay so that the same random number is not generated by the generator)

Shrirangs-MacBook-Pro:HM6 shrirang$ ./hm6

1)------------------Encryption and Decryption using RSA----------------------
a) 10 instances of RSA routine(argument-less) encryption-decryption

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

Message: 0x0A99 986D 		Encrypted: 0x0002 A3F5 3034 		Decrypted: 0x0A99 986D

b) 5 RSA instances(1 prime number(>30,000) as argument) encryption-decryption

Message: 0x257F 009A 		Encrypted: 0xF48D 7388 		Decrypted: 0x257F 009A

Message: 0x03C9 BB64 		Encrypted: 0xB8D5 C8F0 		Decrypted: 0x03C9 BB64

Message: 0x03C9 BB64 		Encrypted: 0xB2F2 402B 		Decrypted: 0x03C9 BB64

Message: 0x1ACE EEFD 		Encrypted: 0x8A16 07C6 		Decrypted: 0x1ACE EEFD

Message: 0x1ACE EEFD 		Encrypted: 0xC598 5C3E 		Decrypted: 0x1ACE EEFD

c) 5 RSA instances(2 prime numbers(>30,000) as arguments) encryption-decryption

Message: 0x60C2 54AB 	Encrypted: 0x1DA8 E6A4 	Decrypted: 0x60C2 54AB

Message: 0x60C2 54AB 	Encrypted: 0x1338 A2CB 	Decrypted: 0x60C2 54AB

Message: 0x60C2 9652 	Encrypted: 0x60AE 1F00 	Decrypted: 0x60C2 9652

Message: 0x60C2 D7F9 	Encrypted: 0x6003 8944 	Decrypted: 0x60C2 D7F9

Message: 0x60C2 D7F9 	Encrypted: 0x410D 8C3D 	Decrypted: 0x60C2 D7F9

d) 5 RSA instances(2 non prime numbers(>30,000) as arguments) encryption-decryption

Message: 0x60C3 19A0 	Encrypted: 0x514C 6880 	Decrypted: 0x0765 4AB0

Message: 0x60C3 19A0 	Encrypted: 0x1DD0 FD40 	Decrypted: 0x3186 3100

Message: 0x60C3 19A0 	Encrypted: 0x1DD0 FD40 	Decrypted: 0x3186 3100

Message: 0x60C3 19A0 	Encrypted: 0x10C9 CA78 	Decrypted: 0x2BB8 C728

Message: 0x60C3 19A0 	Encrypted: 0x3C2C D968 	Decrypted: 0x339F E7BC

Message: 0x60C3 19A0 	Encrypted: 0x2B32 8800 	Decrypted: 0x3530 0C00

Message: 0x60C3 19A0 	Encrypted: 0x3C2C D968 	Decrypted: 0x339F E7BC

Message: 0x60C3 19A0 	Encrypted: 0x10C9 CA78 	Decrypted: 0x2BB8 C728

Message: 0x60C3 5B47 	Encrypted: 0x106C A157 	Decrypted: 0x2197 BB97

Message: 0x60C3 5B47 	Encrypted: 0x106C A157 	Decrypted: 0x2197 BB97

2)--------------------Challenge response scheme--------------------
Plain Text:0x5EFA FBBC 	Decrypted Text:0x5EFA FBBC
Challenge response scheme is Successful

3)------------------Blind signature---------------------
message: 0x2FA5 245B 	signature: 0x0001 0B3D DF46 	decrypted: 0x2FA5 245B

Blind signature: Blind signature Successful
