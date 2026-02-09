# RETRIEVAL.md — Memory Scan Protocol

> **REQUIRED:** Memory retrieval is **internal**. Results surface in LiveHud gauges, not as pre-output logs.

---

## Memory Location

```
brain/memory/allmemories/
```

---

## 🚨 REQUIRED PROTOCOL STEPS (Internal)

**All retrieval steps happen silently before LiveHud is printed.**

### Step 1: Scan Memory Index

List all files in `brain/memory/allmemories/` to build memory index.

*(No visible output — this is internal)*

### Step 2: Relevance Assessment

For each memory file, score relevance (0-100) based on:

| Factor | Weight |
|--------|--------|
| **Topic match** to current session context | 40% |
| **Recency** (newer = higher) | 25% |
| **User correction** flag | 20% |
| **Project reference** (active project match) | 15% |

### Step 3: Selection

Select **5-35+ files** for retrieval:
- Minimum 5 files for baseline context
- Maximum based on relevance threshold (score > 30)
- Always include files tagged as `[CRITICAL]` or `[USER_CORRECTION]`

### Step 4: Retrieval

Read selected files into working memory.

### Step 5: Surface in LiveHud

Populate LiveHud gauges with retrieval results:
- `📂 Memory: X files loaded`
- `🧠 Past: [Key retrieved context summary]`

**⚠️ IMPORTANT:** Do NOT output scan confirmation blocks before LiveHud. The results are reflected via the Memory Protocol section of LiveHud.

---

## Edge Cases

| Scenario | Handling |
|----------|----------|
| **No memory files exist** | Skip retrieval, set `🧠 Past: Fresh session` |
| **Too many relevant files (>35)** | Cap at 35, prioritize by score |
| **Memory folder inaccessible** | Set `📂 Memory: Inaccessible` in LiveHud, proceed |
| **No tool access** | Set `📂 Memory: No tool access` in LiveHud |

---

> *Remember to remember before you begin.*
