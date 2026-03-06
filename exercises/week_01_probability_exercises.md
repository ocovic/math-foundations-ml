# Week 01 – Probability Foundations Exercises

## Concepts Covered

- Sample space
- Events
- Complement rule
- Addition rule
- Independence
- Conditional probability

---

# Conceptual Exercises

## Exercise 1

Given:

$$
P(A) = 0.6
$$

Find:

$$
P(A^c)
$$

### Solution

Using the complement rule:

$$
P(A^c) = 1 - P(A)
$$

Substitute the value:

$$
P(A^c) = 1 - 0.6 = 0.4
$$

---

## Exercise 2

Events $A$ and $B$ are **mutually exclusive**.

Given:

$$
P(A) = 0.3
$$

$$
P(B) = 0.2
$$

Find:

$$
P(A \cup B)
$$

### Solution

For mutually exclusive events:

$$
P(A \cap B) = 0
$$

Therefore:

$$
P(A \cup B) = P(A) + P(B)
$$

Substitute the values:

$$
P(A \cup B) = 0.3 + 0.2 = 0.5
$$

---

## Exercise 3

Events $A$ and $B$ are **independent**.

Given:

$$
P(A) = 0.5
$$

$$
P(B) = 0.4
$$

Find:

$$
P(A \cap B)
$$

### Solution

For independent events:

$$
P(A \cap B) = P(A)P(B)
$$

Substitute the values:

$$
P(A \cap B) = 0.5 \times 0.4 = 0.2
$$

---

# Applied Exercise – Dice Example

A fair six-sided die is rolled.

Define the events:

- $A$: obtaining an even number  
- $B$: obtaining a number greater than 3  

---

## Sample Space

$$
S = \{1,2,3,4,5,6\}
$$

---

## Step 1 – Compute $P(A)$

Event $A$ contains the even outcomes:

$$
A = \{2,4,6\}
$$

Therefore:

$$
P(A) = \frac{3}{6} = \frac{1}{2}
$$

---

## Step 2 – Compute $P(B)$

Event $B$ contains the outcomes greater than 3:

$$
B = \{4,5,6\}
$$

Therefore:

$$
P(B) = \frac{3}{6} = \frac{1}{2}
$$

---

## Step 3 – Compute $P(A \cap B)$

The intersection corresponds to outcomes that belong to both events.

$$
A \cap B = \{4,6\}
$$

Thus:

$$
P(A \cap B) = \frac{2}{6} = \frac{1}{3}
$$

---

## Step 4 – Test for Independence

Two events are independent if:

$$
P(A \cap B) = P(A)P(B)
$$

Compute the product of the probabilities:

$$
P(A)P(B) = \frac{1}{2} \times \frac{1}{2} = \frac{1}{4}
$$

Compare with the intersection probability:

$$
P(A \cap B) = \frac{1}{3}
$$

Since

$$
\frac{1}{3} \ne \frac{1}{4}
$$

the equality does not hold.

Therefore:

**Events $A$ and $B$ are not independent.**

---

## Conditional Probability Verification

Another way to test independence is using conditional probability.

Events are independent if:

$$
P(A \mid B) = P(A)
$$

Compute the conditional probability:

$$
P(A \mid B) = \frac{P(A \cap B)}{P(B)}
$$

Substitute the values:

$$
P(A \mid B) = \frac{1/3}{1/2}
$$

$$
P(A \mid B) = \frac{2}{3}
$$

Compare with the original probability:

$$
P(A) = \frac{1}{2}
$$

Since

$$
P(A \mid B) \ne P(A)
$$

knowing that event $B$ occurred changes the probability of $A$.

Therefore the events are **not independent**.

---

# Key Takeaway

Independence requires that:

$$
P(A \cap B) = P(A)P(B)
$$

or equivalently:

$$
P(A \mid B) = P(A)
$$

If either condition fails, the events are **not independent**.