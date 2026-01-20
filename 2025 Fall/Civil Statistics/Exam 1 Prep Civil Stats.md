#probability
### The Lego Problem (Counting)
A LEGO® Problem. A LEGO miniature figure (AKA minifig) consists of 5 parts – a pair of legs, a torso including arms, a head, hair/hat, and an accessory. The LEGO store allows you to build your own custom minifig from a selection of available parts. On a given day, the LEGO store has 4 different pairs of legs, 6 different torsos, 5 different heads, 6 different hair/hats and 8 accessories in stock. Specifically, they have many copies of each part.  


(a) How many unique minifigs can be constructed if they must contains all 5 parts?  

Number of unique combinations, 5 slots,
4 - legs
6 - torsos
5 - heads
6 - hairs
8 - accessories

$4\cdot6\cdot5\cdot6\cdot8= 5760$ **different options**

(b) Unfortunately, you can’t just buy one minifig, you must buy them in packs of 3. If you want all 3 of your minifigs to be completely different, how many possible minifig packages could be prepared and sold to lovers of little plastic people? (completely different means none of the parts in one minifig are duplicated in other two)  

$$
C^{5760}_{3}=31.833\times 10^9 \text{ different packs of 3 possible }
$$
Pool of 5760 different lil guys, pick 3 from 5760, combination function lets use calculate how many different ways you can chose 3 minifigs from 5760, order not mattering.

(c) If, amongst the different heads, you note 2 male heads, 2 female heads and 1 robot head, what is the probability that a minifig randomly selected from a pile of completed minifigs is female?

$$
\frac{C^2_{1}}{C^5_{1}}=\frac{2}{5}=0.4
$$
Pool of 2 female heads, choose 1 of those female heads, divide by how many different kinds of heads you can chose, (5 different heads).

### Final Exam Problem (Counting)
Six students are eligible to get an A in this class, but I’m only giving out 4 As. How many different lists of A-students can I generate? 
$$
C^6_{4}=15 \text{ different ways to chose 4 students}
$$
Pool of 6 students, 4 students to chose. There are 15 combinations/ways to chose 4 students from those 6 students.


### Apocalypse
It’s the End of the World As We Know It. The potential for an apocalypse worries me. What worries me most is that it could include any number of disasters. There is a 10% chance of a zombie infection. There is a 12% chance of Ragnorak (that’s the Norse apocalypse). There is an 8% chance of a UFO invasion. Heck, it could be like some show on the SyFy channel and all 3 might happen at the same time. (Translation: All three events are independent and not mutually exclusive.)

(a) What is the probability that we will have an apocalypse of one sort or another?  

$P(Z) = 0.1$
$P(R)=0.12$
$P(U)=0.08$

the compliments or "nots" are

$P(Z')=0.9$
$P(R')=0.88$
$P(U')=0.92$

So probability that zombies AND ragnarok AND ufo's don't happen is
$$
P(Z'\cap R'\cap U')=0.9\times 0.88\times 0.92 =0.729
$$
Which means probability of at lease one of these happening is the compliment of none of them happening
$$
P(\text{Apocalypse})=1-0.729=0.271
$$


(b) I’m also a part-time actuary and in my need to prepare, I’ve decided to only  
prepare for those events which have a 0.9% chance or greater of occurring. Which  
types of apocalypses and combinations of apocalypses do I need to prepare for?

The number of combinations of apocalypses are
$P(Z\cap R)=0.1\times 0.12=0.012$
$P(Z\cap U)=0.1\times 0.08=0.008$
$P(R\cap U)=0.12\times 0.08=0.096$
$P(Z\cap R\cap U)=0.1\times 0.12 \times 0.08=0.00096$

all probabilities that are greater than 0.9% or 0.009 are
- Zombie and Ragnarok
- Ragnarok and UFO 
- Zombie
- Ragnarok
- UFO

### Eggs
I left my eggs out overnight several ago. Worried for my health, I went online and learned that the CDC estimates a 0.005% chance of any given egg having Salmonella, which is why you’re supposed to refrigerate them. Risking my life, I made scrambled eggs with 3 of them. What was my probability of my being exposed to Salmonella?

$P(S)=0.00005$ is this probability the egg has salmonella
$P(S')=0.99995$ is the probability of an egg not having salmonella

There are 3 eggs, and only one of those eggs need to have salmonella

chances of all 3 eggs NOT having salmonella is $P(S'\cap S'\cap S')$ or $P(S')^3=0.99985$

which means chance of at lease one of the eggs having salmonella is $${P(S\cup S\cup S)=1-P(S')^3}=0.00014999=0.014999\%$$
### Tests
There are two different versions of tests, A and B, what is the probability that for the 3 tests you get the same one?

similar to flipping a coin 3 times and getting heads three times.

$P(A)=0.5\text{ is the probability of getting test A}$
3 tests you need to get test A, so
$$
P(A)^3=0.125
$$
similarly,
$$
P(B)^3=0.125
$$
you can either get three type A exams or three type B exams, so you add their probabilities.

$$
P(A)^3+P(B)^3=0.125+0.125=0.25
$$

### Monty Hall Problem
3 Envelopes, envelope A, B, and C, only one has money. You choose A.
$P(A)=0.33$ probability of getting the money from envelope A is 33%
$P(B)=0.33$ probability of getting the money from envelope B is 33%
$P(C)=0.33$ probability of getting the money from envelope C is 33%

After choosing, it is revealed that envelope B has nothing in it.
When this event happened, the person willingly chose the envelope with nothing in it, and did not chose the envelope you chose. 

Since one of the envelopes has money in it, AND the person can only open an empty envelope, there's only 2 envelopes to choose from.

$P(E)\text{ is the probability of choosing the empty envelope B}$

if we chose A, and the prize was in A, the chosen empty envelope could only be C or B (50/50)

$$
P(E|A)=0.5\text{ is the probability of the opened envelope being B}
$$

if we chose A, and the prize was in C, the chances of the person opening envelope B has to 1, since B is the only empty envelope, and we chose A.

$$
P(E|C)=1 \text{ is the probability the opened envelope is B}
$$

Using Total Probability Law we can calculate $P(E)$

$$
P(E)=P(E|A)\cdot P(A)+P(E|B)\cdot P(B)+P(E|C)\cdot P(C)
$$

if the prize is in B, then there is no way for B to be the opened *empty* envelope $P(E|B)=0$

$$
P(E)=0.5\times 0.33+1\times 0.33=0.5
$$

knowing this, we can calculate the chances of $P(C|E)$ which is the probability of the opened (empty) envelope is B, and the prize is in C

$$P(C|E)=\frac{P(E|C)\cdot P(C)}{P(E)}=\frac{1\times 0.33}{0.5}=0.66$$
we can also calculate the chances of $P(A|E)$ which is the probability of the opened (empty) envelope is B, and the prize is in A

$$
P(A|E)=\frac{P(E|A)\cdot P(A)}{P(E)}=\frac{0.5\times 0.33}{0.5}=0.33
$$

since there is a greater chance that the prize is actually in C, it is better to ==switch==. 






