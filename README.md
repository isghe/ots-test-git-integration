# ots-test-git-integration

Verify and test [opentimestamps-git-integration](https://github.com/opentimestamps/opentimestamps-client/blob/master/doc/git-integration.md)
```
₿ git log --show-signature
commit d8390c4664eb394d6db1ec6a8da458181ea3bbb8 (HEAD -> master)
ots: Calendar https://bob.btc.calendar.opentimestamps.org: Pending confirmation in Bitcoin blockchain
ots: Calendar https://alice.btc.calendar.opentimestamps.org: Pending confirmation in Bitcoin blockchain
ots: Calendar https://finney.calendar.eternitywall.com: Pending confirmation in Bitcoin blockchain
ots: Calendar https://btc.calendar.catallaxy.com: Pending confirmation in Bitcoin blockchain
ots: Could not verify timestamp!
gpg: Signature made Sat Feb 17 11:45:57 2024 CET
gpg:                using RSA key 0F11E7FD81B2D24AD6C1C75F8E8FEE2637C508B1
gpg: Good signature from "Isidoro Ghezzi <isidoro.ghezzi@icloud.com>" [ultimate]
gpg:                 aka "Isidoro Ghezzi <isidoroghezzi@salgroup.it>" [ultimate]
Author: Isidoro Ghezzi <isidoro.ghezzi@icloud.com>
Date:   Sat Feb 17 11:45:47 2024 +0100

    initial commit
```

```
₿ git cat-file -p d8390c4664eb394d6db1ec6a8da458181ea3bbb8
tree 324984032484b4fd71e50b8e31c048d54e793508
author Isidoro Ghezzi <isidoro.ghezzi@icloud.com> 1708166747 +0100
committer Isidoro Ghezzi <isidoro.ghezzi@icloud.com> 1708166747 +0100
gpgsig -----BEGIN PGP SIGNATURE-----

 iQIzBAABCAAdFiEEDxHn/YGy0krWwcdfjo/uJjfFCLEFAmXQjmUACgkQjo/uJjfF
 CLH33w/9EDzWKvQHBFcgrI/sthDn7+ffNF2Y6BQiOpHcKLGFFzZal5soNlf/IiAW
 y/zuwkHyQVeE7wC7vEgJiMqA4i+vnVcoAa0CPwSxx7MzVVQgXRKf6FOHrfhzFZXX
 d58S/mEpDWefVaIGWKIwYICf6Re19hP73gk0Z6qyd4KggpNgHUbwwvOaS4wQMNfE
 Loj6p1tOaVWnWrUfPRArp0JoRflkiKZEOp3329CIiv6V1Ktjyp/HD7DE/4II+DD1
 riiJqzIPM6HplnZ++mmON5RaQ5aVXZuDL6xj3z8U3TI0kk26lS6EX80sH4JZTXHe
 b3ZFUYqRlyD4Cs0lzTqJBl0pj9zP3BcTbl+2sCtsNJa/wLtBfpuhbo+p6baK/hzi
 djjUFpwqLqQJPdJiVu/foCOzbRGRqdeeODUCvs7+FUrfCAEquVZgYxQBLTHyVJAn
 vFEOlBNPWgmgSrZ+smAOTvgjGS5R/codDVMB7QkB7d1+773IxiEMLm5HAXDJMHCX
 +N8sHXnmZX8q8JUDbqUcVK/DKVN4YLNC9Nye1cBN/z3ZutrVO8hoZKkmI8mmE8+w
 x2MZWEt3kxcsbe9AJrZGhXXgo6uMzTljHbj3qiLVUVbsCYc1g+ccyncL+Ckx4mBA
 JBvovFWMp1TZVOB3d1ka/+OAHb3rvKggWiw+xh8gc+TuqjzpLww=
 =vk15
 -----END PGP SIGNATURE-----
 -----BEGIN OPENTIMESTAMPS GIT TIMESTAMP-----

 AQHwIMk7b4qUmvyQsh4wxe3ffVNs8dO/82z5h7dGtreAQmyGCP/wEBI/P/PlFYZp
 l81setrqzcwI8QRl0I5m8Aiyl/qTH5RciACD3+MNLvkMjiwraHR0cHM6Ly9ib2Iu
 YnRjLmNhbGVuZGFyLm9wZW50aW1lc3RhbXBzLm9yZ//wECXSdL0Vlt5keJpLis2W
 RRkI8SCKOVlQnRJ8MZOFiivl8cxgfBEHe5ab01eERTMe7ocuLgjxBGXQjmbwCII3
 uU+spfk6AIPf4w0u+QyOLi1odHRwczovL2FsaWNlLmJ0Yy5jYWxlbmRhci5vcGVu
 dGltZXN0YW1wcy5vcmf/8BBLK3Lmoa9dvXlq0+81LJ/8CPEg7kj6POjL2W/0ehXY
 CToYG4Bh1zqxBAy4t+nvA32suLEI8QRl0I5l8AiQAf8cox1ACgCD3+MNLvkMjiko
 aHR0cHM6Ly9maW5uZXkuY2FsZW5kYXIuZXRlcm5pdHl3YWxsLmNvbfAQyU95cS3j
 atlbsUIEQmegUQjwIDSSQhgb75ANMsBN06OSA/x2Wb/eEbLtvSI2tAL9o0x/CPEE
 ZdCOZvAIz3qAD8qNcG0Ag9/jDS75DI4jImh0dHBzOi8vYnRjLmNhbGVuZGFyLmNh
 dGFsbGF4eS5jb20=
 -----END OPENTIMESTAMPS GIT TIMESTAMP-----

initial commit
```

```
₿ gpg --verify sign-test.txt.sig
gpg: assuming signed data in 'sign-test.txt'
gpg: Signature made Sat Feb 17 11:45:57 2024 CET
gpg:                using RSA key 0F11E7FD81B2D24AD6C1C75F8E8FEE2637C508B1
gpg: Good signature from "Isidoro Ghezzi <isidoro.ghezzi@icloud.com>" [ultimate]
gpg:                 aka "Isidoro Ghezzi <isidoroghezzi@salgroup.it>" [ultimate]
```
