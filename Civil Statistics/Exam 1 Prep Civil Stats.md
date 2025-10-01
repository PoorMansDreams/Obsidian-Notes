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


