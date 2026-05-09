# John Smith

---

## Objective

Looking to find an internship or entry level position in Software Engineering, Automation or Systems Development.

---

## Summary

Passionate software engineer who began programming at age 7 and spent years honing skills across systems, graphics, audio, and language tooling. Holds two Associate degrees in Computer Science and Information Technology. Thrives in high-performance, fast-moving environments alongside world-class teams. Comfortable on the command line or in an IDE, language-agnostic across the whole stack, and quick to adopt modern tools including AI-assisted development.

---

## Education

**Folsom Lake College** — 2024–2026
- Associate of Science in Computer Science
- Associate of Science in Information Technology

**Folsom High School** — Graduated 2024

---

## Skills

**Languages:** C, C++, Go, Rust, Java, Python

**Operating Systems:**
- Linux — Excellent
- macOS — Proficient
- Windows — Proficient

---

## Areas of Expertise

**General Operating System Skills** (Windows, Mac, Linux)
- Common system configurations
- Subsystems (display, audio, text, input devices, etc.)
- Driver interfaces, file systems, process management

**Tools & Environment**
- CLI, Git, Make / CMake, GDB / LLDB, VS Code, SSH, AI Code Assist

---

## Computer Science Education & Skills

**Data Structures**
Lists (contiguous, linked, circular), Stack, Queue, Priority Queue, Prefix Tree, BST, Binary Space Partition, Hash Set / Hash Map, General & Bipartite Graphs

**Core Concepts**
- Complexity Analysis — Big O, best/worst/average case, time–space trade-offs
- Set Theory — union, intersection, complement, Cartesian products
- Graph Theory — BFS/DFS, shortest paths, connectivity, directed & undirected graphs
- Boolean Algebra — logic gates, truth tables, De Morgan's laws, Karnaugh maps
- CPU Architecture — instruction sets, registers, memory hierarchy, fetch-decode-execute cycle

**Wrappers, Interface Layers & APIs**
Thin wrapper design, handle-based resource APIs, versioned interface definitions, lifetime management, decoupling OS/vendor specifics from application code

---

## Major Projects

**Audio DSP (Digital Signal Processing) Programming** — Reaper + JSFX
Built a full suite of audio processors entirely from scratch — no libraries, no shortcuts. Implemented parametric EQ, dynamics processors (compressor, limiter, gate), and biquad IIR filters (low-pass, high-pass, band-pass), with real-time waveform and spectrum visualization.

**OpenGL Rendering Engine**
Designed and built a 3D rendering engine on top of OpenGL with a full scene graph, shader pipeline, and resource management system. Features hierarchical transforms, hot-reloadable shaders, reference-counted resource lifetimes, draw call batching, and a camera system with Phong lighting.

**Custom Compiler / Parser Engine + Custom Programming Language**
Wrote a complete compiler toolchain for an original programming language — from raw source text to executable output, with no parser frameworks. Includes a hand-written lexer, recursive-descent parser, typed AST, scope resolver, type checker, and code generator targeting a bytecode VM or native output.

**Binary / Text File Format Parsers**
Built low-level readers and writers for structured binary and text-based formats, designed to handle real-world edge cases without crashing. Covers endianness-aware byte handling, struct packing, streaming reads, INI/key-value text parsers, and error reporting with byte offset and line/column context.

---

## Layout & Design Spec

### Page Structure

```
[Header: name, headline, contact chips]
[Objective / Summary block — full width]
[Two-column grid]
  [Education strip — spans both columns, full width]
  [Left column]          [Right column: 260px]
  └ Programming Languages  └ Tools & Environment
  └ Major Projects         └ OS Subsystems & Config
  └ CS Education & Skills  └ Operating Systems
```

### Design System

- **Font:** -apple-system / SF Pro (Apple system font stack)
- **Palette:** White background, gray-100 blocks, gray-200 borders, gray-500 muted text, gray-700 body text, black headings
- **Border radius:** 10px (cards), 14px (blocks)
- **Max width:** 900px centered

### Blocks & Components

- **Section labels:** 11px, uppercase, 0.1em letter-spacing, gray-500
- **Blocks:** gray-100 background, 14px radius, 24px padding, 16px bottom margin
- **Subsection labels:** 11px, uppercase, 0.08em letter-spacing, gray-700, bordered top separator

### Programming Languages

- Grid of cards, auto-fill columns min 100px
- Each card: white background, border, centered, language name bold + small muted note beneath

### Major Projects

- Each project has an SF Symbol-style SVG icon (18×18) left of the title
- Title: 15px bold black
- Body: single paragraph — **bold hook sentence** followed by prose detail in gray-500
- Tags: pill badges below paragraph with 16px top margin
  - Dark pills: gray-500 background, white text
  - Light pills: white background, gray-300 border, gray-700 text
  - Font: 11px, padding: 2px 8px

### Operating Systems

- Proficiency bars: 4px tall, black fill on gray-200 track
- Linux (Excellent): 95% — listed first, full opacity
- macOS (Proficient): 70% — dimmed to 50% opacity
- Windows (Proficient): 70% — dimmed to 50% opacity

### Education Strip

- Full-width flex row spanning both grid columns
- Two cards side by side: Folsom Lake College (with degrees) + Folsom High School

---

### Mobile Layout (max-width: 680px)

**Section order:**
1. Programming Languages
2. Major Projects
3. Tools & Environment
4. OS Subsystems & Config
5. Education
6. Computer Science Education & Skills

**Mobile-specific rules:**
- Grid collapses to single flex column; column wrappers use `display: contents` so blocks reorder independently
- Operating Systems block: **hidden** (display: none)
- Language cards: smaller padding (8px/6px), name 12px, note 10px
- Education strip moves to just before CS Education & Skills
- DS grid collapses to single column
- Language grid: 3 columns
