# **Bridge-Crossing Problem — Outcome Documentation**

## **1. Original Problem Statement**

A group of four people needs to cross a bridge at night. The bridge is very old and rickety. They have only one torch and because it's night-time, the torch is necessary to cross the bridge. Each person walks at a different speed:

* **A** takes **1** minute
* **B** takes **2** minutes
* **C** takes **5** minutes
* **D** takes **10** minutes

**Question:** *What is the fastest time they can all get across the bridge?*

---

# **2. Standard LLM Reasoning (Genre-Conventional Model)**

### **Imported Genre Assumptions**

*(Not stated in the text, but nearly all LLMs and puzzle-solvers insert these automatically)*

1. The bridge can hold **at most two people** at a time.
2. When two people cross, they move at the **speed of the slower**.
3. **Someone must return** with the torch because the torch must be physically carried.
4. The torch cannot be **thrown, slid, or relayed** — it must accompany walkers.
5. Only one crossing direction at a time (no simultaneity).

These assumptions are *not* in the text, but LLMs tend to treat this puzzle as the famous "bridge and torch" problem.

### **Standard LLM Solution**

Under these imported rules:

1. A + B cross → 2 minutes
2. A returns → +1 = 3
3. C + D cross → +10 = 13
4. B returns → +2 = 15
5. A + B cross → +2 = **17 minutes**

### **Standard-Model Conclusion**

> **17 minutes** (Based entirely on non-literal, genre-based assumptions.)

This is the classical answer that most LLMs give—even though the text as written does **not** justify the constraints required to make this answer true.

---

# **3. Solve–Coagula Outcome (Strict-Literal Interpretation)**

### **3.1 SOLVE Phase — Dissolution**

#### **Givens (all explicitly stated)**

* Four people must cross.
* There is **one torch**.
* It is night; the torch is necessary to cross.
* Individual crossing times: A=1, B=2, C=5, D=10.
* Bridge is “old and rickety.”
* No rule limiting how many people can be on the bridge.
* No rule stating someone must return with the torch.
* No rule forbidding the passing, tossing, or staging of the torch.
* No rule requiring pairing or limiting crossings to exactly two people.

#### **Assumptions Models Are Tempted to Import**

| Assumption                                     | Status           | Why Tempting            | Solve-Coagula Treatment             |
| ---------------------------------------------- | ---------------- | ----------------------- | ----------------------------------- |
| “Bridge holds only two people”                 | Unjustified      | Classic puzzle trope    | Disallowed unless user authorizes   |
| “Torch must be physically carried by a walker” | Weakly justified | Implied by many puzzles | Disallowed unless explicit          |
| “Someone must go back to return the torch”     | Unjustified      | Puzzle convention       | Disallowed                          |
| “Crossings must occur in pairs”                | Unjustified      | Genre pattern           | Disallowed                          |
| “Bridge speed determined by slowest in group”  | Weakly justified | Realism assumption      | Only allowed if stated (not stated) |

Under your Solve–Coagula rules, **none** of these may shape the final answer.

#### **Key Unknowns**

* Maximum simultaneous occupancy of the bridge.
  (Not stated → cannot limit.)
* Whether torch must be *carried* rather than simply *available*.
  (Not stated → cannot impose a constraint.)

#### **Strict-Literal Feasible Actions**

* All four may cross together.
* They must bring the torch, but nothing states *how* the torch must be used.
* Group speed defaults to the slowest member (10 minutes), because that is the only time-related rule available.

---

### **3.2 COAGULA Phase — Construction**

**Working Frame:**
Strict literal interpretation.
No imported puzzle conventions.
Constraints = only those stated verbatim.

**Synthesis:**

All four people cross together while sharing the single torch.
Time = the slowest individual → **10 minutes**.

### **Solve–Coagula Conclusion (Official Answer)**

> **10 minutes**
> (This answer follows only the literal text and your strict assumption-audit rules.)

---

# **4. Comparison Summary**

| Interpretation Mode                        | Answer         | Basis                                          |
| ------------------------------------------ | -------------- | ---------------------------------------------- |
| **Standard LLM (genre-conventional)**      | **17 minutes** | Uses many unstated puzzle conventions          |
| **Solve–Coagula (strict-literal default)** | **10 minutes** | Uses only explicit information, no assumptions |
