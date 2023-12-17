React Interview Questions & Answers


1. ## Differentiate between Real DOM and Virtual DOM.
# Real DOM vs Virtual DOM

## Real DOM (Document Object Model)

**Definition:**

The Real DOM is a tree-like structure of objects that represents the structure of a document. It is the actual, physical, and hierarchical structure in memory that the browser creates when an HTML document is loaded.

**Performance:**

- Manipulating the Real DOM is slower, especially when dealing with a large number of elements.
- Directly updating the Real DOM triggers reflow and repaint operations, which can be resource-intensive.

**Operations:**

- Any changes to the Real DOM cause the entire tree or a significant portion of it to be recalculated and redrawn.

**Rendering:**

- Changes to the Real DOM are immediately reflected in the browser window.

## Virtual DOM

**Definition:**

The Virtual DOM is an in-memory representation of the Real DOM elements. It is a lightweight copy of the Real DOM kept in memory and is synced with the Real DOM through a process called reconciliation.

**Performance:**

- Manipulating the Virtual DOM is faster than the Real DOM because it is an abstraction and doesn't directly affect the screen.

**Operations:**

- Changes are first made to the Virtual DOM rather than the Real DOM.
- Diffing (comparing) is performed to identify the differences between the current Virtual DOM and the previous one.

**Rendering:**

- Only the specific differences identified during the diffing process are applied to the Real DOM, minimizing the amount of reflow and repaint operations.

## বাংলায়

### রিয়েল ডম (ডকুমেন্ট অবজেক্ট মডেল)

**সংজ্ঞা:**

রিয়েল ডম হল একটি অবজেক্টের ট্রি-লাইক স্ট্রাকচার, যা একটি ডকুমেন্টের স্ট্রাকচার প্রতিষ্ঠান করে। এটি হল একটি ডকুমেন্ট লোড করা হলে ব্রাউজার যখন তা তৈরি করে তখন অবস্থানবদ্ধ, বাস্তব এবং হায়ারারকী স্ট্রাকচার।

**পারফরম্যান্স:**

- রিয়েল ডম সহ কাজ করা দ্রুত হলো না, সহজেই বলতে গেলে বলা যায় না, এসপেসিয়ালি যখন একটি বড় সংখ্যক উপাদানের সাথে কাজ করা হয়।

**অপারেশন:**

- রিয়েল ডমে যেকোনও পরিবর্তন সংবাদ বা বড় অংশ পুনরায় গণনা এবং পুনরায় আঁকারজুঁকা হতে পারে।

**রেন্ডারিং:**

- রিয়েল ডমে যেকোনও পরিবর্তন তা তারা তা ব্রাউজার উইন্ডোতে অবাধ্য়কভাবে প্রতিফলিত করে।

### ভার্চুয়াল ডম

**সংজ্ঞা:**

ভার্চুয়াল ডম হল রিয়েল ডম উপাদানগুলির মধ্যে সংগ্রহিত একটি ইন-মেমোরি প্রতিনিধিতা। এটি রিয়েল ডমের লাইটওয়েট কপি, যা মেমোরিতে রাখা হয় এবং এটি রিয়েল ডমের সাথে একটি পৃক্তি করার মাধ্যমে ইতিমধ্যে সিঙ্ক করা হয়।

**পারফরম্যান্স:**

- ভার্চুয়াল ডম সহ কাজ করা রিয়েল ডম থেকে দ্রুত হয়, কারণ এটি একটি অভ্যন্তরীণ হওয়া এবং প্রদর্শন করতে না হওয়া একটি সংগঠিত এবং দ্রুত স্ক্রিনে প্রত্যাবর্তন হয় না।

**অপারেশন:**

- পরিবর্তনগুলি প্রথমে ভার্চুয়াল ডমে হয়, রিয়েল ডমে না।
- প্রথম প্রিয় ডম এবং পূর্ববর্তী ভার্চুয়াল ডম মধ্যে পার্থক্যগুলি চিহ্নিত করার জন্য ডিফিং (তুলনা) করা হয়।

**রেন্ডারিং:**

- ডিফিং প্রক্রিয়ার সময় চিহ্নিত হয়নি তার পূর্বের ভার্চুয়াল ডমে, শুধুমাত্র পুনরায় আঁকার এবং রিপেইন্ট অপারেশনগুলি এবং যাচাই করে যে তা রিয়েল ডমে আবার প্রয়োজন।
