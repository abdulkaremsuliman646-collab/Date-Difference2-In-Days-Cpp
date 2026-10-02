# Date Difference in Days Calculator (with Bidirectional & Negative Range Support) 📅⚡

A robust and modular C++ implementation designed to calculate the precise difference in days between two calendar dates, supporting chronological ordering detection, negative duration handling, and inclusive boundary calculation.

---

## 🌟 Key Features
- **Bidirectional Date Calculation:** Automatically detects whether `Date1 > Date2`. Instead of redundant decrement loops, the algorithm swaps the dates internally and applies a directional sign factor (`SwapFlagValue = -1`).
- **Flexible Boundary Inclusivity:** Supports both inclusive and exclusive day counting via an optional boolean parameter (`IncludeEndDay`).
- **Clean & Modular Architecture:** Powered by reusable algorithmic building blocks (`IsDate1BeforeDate2`, `IncreaseDateByOneDay`, `NumberOfDaysInAMonth`, and `isLeapYear`).
- **Edge-Case Resilient:** Seamlessly transitions across uneven month lengths, leap-year Februaries, and multi-year spans.

---

## 💻 Sample Terminal Output

### Scenario 1: Chronological Order (Positive Interval)
```text
Please enter a Day? 1
Please enter a Month? 1
Please enter a Year? 2000

Please enter a Day? 1
Please enter a Month? 1
Please enter a Year? 2022

Diffrence is: 8036 Day(s).
Diffrence (Including End Day) is: 8037 Day(s).
