S -> bA
A -> abaA
A -> abaB
B -> b
B -> epsilon

# Grammaire régulière

LHS | | RHS
---|--|--------
S  | -> | bA
A  | -> | abaA
A  | -> | abaB
B  | -> | b
B  | -> | epsilon

## Entrées acceptées
-----------------|-----------------
babaaba        | Accept
babaabab       | Accept
baba           | Accept
babaabaabaaba  | Accept
babab          | Accept

## Entrées rejetées
 | 
-----------------|-----------------
b            | Reject
bb           | Reject
abab         | Reject
abaaba       | Reject
babababa     | Reject

bb            -> Reject
abab          -> Reject
abaaba        -> Reject
b             -> Reject
babababa      -> Reject




L(G) = { b (aba)^n b^m | n>,1, m<=1}
ERg = b(aba)*(b|λ)


/**************************/

S -> aaS
S -> abaA
S -> bA
S -> abbaB
A -> aaA
A -> abaB
A -> bB
B -> aaB
B -> epsilon