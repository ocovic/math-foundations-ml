## MIT 18.05 – Class 01: Introduction, Counting, and Sets | Class 02: Probability Basics – Notes

### Probability

- Probability is a mathematical measure of the degree of uncertainty associated with the occurrence of an event. It is expressed as a number between 0 (impossible) and 1 (certain), or equivalently as a percentage (0%–100%).
- Formally, probability does not measure “certainty,” but rather the plausibility of an event occurring within a random experiment.
- In finite sample spaces with equally likely outcomes, probability can be computed using the Laplace formula:

  \[
  P(A) = \frac{\text{number of favorable outcomes}}{\text{total number of possible outcomes}}
  \]

  This formula is valid only when all outcomes are equally likely.

---

### Probability vs. Statistics

- **Probability**
  - Logically autonomous.
  - Based on formal rules and axioms.
  - Typically leads to a single correct mathematical answer.

- **Statistics**
  - More complex and interpretative.
  - Uses probability theory to make inferences from observed data.
  - May lead to multiple reasonable conclusions depending on assumptions and models.

---

### Basic Concepts

- **Experiment**: A repeatable procedure with well-defined possible outcomes.
- **Sample Space** \( S \): The set of all possible outcomes of an experiment.
- **Event**: A subset of the sample space.
- **Probability Measure** \( P \): A function defined on events (subsets of \( S \)) that satisfies the Kolmogorov axioms.
  - Assigns a real number between 0 and 1 to each event.
  - Satisfies non-negativity, normalization, and additivity.

---

### Kolmogorov Axioms (1933)

These are the three fundamental axioms that define probability.

1. **Non-negativity**
   \[
   P(A) \ge 0
   \]
   For any event \( A \subseteq S \), probability is non-negative.

2. **Normalization**
   \[
   P(S) = 1
   \]
   The probability of the entire sample space is 1.

3. **Additivity (for mutually exclusive events)**
   If \( A_1, A_2, \dots \) are mutually exclusive (disjoint) events:
   \[
   P(A_1 \cup A_2 \cup \dots) = P(A_1) + P(A_2) + \dots
   \]

---

### Properties Derived from the Axioms

- **Impossible Event**
  \[
  P(\emptyset) = 0
  \]

- **Complement Rule**
  \[
  P(A^c) = 1 - P(A)
  \]

- **Range**
  \[
  0 \le P(A) \le 1
  \]

- **Monotonicity**
  If \( A \subseteq B \), then:
  \[
  P(A) \le P(B)
  \]

---

### Independence

Two events \( A \) and \( B \) are independent if:

\[
P(A \cap B) = P(A) P(B)
\]

Independence means that the occurrence of one event does not affect the probability of the other.

If \( P(B) > 0 \), independence implies:

\[
P(A \mid B) = P(A)
\]

---

### Mutually Exclusive (Disjoint) Events

Two events are mutually exclusive if they cannot occur simultaneously.

\[
P(A \cap B) = 0
\]

For mutually exclusive events:

\[
P(A \cup B) = P(A) + P(B)
\]

Important:

If \( P(A) > 0 \) and \( P(B) > 0 \), mutually exclusive events cannot be independent.

Example:
When rolling a die, obtaining a 2 (event \( A \)) and obtaining a 5 (event \( B \)) are mutually exclusive events.

---

### Non-Mutually Exclusive Events

If events overlap:

\[
P(A \cup B) = P(A) + P(B) - P(A \cap B)
\]

This formula avoids double-counting the intersection.

Example:
Drawing a card that is an Ace (event \( A \)) and red (event \( B \)). The Ace of Hearts and Ace of Diamonds belong to both events.

---

## Mathematical Observations

- Independence is a multiplicative relationship.
- Mutual exclusivity is an additive structural constraint.
- If two events are mutually exclusive and both have positive probability, they cannot be independent.
- Kolmogorov’s axioms define probability abstractly, independent of the frequentist interpretation.