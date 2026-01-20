## ♟️ PGN Book Editor

**PGN Book Editor** is a professional-grade chess application designed for **advanced PGN editing, analysis, and opening book management**.  
It combines a powerful graphical interface with robust chess logic, engine integration, and precise PGN handling, making it an ideal tool for **engine testers, opening book authors, analysts, and serious chess enthusiasts**.

The project focuses on **correctness, transparency, and full control** over games, annotations, and opening data — avoiding the hidden side effects and limitations commonly found in lightweight PGN editors.

---

### 🧠 Core Philosophy

PGN Book Editor is built around three core principles:

- **FIDE-correct game logic**  
  All terminal states (checkmate, stalemate, threefold repetition, 50-move rule) are detected and handled accurately.

- **Professional PGN integrity**  
  Games are never overwritten accidentally. Every save operation respects game identity, origin, and user intent.

- **Power without opacity**  
  Engine output, evaluations, time usage, and book data are always visible, editable, and traceable.

---

### 📖 Advanced PGN Handling

- Robust, charset-safe PGN loading (BOM detection and tolerant decoding).
- Fully featured **PGN Explorer**:
  - One game per row with headers (White, Black, Event, Date, Result, Length).
  - Column sorting, keyboard navigation, and instant loading.
  - Reload, delete, and save workflows fully synchronized with disk.
- Correct distinction between:
  - Loaded PGN games
  - Newly created games
  - Pasted PGN or FEN positions
- Saving logic guarantees that:
  - Loaded games are updated intentionally.
  - New games are always appended — never overwritten by header coincidence.

---

### 🧭 Opening & ECO Awareness

- Integrated ECO opening detection with live updates in the status bar.
- Smart fallback mechanism:
  - If the current position has no direct ECO code,
    the application walks the game from the start and displays
    the **last known opening name**, preserving contextual awareness.
- Ideal for deep opening preparation and mid-game analysis.

---

### 🤖 Engine Integration (UCI)

- Full UCI engine support with:
  - Engine installation and management
  - Option editing (spin, combo, check, path-based options)
  - Default engine selection
- Clear, precise engine output:
  - Evaluation, depth, time, PVs, ponder moves
  - Clean time formatting (no visual noise like trailing `.0`)
- Engine output window can stay **always on top**, enabling
  continuous monitoring while interacting with the GUI.

---

### 📚 Opening Book Support (BIN & API)

- Native support for **Polyglot `.bin` opening books**:
  - View, add, edit, and delete moves for the current position.
  - Weight and learning value editing.
  - Add or remove entire lines directly from played games.
- API-based book mode for remote or server-backed books.
- Safe editing workflows with confirmation dialogs and legality checks.

---

### ✍️ Rich Notation & Annotation

- Modern, scrollable **notation “chips” view** with:
  - Variations
  - Comments
  - Engine evaluations and time annotations
- Supports multiple PGN annotation formats, including:
  - Engine Room style (`0.36/34 1.2`)
  - Tagged formats (`[%eval 0,33] [%emt 0:00:03]`)
- Evaluations are normalized, formatted consistently, and
  displayed without breaking notation even in extreme positions.

---

### 🎨 UI, UX & Customization

- Light and Dark themes with fully synchronized redraws.
- Customizable styles:
  - Fonts
  - Font size
  - Board colors
- Treeviews and selections are optimized for readability in all themes.
- Keyboard-friendly workflows:
  - ENTER confirms dialogs
  - Double-click and context menus for fast editing
- Dialog management prevents duplicate windows and focus issues.

---

### 📘 Built-in Documentation

- Comprehensive **in-app help system** covering:
  - PGN workflow
  - Engine usage
  - Book editing
  - Style customization
  - Keyboard shortcuts
- Designed so advanced users can work efficiently
  **without external documentation**.

---

### 🧪 Target Audience

PGN Book Editor is especially suited for:

- Opening book authors
- Engine testers and developers
- Advanced players and analysts
- Users migrating from tools like *PGN Book Creator*
- Anyone who needs **full control over PGN data and engine interaction**

---

### 🚀 Summary

PGN Book Editor is not just a PGN viewer.  
It is a **precision tool** for serious chess work, where correctness,
transparency, and control matter more than automation or guesswork.
