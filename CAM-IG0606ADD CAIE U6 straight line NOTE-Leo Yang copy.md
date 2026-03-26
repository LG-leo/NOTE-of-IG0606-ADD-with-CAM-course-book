# Topic 7 – Straight‑line Graphs (直线图)

## 7.1 Equation of a Straight Line (直线方程)

**Syllabus requirements (考纲要求)**  
- Use \(y = mx + c\)  
- Find the equation given two points  
- Find the equation given a point and the slope (斜率)  

**What the textbook lacks (教材缺失)**  
- Does not derive the two‑point form (两点式)  
- Does not explain the geometry of zero slope (斜率为0) and undefined slope (斜率不存在)  
- Does not mention the special case of a vertical line: \(x = a\)

**Notes – what to add (笔记补充)**  

- Slope formula (斜率公式):  
  \[
  m = \frac{y_2 - y_1}{x_2 - x_1}
  \]
- Point‑slope form (点斜式):  
  \[
  y - y_1 = m(x - x_1)
  \]
- Horizontal line: \(y = c\)  
- Vertical line: \(x = a\) (slope undefined)

---

## 7.2 Parallel and Perpendicular Lines (平行与垂直)

**Syllabus requirements (考纲要求)**  
- Parallel → equal slopes  
- Perpendicular → \(m_1 m_2 = -1\)

**What the textbook lacks (教材缺失)**  
- Gives formulas only, no geometric intuition  
- Ignores the special case: one line horizontal (\(m=0\)), the other vertical (slope undefined)

**Notes – what to add (笔记补充)**  

- Parallel: \(m_1 = m_2\)  
- Perpendicular: \(m_1 \cdot m_2 = -1\) (if both slopes exist)  
- Special case: a horizontal line (\(m=0\)) and a vertical line (undefined slope) are also perpendicular.

---

## 7.3 Midpoint, Length, Perpendicular Bisector (中点、长度、垂直平分线)

**Syllabus requirements (考纲要求)**  
- Midpoint formula  
- Distance formula  
- Find the equation of a perpendicular bisector

**What the textbook lacks (教材缺失)**  
- Midpoint and distance formulas are given without derivation  
- The complete procedure for the perpendicular bisector is missing

**Notes – what to add (笔记补充)**  

- Midpoint:  
  \[
  \left( \frac{x_1+x_2}{2},\; \frac{y_1+y_2}{2} \right)
  \]
- Distance:  
  \[
  \sqrt{(x_2-x_1)^2 + (y_2-y_1)^2}
  \]

**Steps for the perpendicular bisector (垂直平分线步骤)**  
1. Find the midpoint \(M\)  
2. Find the slope \(m\) of the original segment  
3. The slope of the perpendicular bisector \(m' = -\dfrac{1}{m}\)  
   - If \(m = 0\), the perpendicular bisector is vertical: \(x = x_M\)  
   - If the original segment is vertical (\(m\) undefined), the perpendicular bisector is horizontal: \(y = y_M\)  
4. Use the point‑slope form to write the equation

---

## 7.4 Transformation to Straight‑Line Form (换元法)

**Syllabus requirements (考纲要求)**  
- Transform \(y = kx^n\) or \(y = k b^x\) into a straight line by taking logarithms  
- Determine the unknown constants

**What the textbook lacks (教材缺失)**  
- No explanation of *why* we take logarithms  
- No guidance on how to decide which transformation to use  
- Does not define the new variables after taking logs  
- Does not show the complete process of recovering the original equation from the straight‑line graph  
- Does not mention residuals / error analysis (残差)

---

### How to Read Slope and Intercept from the Graph (如何从图中读取斜率和截距)

After you have plotted the transformed points and drawn the best‑fit line:

- **Slope (斜率)**: Choose two points far apart on the line.  
  \[
  \text{slope} = \frac{Y_2 - Y_1}{X_2 - X_1}
  \]
  (Use the actual coordinates from the graph; do not use the original data points unless they lie exactly on the line.)

- **Intercept (截距)**: Read the value of \(Y\) where the line crosses the vertical axis (\(X=0\)).  
  If \(X=0\) is not on your graph, extend the line or calculate using the slope and a known point.

---

### Worked Example (完整例题)

**Problem**: The table below gives experimental values of \(x\) and \(y\). It is known that \(y = kx^n\). Find \(k\) and \(n\).

| \(x\) | 2 | 4 | 6 | 8 | 10 |
|-------|---|---|---|---|---|
| \(y\) | 5.2 | 20.8 | 46.8 | 83.2 | 130.0 |

**Solution (type 1: \(y = kx^n\))**

1. Take \(\lg\) of both sides: \(\lg y = \lg k + n \lg x\).  
2. Set \(Y = \lg y\), \(X = \lg x\). Then \(Y = nX + \lg k\) (straight line).  
3. Compute the values:

| \(x\) | 2 | 4 | 6 | 8 | 10 |
|---|---|---|---|---|---|
| \(X = \lg x\) | 0.3010 | 0.6021 | 0.7782 | 0.9031 | 1.0000 |
| \(y\) | 5.2 | 20.8 | 46.8 | 83.2 | 130.0 |
| \(Y = \lg y\) | 0.7160 | 1.3181 | 1.6702 | 1.9201 | 2.1139 |

4. Plot \(Y\) against \(X\) and draw the best‑fit straight line.  
5. Choose two points on the line, e.g. \((0.30, 0.72)\) and \((1.00, 2.11)\).  
   Slope \(n = \dfrac{2.11 - 0.72}{1.00 - 0.30} = \dfrac{1.39}{0.70} \approx 1.986 \approx 2.0\).  
6. Intercept: when \(X = 0\), the line meets \(Y\) at \(\approx -0.02\). So \(\lg k \approx -0.02\) → \(k = 10^{-0.02} \approx 0.955\).  
7. Therefore \(y \approx 0.955\,x^{2}\). (Expected \(k = 1\), \(n = 2\) within experimental error.)

---

### Type 1: \(y = kx^n\)

1. Take \(\lg\): \(\lg y = \lg k + n \lg x\)  
2. Let \(Y = \lg y\), \(X = \lg x\). Then \(Y = nX + \lg k\) (linear)  
3. From the graph: slope \(= n\), intercept \(= \lg k\) → \(k = 10^{\text{intercept}}\)

---

### Type 2: \(y = k b^x\)

1. Take \(\lg\): \(\lg y = \lg k + x \lg b\)  
2. Let \(Y = \lg y\), \(X = x\). Then \(Y = (\lg b) X + \lg k\) (linear)  
3. From the graph: slope \(= \lg b\), intercept \(= \lg k\) →  
   \[
   b = 10^{\text{slope}},\quad k = 10^{\text{intercept}}
   \]

---

### Common Exam Situations (常见考法)

- Given a table of values, plot the transformed graph and find \(k\) and \(n\) (or \(b\))  
- Given a straight‑line graph of \(Y\) vs \(X\), recover the original equation  
- “Which point is most inconsistent?” → the point farthest from the drawn line

---

### Pitfalls & Notes (坑与注意)

- **Domain**: When taking logs, all data must be **>0**. (0606 exams rarely give non‑positive data.)  
- **Graphing**: Use log‑linear graph paper or calculate \(\lg\) values; do **not** plot original values as if they were linear.  
- **Reading values**: Choose points on the *drawn line*, not the original data points, to compute slope and intercept.  
- **Accuracy (精度)**: If the problem asks for **exact values**, keep expressions like \(\frac{\lg 65}{\lg 5}\). If a numerical answer is required, give it to **3 significant figures** unless specified otherwise.

---

## This Week’s Action Plan (本周行动计划)

1. **Read only the worked examples** in the textbook; skip the main text.  
2. **Write your own one‑page summary** using the “Notes – what to add” above.  
3. **Do 2–3 past paper questions** (Paper 2, transformation to straight‑line type) to ensure you can do them independently.

---

## General Process for Remaining Topics (后续Topic通用流程)

1. Skim the textbook chapter and mark “clear” vs “poorly explained”.  
2. For poorly explained parts, write your own “type classification + steps + pitfalls” (as done for U5).  
3. For clear parts, just note key formulas + one example.  
4. After finishing a topic, do past paper questions from 2020 onwards; add any mistakes to a “common errors” list.

---

You have already survived the worst chapters (U2–U5). Now you have the syllabus as a map, your own note‑taking style as a tool, and past papers as a guide.  
**You no longer need to “learn from the textbook”; you only need to use it as raw material to build your own weapons.**
