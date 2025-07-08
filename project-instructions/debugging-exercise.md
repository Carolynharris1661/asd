# 🐞Debugging Exercise

Use the Chrome debugger to fix bugs and bring this broken animation back to life! Even if you don’t understand every line of the code at first, you’ll learn to trace errors, read messages, and step through the program using powerful developer tools.

---

## What You'll Learn

- How to use console messages to identify syntax and runtime errors
- How to recognize and correct common typos in code
- How to use breakpoints and the Chrome debugger to step through logic

**Table of Contents**

- [Overview](#overview)
- [Project Grading](#project-grading)
- [TODO 1: Find Extra, Missing, or Incorrect Symbols and Keywords](#todo-1-find-extra-missing-or-incorrect-symbols-and-keywords)
- [TODO 2: Find All Typos](#todo-2-find-all-typos)
- [TODO 3: Get the Circles Moving](#todo-3-get-the-circles-moving)
- [TODO 4: Fix Horizontal Movement](#todo-4-fix-horizontal-movement)
- [TODO 5: Fix Sticky Circles](#todo-5-fix-sticky-circles)
- [📤 Submit Your Work](#-submit-your-work)

---

# Overview

<img src="img/working.gif" alt="debugging demo gif">

In this project, the code is already written, but it’s broken! Your job is to find and fix the bugs using console errors and the Chrome debugger. The techniques used in the program may be new, but don’t worry. With careful observation and debugging tools, you’ll be able to trace through the logic and make everything work again.

---

## Push Reminder

To push to GitHub, enter the following commands in bash:

```bash
git add -A
git commit -m "saving debug exercise"
git push
```

## Project Grading

| Requirement                             | Description                                              | Points  |
| --------------------------------------- | -------------------------------------------------------- | ------- |
| **Fix all syntax and symbol errors**    | Identify incorrect or missing keywords and symbols       | 20      |
| **Correct all variable/function typos** | Locate undefined references using console stack traces   | 20      |
| **Get the circles to appear and move**  | Use the debugger to identify logic issues with rendering | 20      |
| **Enable horizontal movement**          | Debug position calculations and fix directional logic    | 20      |
| **Fix sticky bottom collision logic**   | Complete the bouncing behavior with accurate detection   | 20      |
|                                         | **Total**                                                | **100** |

# Lesson Steps

🔍 To begin your debugging journey, open the `asd-debugging-exercise` folder and launch the HTML file using Live Server. Then, press `F12` to open Chrome DevTools — your trusty magnifying glass for hunting down errors. You’ll be using both the **Console** and **Sources** tabs to solve the mystery.

Keep this tab open throughout your project, and check in after every change until you track down every bug! 🕵️‍♀️

> ## ⚠️ IMPORTANT
>
> **DO NOT** just go through deleting red squiggles! Some of the syntax may look strange but is completely correct. Rely on the **stack trace** and **step-through debugging** to guide your fixes; otherwise, you might “fix” something that was never broken.

**Why this matters:** This exercise teaches you to debug like a professional developer - using runtime error messages and systematic debugging rather than guessing.

**The right approach:**

1. ✅ Check browser console for error messages
2. ✅ Use Chrome debugger to step through code
3. ✅ Follow the specific guidance for each TODO
4. ❌ Don't edit code based on editor warnings alone

# TODO 1: Find Extra, Missing, or Incorrect Symbols and Keywords

## **TODO 1: Find Extra, Missing, or Incorrect Symbols and Keywords**

🎯 **Goal:** Use the developer tools console to locate and fix syntax issues caused by missing or incorrect symbols and keywords. Syntax errors can include:

- Missing or extra punctuation (brackets, parentheses, semicolons, commas)
- Misspelled JavaScript keywords (like `if`, `function`, `var`, etc.)
- Incorrect operators or symbols

---

### **Step-by-Step Instructions**

1. Open your project in Live Server and launch the **Chrome Developer Tools** (F12).
2. Go to the **Console** tab to view any error messages.
3. Use the console messages and stack traces to locate each of the following:
   - A misspelled keyword (e.g., `funtion`, `iff`, etc.)
   - A missing or extra symbol (such as a curly brace, parenthesis, or semicolon)
4. There are **FOUR** errors of this type in total. Fix each one carefully by using the debugger output rather than guessing.

> ⚠️ **Use the console to find each error.** If you try to hunt them down manually, you may miss one or break working code. The console is your most accurate source of truth.
>
> **NOTE:** Error messages sometimes point to the line after the actual problem. If the console indicates an error on a specific line, check that line and the line immediately before it.

---

<table style="width: 80%; margin-left: auto; margin-right: auto; border-collapse: collapse; margin-top: 15px; background-color: #2c2c2c; border: 1px solid #444; border-radius: 8px; overflow: hidden;">
  <tr>
    <th style="text-align: left; padding: 10px; background-color: #444; color: #e2e2e2; border-bottom: 1px solid #666;">
      💡 Review Important Concepts
    </th>
  </tr>
  <tr>
    <td style="padding: 10px; color: #e2e2e2;">
      <strong>⚠️ Syntax Errors:</strong> These prevent your code from running at all. Misspelled keywords, missing braces, or misplaced symbols are common causes.<br><br>
      <strong>🔧 Opening DevTools:</strong> Press <code>F12</code> or right-click → <code>Inspect</code> to access DevTools.<br><br>
      <strong>📋 Using the Console:</strong> The Console tab displays error messages and stack traces, which point you to the exact file and line where the error occurred.
    </td>
  </tr>
</table>

---

### ✅ **Check Your Work**

- Open the console in DevTools.
- If your fixes are successful, you should now see a **ReferenceError for `maXX`** in the console.
- **Do not move forward until this message appears.** It confirms you've cleared the first layer of errors.

<br><br><br><br>

## **TODO 2: Find All Typos**

🎯 **Goal:** Use the console to identify and fix typos in variable or function names that are causing runtime errors.

---

### **Step-by-Step Instructions**

1. Open your project with Live Server and keep the **Console** tab of DevTools open.
2. Look for **ReferenceErrors** that point to undefined variables or functions.
3. There are **THREE** such typos in total. These may include:
   - Misspelled variable names
   - Incorrect capitalization
   - Calling a function by the wrong name
4. Carefully correct each typo based on what the console messages are reporting and how you see these and similar terms spelled on other lines.

> ⚠️ **Don't assume the program is fixed just because something appears on the screen.** You may see some circles before this step is complete, but that does not mean all errors are resolved.

---

<table style="width: 80%; margin-left: auto; margin-right: auto; border-collapse: collapse; margin-top: 15px; background-color: #2c2c2c; border: 1px solid #444; border-radius: 8px; overflow: hidden;">
  <tr>
    <th style="text-align: left; padding: 10px; background-color: #444; color: #e2e2e2; border-bottom: 1px solid #666;">
      💡 Review Important Concepts
    </th>
  </tr>
  <tr>
    <td style="padding: 10px; color: #e2e2e2;">
      <strong>🐞 Runtime Errors:</strong> These occur while the program is running, often due to misspelled variables or undefined functions.<br><br>
      <strong>📌 Stack Traces:</strong> The console will show the function call history when an error occurs, helping you trace where the issue originated, even if the real bug is a few steps back.
    </td>
  </tr>
</table>

---

### ✅ **Check Your Work**

- Open the console in DevTools.
- You should **no longer see any ReferenceErrors**.
- If any ReferenceErrors are still present, **do not move forward** until they are resolved.
- > 💬 If you see a different kind of error instead, check with your instructor before continuing.

<br><br><br><br>

# TODO 3: Get the Circles Moving

🎯 **Goal:** Use the Chrome debugger to step through the program and discover why the circles aren’t appearing or moving.

---

### 🔎 Review Before You Begin

Before diving into the debugging steps, take a moment to familiarize yourself with the **DevTools control panel**:

<img src="img/panel.png" alt="DevTools control panel">

- Hover over each icon in Chrome’s **Sources** tab to learn what they do.
- Pay special attention to:
  - Resume script execution
  - Step into function
  - Step over next function call
  - Step out of current function

These will be your primary tools for navigating the code frame-by-frame.

---

### **Step-by-Step Instructions**

1. Open the **Sources** tab in DevTools and click on the `index.js` file to view your code.
2. Click on **line 92** (the start of the `update` function) to place a **breakpoint**. This function runs once per frame and controls all movement logic.

<img src="img/breakpoint.gif" alt="how to add a breakpoint gif">

3. Refresh the page. Your code should pause at the breakpoint.
4. Hover your mouse over the variables `i`, `maxCircles`, and `circles`. Take note of their current values.

> **💡 Why line 92?**  
> That `for` loop sets up how many times the circle logic runs. If `maxCircles` is wrong, this loop won't behave as expected.

5. Click the **Resume** button to continue execution and watch for changes.
6. Notice that `maxCircles` becomes `0` — this is the source of the issue. Now your task is to **track where that value is changed**.
7. Refresh the page and instead of resuming, try using the **Step Into** button to walk through the program one line at a time.
8. Watch for the moment where `maxCircles` is reassigned or manipulated. When you find the cause, fix it in the code.

> ⚠️ **Heads up:**  
> If you accidentally step into jQuery or external code, either hit the **Step Out** button or refresh the page and resume stepping again — you're only interested in _your_ code.

---

<table style="width: 80%; margin-left: auto; margin-right: auto; border-collapse: collapse; margin-top: 15px; background-color: #2c2c2c; border: 1px solid #444; border-radius: 8px; overflow: hidden;">
  <tr>
    <th style="text-align: left; padding: 10px; background-color: #444; color: #e2e2e2; border-bottom: 1px solid #666;">
      💡 Review Important Concepts
    </th>
  </tr>
  <tr>
    <td style="padding: 10px; color: #e2e2e2;">
      <strong>🔍 Debugging with Sources:</strong> The <code>Sources</code> tab lets you inspect and pause your code at any line to examine what's happening in real time.<br><br>
      <strong>⏱ Step-by-Step Execution:</strong> The debugger allows you to run code one line at a time. This makes it easy to observe when and how variables change — and catch errors that don’t throw messages.
    </td>
  </tr>
</table>

---

### ✅ **Check Your Work**

- Open your project with Live Server.
- When the program runs correctly, all the circles should:
  - Stick to the **left** side of the screen at first
  - Then slowly migrate to the **bottom** of the box
- **Do not move forward** until you see this exact behavior.

<br><br><br><br>

## **TODO 4: Fix Horizontal Movement**

🎯 **Goal:** Use breakpoints and the step-through debugger to identify why the circles are not moving left or right.

---

### **Step-by-Step Instructions**

> 💡 You may have already spotted this bug while working on TODO 3. If you’ve fixed it, you’re ahead, but if not, follow the steps below to uncover the issue.

1. Remove your previous breakpoint (line 92) by clicking it again in the **Sources** tab.
2. In the `update` function, examine the three function calls:
   - `moveCircle(...)`
   - `bounceCircle(...)`
   - `updateCircleOnScreen(...)` 

   *Which one seems most likely to handle horizontal motion?*
3. Place a **breakpoint** on that line.
4. Refresh the page to trigger the breakpoint.
5. Use the **Step Into** button to enter the function and examine what’s happening.
   - If you land inside jQuery or see unfamiliar code, click **Resume** and try again.
6. Look for missing or incorrect logic that would prevent left/right movement, then fix it.

> 🔁 **Reminder:** Because the `update` function runs every frame, your breakpoint will be hit again after you click **Resume**, allowing you to easily retry with a new approach.

---

<table style="width: 80%; margin-left: auto; margin-right: auto; border-collapse: collapse; margin-top: 15px; background-color: #2c2c2c; border: 1px solid #444; border-radius: 8px; overflow: hidden;">
  <tr>
    <th style="text-align: left; padding: 10px; background-color: #444; color: #e2e2e2; border-bottom: 1px solid #666;">
      💡 Review Important Concepts
    </th>
  </tr>
  <tr>
    <td style="padding: 10px; color: #e2e2e2;">
      <strong>🧠 Debugging with Intuition:</strong> As your experience grows, you’ll start narrowing down errors based on variable names, function roles, and logic structure — not just stack traces.<br><br>
      <strong>🗺 Strategic Breakpoints:</strong> Placing breakpoints in functions with names that suggest they handle the issue (e.g., <code>bounceCircle</code>) helps you skip irrelevant code and focus on likely problem areas.
    </td>
  </tr>
</table>

---

### ✅ **Check Your Work**

- Open your project with Live Server.
- When the program runs correctly, all the circles should:
  - No longer stick to the **left** side
  - But should still drop to the **bottom**
- **Do not move forward** until all circles move freely left and right without clinging to the wall.

<br><br><br><br>

## **TODO 5: Fix Sticky Circles**

🎯 **Goal:** Track down why the circles are sticking to the bottom of the screen instead of bouncing, and fix the logic causing it.

---

### **Step-by-Step Instructions**

1. Start with a clean slate by removing any previous breakpoints.
2. Return to the `update` function and once again examine the three key function calls:
   - `moveCircle(...)`
   - `bounceCircle(...)`
   - `updateCircleOnScreen(...)` 

   *Which one seems responsible for detecting and handling collisions?*
3. Place a **breakpoint** at the line you think is most relevant.
4. Refresh the page and use the **Step Into** button to begin walking through the logic.
5. Watch for any conditions or calculations that might be missing or incorrect — especially related to reversing direction on impact.
6. When you find the bug, fix the logic so the circles **bounce off** the bottom of the box instead of sticking to it.

> 💡 **Hint:** You’ve done this dance before. Rely on what you learned in TODO 4, and think carefully about which function actually handles boundary collisions.

---

<br>

## 📤 Submit Your Work

Make sure you save and submit your work regularly. These files are already being tracked by your GitHub repo, so you can commit and push with the following commands:

```bash
git commit -a -m "Finished Debugging project"
git push
```

✅ Once you’ve pushed your changes, check GitHub to confirm your updates appear in the repository.
