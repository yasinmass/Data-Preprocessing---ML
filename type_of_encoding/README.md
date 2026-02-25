📌 <strong>Categorical Encoding in Machine Learning</strong>
<blockquote> 🔄 Converting categorical (text) data into numerical format so machine learning models can understand it. </blockquote> <hr>
📖 <strong>Why Do We Need Encoding?</strong>

Machine learning models work with <b>numbers</b>, not text.

Real-world datasets contain values like:

Gender → Male, Female

City → Chennai, Mumbai

Satisfaction → Low, Medium, High

Since models cannot process text directly, we convert them into numbers.
This process is called <b>Categorical Encoding</b>.

<hr>
🧠 <strong>Types of Categorical Data</strong>

Categorical data is divided into two main types:

<ul> <li><b>Nominal Data</b></li> <li><b>Ordinal Data</b></li> </ul> <hr>
🔵 1️⃣ <strong>Nominal Data (No Order)</strong>

Nominal data represents categories that <b>do NOT have any ranking or sequence</b>.

📌 Examples

Gender → Male, Female

Color → Red, Blue, Green

City → Chennai, Mumbai, Delhi

There is <u>no logical comparison</u>:

Red > Blue ❌

Male > Female ❌

✅ <strong>Encoding Methods for Nominal Data</strong>
<ul> <li>One-Hot Encoding</li> <li>Dummy Encoding</li> <li>Binary Encoding</li> <li>Hash Encoding</li> <li>Frequency Encoding</li> </ul> <blockquote> 💡 Most commonly used: <b>One-Hot Encoding</b> </blockquote> <hr>
🟢 2️⃣ <strong>Ordinal Data (Has Order)</strong>

Ordinal data represents categories that have a <b>meaningful ranking or order</b>.

📌 Examples

Satisfaction → Low < Medium < High

Size → Small < Medium < Large

Rating → 1 < 2 < 3 < 4 < 5

Here order matters:

<b>High > Medium > Low</b> ✅

✅ <strong>Encoding Methods for Ordinal Data</strong>
<ul> <li>Label Encoding</li> <li>Ordinal Encoding (Manual Mapping)</li> </ul>
📌 Example Mapping
<pre> {'Low': 0, 'Medium': 1, 'High': 2} </pre> <hr>
🟡 3️⃣ <strong>Supervised Encoding (Uses Target Variable)</strong>

These encoding methods use the <b>target/output column</b> during transformation.

They can improve performance but must be used carefully to avoid data leakage.

Risk of data leakage
📊 Structured Overview
```text
Categorical Encoding
│
├── Nominal Data (No Order)
│   ├── One-Hot Encoding
│   ├── Dummy Encoding
│   ├── Binary Encoding
│   ├── Hash Encoding
│   └── Frequency Encoding
│
├── Ordinal Data (Has Order)
│   ├── Label Encoding
│   └── Ordinal Encoding (Manual Mapping)
│
└── Supervised Encoding (Uses Target)
    ├── Target Encoding
    └── Leave-One-Out Encoding
```
🎯 <strong>Key Takeaways</strong>
<ul> <li>✔ If there is <b>NO order</b> → Use One-Hot Encoding</li> <li>✔ If there <b>IS order</b> → Use Label / Ordinal Encoding</li> <li>✔ For advanced tasks → Use Target Encoding carefully</li> </ul> <hr> <details> <summary><b>🚀 Quick Decision Guide (Click to Expand)</b></summary> <br> <table> <tr> <th>Situation</th> <th>Recommended Encoding</th> </tr> <tr> <td>No order in categories</td> <td>One-Hot Encoding</td> </tr> <tr> <td>Clear ranking exists</td> <td>Label / Ordinal Encoding</td> </tr> <tr> <td>Too many categories</td> <td>Binary / Hash Encoding</td> </tr> <tr> <td>Using target relationship</td> <td>Target Encoding</td> </tr> </table> </details> <hr>

⭐ Final Thought

Understanding the <b>type of categorical data</b> is more important than memorizing encoding techniques.
