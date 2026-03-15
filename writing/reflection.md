# CS101 Spring 2026 — Practice Midterm Reflection

Name: Aidana 
Date: 15/03/2026

After completing the practice test, please reflect on your experience by
answering the questions below. Replace each `todo` with a thoughtful response (a few sentences each). Your responses help you consolidate what you learned and identify areas to review before the real midterm.

---

## 1. Self-Assessment

**Question:** How did you feel about your performance on the practice test? Which topics felt most comfortable, and which ones felt most difficult?

**Your Answer:**

I feel confident because most of my answers were correct, and I performed well overall. I found topics like lists, tuples, and loops (for/if) to be the most comfortable. However, I struggled with more abstract concepts, specifically lambda functions, algorithmic methods, and dictionary operations.
---

## 2. Tricky Questions

**Question:** Identify one question you got wrong (or were unsure about).
Explain the concept being tested and describe why the correct answer is right.

**Your Answer:**

I initially struggled with Question 24. This question tests the concept of Class Instances and how they interact with lists. The correct answer is `c) False, True`. This is because Python can store objects inside a list just like integers or strings. When you iterate through that list, the loop variable refers to the actual object, allowing you to access its specific attributes, such as .pages.
---

## 3. Loops and Iteration

**Question:** In your own words, explain the difference between `range(a, b, step)` with a positive step versus a negative step. Give one original example of each.

**Your Answer:**

Positive Step: Increments the index. It starts at a and moves toward b.Example: list(range(1, 5, 1)) returns [1, 2, 3, 4]

Negative Step: Decrements the index. It starts at a and moves "backwards" toward b, where a must be greater than b.
Example: list(range(5, 1, -1)) returns [5, 4, 3, 2]
---

## 4. Data Structures

**Question:** Python has lists, tuples, dictionaries, and sets. Describe one key difference between a list and a tuple, and one key difference between a dictionary and a set. When would you choose each?

**Your Answer:**

List vs. Tuple: The main difference is mutability. Lists are flexible and can be changed after creation, whereas tuples are "read-only." Programmers use a list for a collection that needs updating, like a task list, and a tuple for fixed data, like GPS coordinates.

Dictionary vs. Set: A dictionary stores key-value pairs (like a word and its definition), while a set only stores unique individual items. A dictionary is used when it's needed to look up data using a label, and a set when you need to ensure there are no duplicate values in your data.

---

## 5. Functions

**Question:** What is a default parameter in a Python function? Write a short
example function that uses a default parameter, and explain what happens when
the caller omits that argument.

**Your Answer:**
A default parameter is a fallback value defined in the function header. If the person calling the function does not provide an argument for that parameter, Python uses the default value automatically. For example:

```python
def power(base, exponent=2): 
    return base ** exponent
```
If I call power(5), it returns `25` because the exponent defaults to `2`. If I call power(5, 3), it overrides the default and returns `125`.
---

## 6. List Comprehensions

**Question:** List comprehensions can include an optional filter condition.
Rewrite the following traditional loop as a list comprehension:

```python
result = []
for n in range(1, 11):
    if n % 3 == 0:
        result.append(n * 2)
```

**Your Answer:**
```python
result = [n * 2 for n in range(1, 11) if n % 3 == 0]
```
---

## 7. Operator Precedence

**Question:** Python evaluates `**` (exponentiation) right-to-left.
What is the value of `2 ** 2 ** 3`? Show your step-by-step reasoning.

**Your Answer:**
`2 ** 2 ** 3` is calculated with the following steps:

1) 2 ** 3 = 2 * 2 * 2 = 8
2) 2 ** 8 = 2 * 2 * 2 * 2 * 2 * 2 * 2 * 2 = 256. 

Hence, the final answer is 256.


---

## 8. Classes 

**Question:** What are classes in Python programming? Explain why they are necessary in programming.

**Your Answer:**

Classes are used to create objects. They are essential in programming because they allow developers to group data and functions into one organized unit. This makes code reusable and much easier to manage. For instance, instead of managing hundreds of separate variables for a "User," you can create one User class and generate as many individual user objects as you need.

---

(Did you remember to add your name and date at the top of this document?)
