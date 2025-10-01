# Clean Animation Outline (Full Text per Frame)

### Frame 1 – Sampling

**Animation:** Sampling (shimmering icon)
**Action:** Model is “thinking.”
**Visible Text:**

```
Problem: A rectangle has a perimeter of 24 inches. What is the maximum possible area of the rectangle?

Solution:
[[{shimmering sampling icon}]]
```

---

### Frame 2 – Proposed Candidate Prefix

**Animation:** Typing-out text
**Action:** Generate first candidate.
**Visible Text:**

```
Solution:
[[Let the length of the rectangle be (l), width be (w). We want to maximize the area (A = lw) subject to the constraint (2l + 2w = 24).]]
```

---

### Frame 3 – Sampling

**Animation:** Shimmering icon
**Action:** Pause before continuing.
**Visible Text:**

```
Solution:
[Let the length of the rectangle be (l), width be (w). We want to maximize the area (A = lw) subject to the constraint (2l + 2w = 24).]
[[{shimmering sampling icon}]]
```

---

### Frame 4 – Contraction

**Animation:** Deletion of candidate prefix
**Action:** Backspace until only the first part remains.
**Visible Text:**

```
Solution:
[[Let the length of the rectangle be (l)]]
```

---

### Frame 5 – Sampling

**Animation:** Shimmering
**Action:** Pause again.
**Visible Text:**

```
Solution:
[Let the length of the rectangle be (l)]
[[{shimmering sampling icon}]]
```

---

### Frame 6 – Candidate Accepted

**Animation:** Bold + shimmer
**Action:** Commit prefix.
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}}
```

---

### Frame 7 – Proposed Candidate Prefix

**Animation:** Typing-out text
**Action:** Add width and constraint.
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}} 
[[and the width of the rectangle be (w). Since the perimeter of the rectangle is 24 inches, we have that (2l + 2w = 24), so (l + w = 12). We wish to maximize the area of the rectangle,]]
```

---

### Frame 8 – Sampling

**Animation:** Shimmering
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}} 
[and the width of the rectangle be (w). Since the perimeter of the rectangle is 24 inches, we have that (2l + 2w = 24), so (l + w = 12). We wish to maximize the area of the rectangle,]
[[{shimmering sampling icon}]]
```

---

### Frame 9 – Candidate Accepted + Sampling

**Animation:** Commit + shimmer
**Action:** Accept second prefix, then pause.
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}} 
{{and the width of the rectangle be (w). Since the perimeter of the rectangle is 24 inches, we have that (2l + 2w = 24), so (l + w = 12). We wish to maximize the area of the rectangle,}}
[[{shimmering sampling icon}]]
```

---

### Frame 10 – Proposed Candidate Prefix

**Animation:** Typing-out text
**Action:** Add expression for A and derivative step.
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}} 
{{and the width of the rectangle be (w). Since the perimeter of the rectangle is 24 inches, we have that (2l + 2w = 24), so (l + w = 12). We wish to maximize the area of the rectangle,}} 
[[which because of the constraint can be expressed as (A = lw = l(12 - l) = 12l - l^2). To find the maximum area, we take the derivative of (A) with respect to (l) and set it to zero:]]
```

---

### Frame 11 – Sampling

**Animation:** Shimmering
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}} 
{{and the width of the rectangle be (w). Since the perimeter of the rectangle is 24 inches, we have that (2l + 2w = 24), so (l + w = 12). We wish to maximize the area of the rectangle,}} 
[which because of the constraint can be expressed as (A = lw = l(12 - l) = 12l - l^2). To find the maximum area, we take the derivative of (A) with respect to (l) and set it to zero:]
[[{shimmering sampling icon}]]
```

---

### Frame 12 – Contraction

**Animation:** Deletion
**Action:** Shrink back to only “which.”
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}} 
{{and the width of the rectangle be (w). Since the perimeter of the rectangle is 24 inches, we have that (2l + 2w = 24), so (l + w = 12). We wish to maximize the area of the rectangle,}} 
[[which]]
```

---

### Frame 13 – Sampling

**Animation:** Shimmering
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}} 
{{and the width of the rectangle be (w). Since the perimeter of the rectangle is 24 inches, we have that (2l + 2w = 24), so (l + w = 12). We wish to maximize the area of the rectangle,}} 
[which]
[[{shimmering sampling icon}]]
```

---

### Frame 14 – Candidate Accepted + Correct Solution Found

**Animation:** Commit prefixes + shimmer entire solution
**Action:** Accept full reasoning and reveal final result.
**Visible Text:**

```
Solution:
{{Let the length of the rectangle be (l)}} 
{{and the width of the rectangle be (w). Since the perimeter of the rectangle is 24 inches, we have that (2l + 2w = 24), so (l + w = 12). We wish to maximize the area of the rectangle,}} 
{{which}} 
is (A = lw). Let (l = 12 - w) and plug into the area:

A = (12 - w)w  ⇒  A = 12w - w^2

Differentiate: A'(w) = 12 - 2w

Set derivative = 0 ⇒ w = 6

Then l = 6. Therefore, the maximum area is

A = lw = 6 × 6 = **36**
```

**Final Animation:** Entire solution shimmers (correct solution found).

---

