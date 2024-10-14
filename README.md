# FCSC 2021 Encrypted Shellcode

Lors d'un audit, vous trouvez ces fichiers et ces commandes dans des logs :
<code> 

    $ dd if=/dev/urandom of=key.bin bs=16 count=1
    $ ./esc -e < stereogram.png > stereogram.png.enc
    $ ./esc < stereogram.png
    [>] Done encrypting 1280731 bytes.
    [2]    11735 segmentation fault  ./esc < stereogram.png

</code>


Il semblerait que ce crash ait été exploité : pouvez-vous comprendre comment et lire le fichier flag.txt ?

Vous n'avez pas key.bin, mais le service fourni donne un accès à esc (sans argument) et utilisant le même fichier key.bin que celui généré par la commande ci-dessus.



Auteur : [Cryptanalyse](https://twitter.com/Cryptanalyse)

Origine : [Encrypted Shellcode](https://hackropole.fr/fr/challenges/pwn/fcsc2021-pwn-encrypted-shellcode/)




-----------

## Installation manuel
Vous n'utilisez pas l'application **les CTFs de Cyrhades** ? C'est dommage !
Mais voici comment installer ce CTF manuellement :

> git clone https://github.com/Hack-Oeil/fcsc2021-pwn-encrypted-shellcode.git

> cd fcsc2021-pwn-encrypted-shellcode


-----------

## Sur le site officiel hackropole.fr
> https://hackropole.fr/fr/challenges/pwn/fcsc2021-pwn-encrypted-shellcode/