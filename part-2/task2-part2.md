Answers for Distributed Systems (Autumn 2019) Task 2, Part 2 on Petri Nets.

Q1: Are these three nets live? Explain how did you check this.

A1: Check whether there is at minimum one transition that can fire. If
there are no transitions that can fire, the net is dead; otherwise it
is considered live.

* Net-1 is live as transitions can fire: {t2}
* Net-2 is live as transitions can fire: {t2,t4}
* Net-3 is live as transitions can fire: {t2,t4,t6}
