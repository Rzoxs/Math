S -> bA
A -> abaA
A -> abaB
B -> b
B -> epsilon

LHS | | RHS
---|--|--------
S  | -> | bA
A  | -> | abaA
A  | -> | abaB
B  | -> | b
B  | -> | epsilon

		

babaaba       -> Accept
babaabab      -> Accept
baba          -> Accept
babaabaabaaba -> Accept
babab         -> Accept

bb            -> Reject
abab          -> Reject
abaaba        -> Reject
b             -> Reject
babababa      -> Reject

L(G) = { b^n aba^m | n,m >= 0}
ERg = (b)* (aba)*


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