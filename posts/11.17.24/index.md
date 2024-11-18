# Exponential Cryptology with Keys - (ECK)
First of all I have to mention this is a proof of concept and has lots of flaws. This is by no means any method to keep data secure and can be broken increadibly easily. This has also been found out in some form or another at some point.

This method works by first assigning each letter or character a number. Atleast numbers past 100. Also dont skip 10s and 5s. There is just a quick sample table below. 

|Character | Number |
|:---------|:---------|
|A|101|
|B|102|
|C|103|
|D|104|
|E|106|
|F|107|
|G|108|
|H|109|
|I|111|
|J|112|
|K|113|
|L|114|
|M|116|
|N|117|
|O|118|
|P|119|
|Q|121|
|R|122|
|S|123|
|T|124|
|U|126|
|V|127|
|W|128|
|X|129|
|Y|131|
|Z|132|
|(Space)|133|
|(Pierod)|134|


This table should be on both recieving ends and is one of the keys. The second key is the order of exponents. The way that this algorithm works is by first translating each character into each Corresponding Number. We will use the code "This is a secret".

```This is a secret -> 124_109_111_123_133_111_123_133_101_133_123_106_103_122_106_124_134```

The next step is to make the second key. The second key will be any 10 numbers between 5-9. Obviously this can be modified to any number amount you want and however high you want it. The higher the numbers the harder to crack. For simplicity I will be useing the code 5678956789. Apply each exponent base to the above numbers in order.

```124_109_111_123_133_111_123_133_101_133_123_106_103_122_106_124_134 -> 124^5_109^6_111^7_123^8_133^9_111^5_123^6_133^7_101^8_133^9_123^5_106^6_103^7_122^8_106^9_124^5_134^6```
This tranlates into the following numbers below:

```29316250624_1677100110841_207616015289871_52389094428262881_13021612539908538853_16850581551```
```_3462825991689_736141813551277_10828567056280801_13021612539908538853_28153056843_1418519112256```
```_122987386542487_49077072127303936_1689478959002692096_29316250624_5789336458816```

That is your final code in integer form. Obviously this entire algorithm can be condensed if just done in binary entirely.

# Cracking
To crack this code you would have to know atleast the first key, what letter equals which number. The simplist way is to take a number and check for a perfect square, then a perfect cube, and so on untill you find the what the exponent is. Then you just simply compare it to the key and get your code. If you increase the exponents anywhere up to 100 not only is the code going to be increadibly time consumeing by programs to crack but also very data intesive because of the size of the numbers. In general this code is fairly easy to crack as long as you have the first key, the exponents are just to randomize the code and stop frequency anaylsis.
