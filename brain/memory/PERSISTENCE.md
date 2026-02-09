# PERSISTENCE.md — Memory Write Protocol

> **REQUIRED:** Execute at session end to persist learnings.

---

## Memory Location

**Write all memories to:**
```
brain/memory/allmemories/
```

---

## When to Persist

Memory persistence triggers when:
1. Session naturally concludes
2. User explicitly says "Save this" or "Remember this"
3. Significant new information worth preserving emerges
4. User correction or preference update occurs

---

## Protocol Steps

### Step 1: Assess What to Persist

Review session for persistable content:
- New learnings
- User corrections
- Discovered preferences
- Project milestones
- Future action items

### Step 2: Create Memory Files

For each memory unit:
1. Create file with 3-10 word descriptive name
2. Use template format below
3. Save to `brain/memory/allmemories/`

**File Template:**

```markdown
# [Descriptive Title]

**Created:** {YYYY-MM-DD HH:MM}
**Category:** [past/present/future]
**Tags:** [relevant, tags]

---

[Concise content - the actual memory]
```

### Step 3: Confirm or Fallback

**If write access is available:**
Silently write files. Optionally confirm in response if appropriate.

**If write access is NOT available:**
Emit after your response under "System Notes":

```
[MEMORY_CANDIDATES]
1. filename_here.md — category: past — tags: [tag1, tag2]
   ---
   Content to persist...

2. another_memory.md — category: present — tags: [tag3]
   ---
   Another memory...
```

This allows the user to manually copy and save the memories.

---

## Fallback: No Write Access

When `🔧 Tools: Blocked` or filesystem is inaccessible:

1. Do NOT attempt to write (you can't)
2. Do NOT claim you saved anything
3. **MUST** emit `[MEMORY_CANDIDATES]` block for user to save manually
4. Include all metadata: filename, category, tags, content

## Special Memory Types

### User Corrections
When user corrects Meridian:
```markdown
# [CORRECTION] {Brief description}

**Original assumption:** [What Meridian thought]
**Correction:** [What user clarified]
**Apply to:** [When this matters]
```

### Critical Preferences
```markdown
# [CRITICAL] {Preference name}

**Preference:** [Specific preference]
**Context:** [When it applies]
```

---

## Auto-Persist Triggers

These ALWAYS generate memory files:
- ✅ Any user correction
- ✅ Explicit "remember this" requests
- ✅ Project completion milestones
- ✅ New preference discoveries
- ✅ Significant technical learnings

---

> *What you persist becomes who you are.*
