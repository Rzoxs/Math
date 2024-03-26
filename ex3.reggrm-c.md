# Grammaire régulière

LHS | | RHS
---|--|--------
S  | -> | aaS
S  | -> | abaA
S  | -> | bA
S  | -> | abbaB
A  | -> | aaA
A  | -> | abaB
A  | -> | bB
B  | -> | aaB
B  | -> | ε

## Entrées acceptées
Entrée         | Résultat
---------------|---------------
aaabaaaabaaa   | Accept
aababa         | Accept
aaabbaaa       | Accept
aaabba         | Accept
aabb           | Accept
bb             | Accept
baaaba         | Accept
abab           | Accept
aabb           | Accept
ababaa         | Accept
aaaaaaaabb     | Accept

## Entrées rejetées
Entrée         | Résultat
---------------|-----------------
b              | Reject
ba             | Reject
aaba           | Reject
aaaa           | Reject
aaaaabb        | Reject
aabaaa         | Reject
bbaabb         | Reject
baaab          | Reject
bbaab          | Reject
bba            | Reject

## Description mathématique & expression régulière