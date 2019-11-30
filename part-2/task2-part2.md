Answers for Distributed Systems (Autumn 2019) Task 2, Part 2 on Petri Nets.

Q1: Are these three nets live? Explain how did you check this.

A1: Check whether there is at minimum one transition that can fire. If
there are no transitions that can fire, the net is dead; otherwise it
is considered live.

* Net-1 is live as transitions can fire: {t2}
* Net-2 is live as transitions can fire: {t2,t4}
* Net-3 is live as transitions can fire: {t2,t4,t6}

Q2: Are these nets bounded? Explain how did you check this.

A1: A Petri net is considered bounded if all of its places are k-bounded.
That is, each place can have a maximum of k tokens for some value of k. A
Petri net is not bounded if it has a place that can have an unlimited
number of tokens.

* Net-1 is k-bounded with k=1. At M0 there is one token in {s1,s2}. 
Following through the possible transitions, we end up again in a marking
that matches M0. At no point is there more than one token in any place.
The k=1 was checked manually.
* Net-2 is not bounded. Experimental testing allows infinite tokens to
accumulate in place s8.
* Net-3 bounding unknown.

Q3: For each of these nets, what is the length of the shortest firing
sequence that leads to a marking in which all odd-numbered places have a
token? For example, in the case of the first net, we want to know the
length of the shortest firing sequence that leads to the marking where
there is a token in s1 and a token in s3.

* Net-1 

Q4: The three nets shown here are the first three elements of an infinite
family of nets. We can create the n th member of the family by taking the
(n-1) th member and replicating the repeating pattern to the right. Consider
the n th Petri net in this family. Can you say something about the length
of the shortest path that leads to a marking in which all odd-numbered
places have a token?