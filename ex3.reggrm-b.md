# Grammaire régulière

LHS | | RHS
---|--|--------
S  | -> | bA
A  | -> | abaA
A  | -> | abaB
B  | -> | b
B  | -> | ε

## Entrées acceptées
Entrée         | Résultat
---------------|---------------
babaaba        | Accept
babaabab       | Accept
baba           | Accept
babaabaabaaba  | Accept
babab          | Accept

## Entrées rejetées
Entrée         | Résultat
---------------|-----------------
b              | Reject
bb             | Reject
abab           | Reject
abaaba         | Reject
babababa       | Reject

## Description mathématique & expression régulière
L(G) = { b (aba)^n b^m | n>,1, m<=1}
ERg = b(aba)*(b|λ)