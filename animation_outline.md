Possible animations:
- Sampling animation: shimmering effect on the sampling icon while the model "thinks".
- Proposed candidate prefix animation: text being typed out as an uncommitted proposal.
- Contraction animation: deleting characters from the latest proposed text back to a prior prefix.
- Candidate prefix accepted and committed animation: newly approved text becomes bold and receives a brief shimmer.
- Correct solution has been found animation: the full solution shimmers to signal completion.

---

### Frame 1 - Initial sampling
**Problem** A rectangle has a perimeter of 24 inches. What is the maximum possible area of the rectangle?

**Solution view**
- Committed text: *(none yet)*
- Proposed text: *(none yet)*

**Animations**
- Sampling animation - shimmering sampling icon.

---

### Frame 2 - First proposal appears
**Problem** Same as Frame 1.

**Solution view**
- Committed text: *(none yet)*
- Proposed text: "Let the length of the rectangle be ( l ), width be ( w ). We want to maximize the area ( A = lw ) subject to the constraint ( 2l + 2w = 24 )."

**Animations**
- Proposed candidate prefix animation - the text above types on screen.

---

### Frame 3 - Sampling on proposed text
**Problem** Same as Frame 1.

**Solution view**
- Committed text: *(none yet)*
- Proposed text: "Let the length of the rectangle be ( l ), width be ( w ). We want to maximize the area ( A = lw ) subject to the constraint ( 2l + 2w = 24 )."

**Animations**
- Sampling animation - shimmering sampling icon while considering the proposal.

---

### Frame 4 - Proposal contracts
**Problem** Same as Frame 1.

**Solution view**
- Committed text: *(none yet)*
- Proposed text: "Let the length of the rectangle be ( l )"

**Animations**
- Contraction animation - previously typed text deletes back to this prefix.

---

### Frame 5 - Sampling after contraction
**Problem** Same as Frame 1.

**Solution view**
- Committed text: *(none yet)*
- Proposed text: "Let the length of the rectangle be ( l )"

**Animations**
- Sampling animation - shimmering sampling icon on the shorter proposal.

---

### Frame 6 - Prefix accepted
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l )"**
- Proposed text: *(none)*

**Animations**
- Candidate prefix accepted and committed animation - accepted text bolds and shimmers briefly.

---

### Frame 7 - New proposal extends solution
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l )"**
- Proposed text: " and the width of the rectangle be ( w ). Since the perimeter of the rectangle is 24 inches, we have that ( 2l + 2w = 24 ), so ( l + w = 12 ). We wish to maximize the area of the rectangle, "

**Animations**
- Proposed candidate prefix animation - the new text types out after the committed prefix.

---

### Frame 8 - Sampling on second proposal
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l )"**
- Proposed text: " and the width of the rectangle be ( w ). Since the perimeter of the rectangle is 24 inches, we have that ( 2l + 2w = 24 ), so ( l + w = 12 ). We wish to maximize the area of the rectangle, "

**Animations**
- Sampling animation - shimmering sampling icon while evaluating the extended proposal.

---

### Frame 9 - Second proposal accepted
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l ) and the width of the rectangle be ( w ). Since the perimeter of the rectangle is 24 inches, we have that ( 2l + 2w = 24 ), so ( l + w = 12 ). We wish to maximize the area of the rectangle, "**
- Proposed text: *(none)*

**Animations**
- Candidate prefix accepted and committed animation - the new paragraph bolds and shimmers.
- Sampling animation - shimmering sampling icon after the acceptance.

---

### Frame 10 - Third proposal introduces calculus step
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l ) and the width of the rectangle be ( w ). Since the perimeter of the rectangle is 24 inches, we have that ( 2l + 2w = 24 ), so ( l + w = 12 ). We wish to maximize the area of the rectangle, "**
- Proposed text: " which because of the constraint can be expressed as ( A = lw = l(12 - l) = 12l - l^2 ). To find the maximum area, we take the derivative of ( A ) with respect to ( l ) and set it to zero:"

**Animations**
- Proposed candidate prefix animation - new calculus-focused text types onto the screen.

---

### Frame 11 - Sampling on calculus step
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l ) and the width of the rectangle be ( w ). Since the perimeter of the rectangle is 24 inches, we have that ( 2l + 2w = 24 ), so ( l + w = 12 ). We wish to maximize the area of the rectangle, "**
- Proposed text: " which because of the constraint can be expressed as ( A = lw = l(12 - l) = 12l - l^2 ). To find the maximum area, we take the derivative of ( A ) with respect to ( l ) and set it to zero:"

**Animations**
- Sampling animation - shimmering sampling icon while evaluating the calculus proposal.

---

### Frame 12 - Third proposal contracts
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l ) and the width of the rectangle be ( w ). Since the perimeter of the rectangle is 24 inches, we have that ( 2l + 2w = 24 ), so ( l + w = 12 ). We wish to maximize the area of the rectangle, "**
- Proposed text: " which"

**Animations**
- Contraction animation - deletes the calculus explanation back to the shorter prefix "which".

---

### Frame 13 - Sampling on shortened prefix
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l ) and the width of the rectangle be ( w ). Since the perimeter of the rectangle is 24 inches, we have that ( 2l + 2w = 24 ), so ( l + w = 12 ). We wish to maximize the area of the rectangle, "**
- Proposed text: " which"

**Animations**
- Sampling animation - shimmering sampling icon while reconsidering how to continue.

---

### Frame 14 - Final solution committed and celebrated
**Problem** Same as Frame 1.

**Solution view**
- Committed text: **"Let the length of the rectangle be ( l ) and the width of the rectangle be ( w ). Since the perimeter of the rectangle is 24 inches, we have that ( 2l + 2w = 24 ), so ( l + w = 12 ). We wish to maximize the area of the rectangle, which is ( A = lw ). Let ( l = 12 - w ) and plug into the area:  A = (12 - w)w  =>  A = 12w - w^2.  Now, we differentiate ( A ) with respect to ( w ):  A'(w) = 12 - 2w.  We wish to maximize ( A ), so we set ( A'(w) = 0 ), and solve for ( w ):  12 - 2w = 0  =>  w = 6.  Since ( l = 12 - w ), we have that ( l = 12 - 6 = 6 ). Therefore, the area of the rectangle is  A = lw = 6 \cdot 6 = \boxed{36}."**
- Proposed text: *(none - full solution is locked in)*

**Animations**
- Candidate prefix accepted and committed animation - final text locks in and shimmers.
- Correct solution has been found animation - entire solution receives a celebratory shimmer.
---
