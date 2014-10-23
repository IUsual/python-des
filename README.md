Python-DES
==========

[DES](http://en.wikipedia.org/wiki/Data_Encryption_Standard) encryption in Python.

DES is a _symmetric_ encryption algorithm, meaning you use the same key to
encrypt and decrypt the data later on.

This is the first Python codes I made, in when I begin to learn Python language and start my Cryptography class in Nuaa. Some problems are existed, and there will be some `pull` and `push` to do overcome.

Usage
=====
Now, it runs like this:

```pycon
>>> from python-des import SimpleDES
>>> key = "AABB09182736CCDD"
>>> plain = "123456ABCD132536"
>>> des = SimpleDes(key)
>>> des.printHexList(des.encrypt(plain))
C0 B7 A8 D0 5F 3A 82 9C
```

**INFO:* `des.encrypt()` returns a binary list, which is convenient for further handle.
You can encrypt more text using one key, do `des.encrypt(text)` as well.

Issues
======

### First
Whatever, I need decrypt here.There is just encryption here, decrypt is a must.

### Second
Debug infos, I think `logging` module can be used to do something else, or, unit test or `doctest` is also a better way to make it better.

### Third
Otherwise, now I use int type to process data, maybe `struct` module can help me speed it's run times up, and reduce space waste.


