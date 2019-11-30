
Empty testing is only possible when the number of tokens is known in advance. Because the number of witnesses per claim is determined
when the petri net is running, is's not possible to know when all witnesses have been handled so the exercise is impossible.
- The Zero Testing net shown in lecture 6 requires that there are N input/output arcs from p', where N is the initial number of tokens (number of witnesses per claim in this case). N is not constant so the number of arcs would have to change while the net is running.

The net in witnesses.pnml will never finish handling a claim because it doesn't know when all witnesses are handled. 
