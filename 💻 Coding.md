# LeetCode Cheat Sheet

## Sliding Window

### Longest Substring Without Repeating Characters
- **URL:** https://leetcode.com/problems/longest-substring-without-repeating-characters/
- **Difficulty:** Medium
- **Explanation:** Use a HashSet to track characters in the window. Move right pointer forward, adding characters. If right character is already in the set, remove left character and move left pointer until the duplicate is gone. Answer is the max window size seen.

### Longest Repeating Character Replacement
- **URL:** https://leetcode.com/problems/longest-repeating-character-replacement/
- **Difficulty:** Medium
- **Explanation:** Use a HashMap to count letter frequencies in the window. Add right pointer letter to map. If window is invalid (window size minus most frequent letter's frequency > k), remove left pointer letter from map and move left pointer right until window is valid again. Answer is the max valid window size.

# 🗺️ Senior Developer Roadmap

> [!quote] The Principle You don't need to know everything. You need to know things at the **right depth**, at the **right time**.

---

## 🎯 The Big Picture

```
T-SHAPED KNOWLEDGE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 Algorithms  Networking  Security  Systems  Architecture
                      ┃
                      ┃  Android + Kotlin
                      ┃  Product Thinking
                      ┃  System Design
```

**Goal:** Google SWE III (London) → Senior Android Engineer

---

## ⚡ Phase 1 — Interview Gate (Now → 3 months)

> [!warning] Highest Priority This directly gates your next opportunity. Everything else waits.

### Algorithms & Data Structures

- [ ] **Arrays & Hashing** — NeetCode 150
    - [ ] Two Sum, Group Anagrams, Top K Frequent
    - [ ] Product of Array Except Self, Valid Sudoku
- [ ] **Two Pointers**
    - [ ] Valid Palindrome, 3Sum, Container With Most Water
- [ ] **Stack**
    - [ ] Valid Parentheses, Min Stack, Daily Temperatures
- [ ] **Sliding Window**
- [ ] **Binary Search**
- [ ] **Linked Lists**
- [ ] **Trees & BST**
- [ ] **Graphs** ← Google loves these
- [ ] **Dynamic Programming** ← hardest, start early
- [ ] **Heaps & Priority Queues**

### System Design (for SWE III)

- [ ] Design a fitness tracking system (relevant to Spiko)
- [ ] Design a notification service
- [ ] Design a feed system
- [ ] Read: _System Design Interview_ — Alex Xu
- [ ] Study: CAP theorem, consistent hashing, load balancing

### Coding Practice Targets

|Week|Problems|Focus|
|---|---|---|
|1-2|20|Arrays, Hashing, Two Pointers|
|3-4|20|Stack, Sliding Window, Binary Search|
|5-6|20|Linked Lists, Trees|
|7-8|20|Graphs, DP intro|
|9-12|30|Mixed, timed practice|

---

## 🤖 Phase 2 — Android Mastery (Parallel, ongoing)

> [!tip] Context-Driven Learning Go deep when you hit a real problem in Spiko or at work. Don't study in a vacuum.

### Kotlin Language

- [ ] Coroutines internals (how suspension actually works)
- [ ] Flows — cold vs hot, StateFlow vs SharedFlow
- [ ] Sealed classes, inline functions, reified generics
- [ ] Extension functions, delegation patterns
- [ ] KMP — Kotlin/Native compilation model

### Jetpack Compose

- [ ] Recomposition internals — when and why it triggers
- [ ] `remember` vs `rememberSaveable` vs ViewModel state
- [ ] Custom layouts and `Modifier` internals
- [ ] Side effects — `LaunchedEffect`, `DisposableEffect`, `SideEffect`
- [ ] Performance: `derivedStateOf`, stability, `@Immutable`

### Architecture & Patterns

- [ ] Clean Architecture layers (Data → Domain → Presentation)
- [ ] MVVM vs MVI — tradeoffs
- [ ] Dependency Injection with Hilt
- [ ] Repository pattern
- [ ] Use cases / Interactors

### Android Internals (go deep when relevant)

- [ ] Activity/Fragment lifecycle in detail
- [ ] ViewModel survival — `onSaveInstanceState` vs ViewModel
- [ ] Binder IPC — how Android processes communicate
- [ ] ART runtime — how Kotlin/JVM bytecode runs
- [ ] Background work — WorkManager, Foreground Services

---

## 🌐 Phase 3 — Breadth Layer (Absorb over 1-2 years)

> [!info] Learn When It Becomes Relevant Don't force these. Let real problems pull you in.

### Networking

- [ ] TCP/IP model — enough to debug weird API issues
- [ ] HTTP/2 vs HTTP/3
- [ ] WebSockets — relevant for real-time features
- [ ] DNS, CDNs — how your Spiko backend reaches users
- [ ] TLS handshake at a conceptual level

### Security

- [ ] HTTPS / TLS — how certificates work
- [ ] OAuth 2.0 + JWT — you'll implement these
- [ ] RSA at a conceptual level (asymmetric encryption)
- [ ] OWASP mobile top 10 — directly applicable to Spiko
- [ ] Secure storage on Android (EncryptedSharedPreferences, Keystore)

### Computer Systems

- [ ] Memory: stack vs heap, garbage collection (ART's GC)
- [ ] Processes vs threads vs coroutines
- [ ] CPU caching — why data locality matters
- [ ] _CS:APP_ — read when you want to go deep, not as a prerequisite

### Databases

- [ ] SQL fundamentals + query optimization
- [ ] Indexing — why queries are slow without it
- [ ] Room / SQLDelight internals
- [ ] NoSQL tradeoffs (relevant to Spiko's backend choices)

---

## 🏗️ Phase 4 — Cross-Platform Awareness (Background)

> [!note] You Already Have Good Intuition Here This context helps you make architectural decisions, not just code.

- [ ] KMP — extracting shared logic from your Compose app
- [ ] Flutter rendering model — Skia/Impeller
- [ ] React Native new architecture — JSI + Fabric
- [ ] SwiftUI basics — enough to collaborate with iOS devs
- [ ] SKIE library — Kotlin/Swift coroutine interop

---

## 📈 Spiko as a Learning Vehicle

> [!success] Your Best Teacher 50k users means real problems. Use every Spiko challenge as a learning trigger.

|Spiko Problem|What to Learn|
|---|---|
|Slow API calls|Networking, caching strategies|
|Auth implementation|OAuth, JWT, secure storage|
|Push notifications|FCM, background processing|
|Offline support|Room, sync strategies, conflict resolution|
|Performance issues|Compose recomposition, profiling tools|
|Scaling backend|System design, databases|
|KMP port|Kotlin/Native, Swift interop|

---

## 🧠 Meta-Skills (What Actually Makes You Senior)

These aren't things you study. They accumulate through building.

- **Judgment** — knowing which layer a problem lives in
- **Debugging intuition** — forming hypotheses fast
- **Reading code** — understanding unfamiliar codebases quickly
- **Communication** — explaining tradeoffs clearly
- **Saying no** — knowing what _not_ to build

---

## 📚 Core Reading List

|Book|Priority|When|
|---|---|---|
|_NeetCode 150_|🔴 High|Now|
|_System Design Interview_ — Alex Xu|🔴 High|Now|
|_Clean Architecture_ — Uncle Bob|🟡 Medium|After interviews|
|_Kotlin in Action_|🟡 Medium|Parallel|
|_CS:APP_ — Bryant & O'Hallaron|🟢 Low|When curious|
|_Designing Data-Intensive Applications_|🟡 Medium|Phase 3|

---

## ✅ Weekly Rhythm

```
Mon - Wed   → LeetCode (2-3 problems/day)
Thu         → System design study / mock
Fri         → Android deep dive OR Spiko feature
Sat         → LeetCode contest OR review weak areas  
Sun         → Light reading, planning next week
```

---

## 🔗 Related Notes

- [[Spiko Architecture]]
- [[NeetCode Progress Tracker]]
- [[Google Interview Prep]]
- [[Android Internals]]
- [[KMP Migration Plan]]