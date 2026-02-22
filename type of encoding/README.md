📌 Categorical Encoding in Machine Learning

📖 Why Do We Need Encoding?

Machine learning models work with numbers, not text.

📖 Overview

Categorical Encoding is the process of converting categorical (text) data into numerical format so that machine learning models can understand it.

Categorical data is divided into two main types:

Nominal Data

Ordinal Data

🔹 1️⃣ Nominal Data (No Order)


Nominal data represents categories that do not have any natural order or ranking.

📌 Examples

Gender → Male, Female

Color → Red, Blue, Green

City → Chennai, Mumbai, Delhi

There is no logical comparison like:

Red > Blue ❌

Male > Female ❌

✅ Encoding Methods for Nominal Data

One-Hot Encoding

Dummy Encoding

Binary Encoding

Hash Encoding

Frequency Encoding

🔹 2️⃣ Ordinal Data (Has Order)

Ordinal data represents categories that have meaningful ranking or order.

📌 Examples

Satisfaction → Low < Medium < High

Size → Small < Medium < Large

Rating → 1 < 2 < 3 < 4 < 5

Here order matters:

High > Medium > Low ✅

✅ Encoding Methods for Ordinal Data

Label Encoding

Ordinal Encoding (Manual Mapping)

🔹 3️⃣ Supervised Encoding (Uses Target Variable)

These encoding methods use the target/output column during transformation.

✅ Methods

Target Encoding

Leave-One-Out Encoding

📊 Structured Overview
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
│   └── Ordinal Encoding (Manual)
│
└── Supervised Encoding (Uses Target)
    ├── Target Encoding
    └── Leave-One-Out Encoding
🎯 Key Takeaway

Nominal → Use One-Hot or similar techniques

Ordinal → Use Label or Ordinal Encoding

Supervised tasks → Consider Target Encoding carefully