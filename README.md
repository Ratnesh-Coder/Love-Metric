# 💗 Love Metric

### Browser-Based Chat Analysis and Communication Pattern Insights

**Love Metric** is a privacy-focused browser application that analyzes exported WhatsApp and Instagram conversations and turns raw chat data into measurable communication patterns.

Instead of relying only on subjective impressions, Love Metric examines observable signals such as **message balance, reply times, engagement, emotional warmth, conversation depth, emoji usage, word patterns, activity, and communication trends**.

The project is maintained as a versioned series, with each version representing an evolution of the analysis model and user experience.

---

## 🎯 Problem Statement

Let’s be honest — **we’ve all been there.** 😭

You’re chatting with someone and suddenly your brain becomes a full-time FBI analyst:

- “Do they actually like me?”
- “Why did they reply in 2 minutes yesterday but 2 hours today?”
- “Am I getting the same energy back, or am I carrying this conversation?”
- “Was that heart emoji meaningful or am I just delulu?” 💀
- “Are they interested… or are they just being nice?”

And then you start analyzing message timings, emojis, who started the conversation, who asked more questions, and basically everything except the actual conversation. 😭

The problem is simple:

> **When we chat with someone, we can observe how they communicate with us, but we cannot directly know whether they actually like us, are interested in us, or are simply being friendly.**

That’s where **Love Metric** comes in.

Instead of relying entirely on overthinking, Love Metric analyzes observable communication patterns in a chat and converts them into measurable insights — because apparently, when feelings get confusing, **we need data and charts.** 📊💀

The project looks at things such as:

- Who initiates conversations
- Who contributes more messages
- Reply speed and responsiveness
- Conversation depth
- Engagement and question frequency
- Emotional warmth
- Emoji and word patterns
- Consistency over time
- Changes in communication patterns

> ⚠️ **Important:** Love Metric does **not** read minds and cannot determine someone's actual feelings. It only analyzes patterns visible in the conversation.

---

## 💡 How It Works

Love Metric runs the analysis directly in the browser.

```text
        CHAT EXPORT
             │
             ▼
     ┌─────────────────┐
     │ File Detection  │
     └────────┬────────┘
              │
              ▼
     ┌─────────────────┐
     │ Message Parsing │
     └────────┬────────┘
              │
              ▼
     ┌─────────────────────────────┐
     │ Communication Analysis      │
     │                             │
     │ • Reciprocity               │
     │ • Responsiveness            │
     │ • Engagement                │
     │ • Warmth                    │
     │ • Emotional Support         │
     │ • Conversation Depth        │
     │ • Consistency               │
     │ • Temporal Trends           │
     └──────────────┬──────────────┘
                    │
                    ▼
          ┌──────────────────┐
          │ Visual Report    │
          ├──────────────────┤
          │ Overview         │
          │ Patterns         │
          │ Reply Times      │
          │ Emojis           │
          │ Words            │
          │ Activity         │
          └──────────────────┘
```

---

# 🧩 Project Versions

The repository contains three development versions.

```text
LoveMetric/
│
├── README.md
│
├── v1/
│   └── index.html
│
├── v2/
│   └── index.html
│
└── v3/
    └── index.html
```

---

## Version 1 — Initial Communication Analysis

`v1/index.html`

The first version establishes the core Love Metric analysis engine.

### Main capabilities

- WhatsApp chat export analysis
- Instagram chat export analysis
- Message parsing
- Sender identification
- Message-count analysis
- Reciprocity analysis
- Conversation initiation analysis
- Reply-time analysis
- Engagement measurement
- Emotional warmth measurement
- Emotional-support indicators
- Conversation-depth measurement
- Communication consistency
- Temporal communication trends
- Emoji analysis
- Word-frequency analysis
- Connection score
- Confidence level
- Communication-pattern detection
- Interactive charts

### Connection Score

Version 1 calculates a multidimensional connection score using weighted communication signals:

```text
Reciprocity        20%
Responsiveness     15%
Engagement         15%
Warmth             15%
Emotional Support  10%
Conversation Depth 15%
Consistency        10%
```

The score is intended as a **communication-pattern estimate**, not a measurement of someone's feelings.

---

# Version 2 — Improved Chat Analysis

`v2/index.html`

Version 2 expands the original analysis experience and improves the interface and report presentation.

### Added / refined capabilities

- Improved landing page
- WhatsApp `.txt` chat parsing
- Instagram `.json` parsing
- Instagram `.html` parsing
- Multiple chat-file support
- Drag-and-drop file upload
- Sample conversation mode
- Connection score presentation
- Confidence indicator
- Reply-time visualization
- Emoji analysis by participant
- Word-frequency visualization
- Language-category analysis
- Daily activity analysis
- Conversation span
- Active-day analysis
- Longest communication streak
- Most-active-day detection
- Privacy-focused browser execution

### Report Sections

```text
Overview
   │
   ├── Connection Score
   ├── Communication Metrics
   └── Breakdown

Reply Times
   │
   └── Response-time visualization

Emojis
   │
   └── Emoji usage by person

Words
   │
   ├── Word frequency
   └── Language categories

Activity
   │
   ├── Messages over time
   ├── Most active day
   ├── Longest streak
   └── Conversation span
```

---

# Version 3 — Evidence-Based Communication Analysis

`v3/index.html`

Version 3 expands the analysis model with a stronger focus on **observable dimensions, evidence, interpretation, and communication patterns**.

### Communication Dimensions

Seven observable dimensions are analyzed:

1. **Reciprocity**
2. **Responsiveness**
3. **Engagement**
4. **Warmth**
5. **Emotional Support**
6. **Conversation Depth**
7. **Consistency**

The application visualizes these dimensions and combines them into a connection score.

### Relationship Patterns

Version 3 can identify communication patterns such as:

- High warmth
- Deep conversation
- Emotional support
- Surface-level connection
- High chemistry with uncertain consistency
- Increasing closeness
- Declining engagement
- Stable connection
- Asymmetric participation

These labels describe **observable communication behavior**, not psychological facts.

### Evidence-Based Interpretation

The report can provide supporting evidence such as:

- Message contribution percentage
- Conversation initiation percentage
- Median reply time
- Reply-time asymmetry
- Question frequency
- Affectionate-language frequency
- Conversation trends
- Substantive-message ratio
- Average conversation-session length

The interpretation layer is explicitly limited to what can reasonably be inferred from the chat data.

---

# 📥 Supported Chat Exports

Love Metric supports the following formats:

| Source | Format | Support |
|---|---|---|
| WhatsApp | `.txt` | ✅ |
| Instagram | `.json` | ✅ |
| Instagram | `.html` | ✅ |
| Multiple files | Multiple supported files | ✅ |

Multiple Instagram message files can be processed together.

### WhatsApp

Export the conversation without media:

```text
WhatsApp
→ Chat menu
→ More
→ Export chat
→ Without media
```

### Instagram

Export your information through Meta's account information/export workflow.

For the supported Instagram formats, the application can process message JSON or HTML exports.

---

# 📊 Analysis Metrics

Love Metric calculates a range of communication metrics.

## Reciprocity

Measures how evenly communication is distributed between participants.

```text
Message contribution
Conversation initiation
Participation balance
```

---

## Responsiveness

Examines reply timing.

```text
Median reply time
Reply-time distribution
Per-person response behavior
Response asymmetry
```

Fast replies indicate responsiveness, **not necessarily romantic interest**.

---

## Engagement

Looks at signals such as:

```text
Questions
Follow-up behavior
Message activity
Substantive responses
```

---

## Warmth

Examines affectionate and supportive language relative to the communication patterns observed in the conversation.

---

## Emotional Support

Looks for apparent supportive responses following messages that contain signals of difficulty or emotional disclosure.

The result is presented as an observable communication pattern rather than a psychological conclusion.

---

## Conversation Depth

Examines:

```text
Message length
Substantive messages
Questions
Follow-up exchanges
Conversation-session length
```

---

## Consistency

Measures how consistently communication occurs across the analyzed time period.

---

## Temporal Trends

The application can compare communication behavior across time and identify trends such as:

```text
Increasing
Declining
Stable
Inconsistent
```

---

# 📈 Visualizations

Love Metric uses interactive charts to visualize:

- Connection dimensions
- Reply times
- Emoji usage
- Word frequency
- Daily activity
- Communication trends

The visual report makes large chat exports easier to understand without manually reading the entire conversation.

---

# 🔐 Privacy

Privacy is a core design principle of Love Metric.

The application is designed to process uploaded chat files **locally inside the browser**.

```text
Your Chat
    │
    ▼
Your Browser
    │
    ▼
Local Parsing
    │
    ▼
Local Analysis
    │
    ▼
Local Report
```

The application does not require a backend server for the chat-analysis process.

The interface states:

> Runs entirely in your browser — nothing is uploaded.

### Important Privacy Note

This repository includes external frontend resources such as Google Fonts and Chart.js. The chat-analysis data itself is processed in the browser, but users should still consider their browser/network environment and any externally loaded resources when evaluating privacy requirements.

---

# 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Application structure |
| **CSS3** | Responsive interface and styling |
| **JavaScript** | Chat parsing and analysis engine |
| **Chart.js** | Interactive data visualization |
| **Google Fonts** | Typography |
| **FileReader API** | Reading local chat exports |
| **Browser APIs** | Local file processing |

The project currently uses a lightweight, client-side architecture without a dedicated application backend.

---

# 🚀 Getting Started

## Prerequisites

No Node.js, Python, database, or backend server is required for the current versions.

You only need:

- A modern web browser
- A supported WhatsApp or Instagram chat export
- Git (only if cloning the repository)

---

## Run Locally

Clone the repository:

```bash
git clone https://github.com/Ratnesh-Coder/LoveMetric.git
```

Navigate into the project:

```bash
cd LoveMetric
```

Open any version:

```text
v1/index.html
v2/index.html
v3/index.html
```

You can open `index.html` directly in a modern browser.

For development, you can also serve the repository using a local static server.

---

# 🧪 Example Workflow

```text
1. Open Love Metric
        ↓
2. Select a chat export
        ↓
3. Drop the file into the application
        ↓
4. Start analysis
        ↓
5. Parse messages
        ↓
6. Calculate communication metrics
        ↓
7. Generate visualizations
        ↓
8. Explore the analysis report
```

A built-in sample conversation is also available for testing the interface without using a personal chat export.

---

# ⚠️ Limitations

Love Metric is a communication-analysis and visualization project.

It should **not** be treated as a mind-reading system or a definitive relationship detector.

Chat data alone cannot reliably determine:

- Whether someone is secretly in love
- Whether someone is faithful or cheating
- Whether someone is attracted to another person
- Someone's private feelings outside the conversation
- Someone's psychological diagnosis
- Whether a relationship will last

Communication style varies significantly between people, so numerical scores and detected patterns should be interpreted as **descriptive indicators of the analyzed conversation**, not objective facts about the people involved.

---

# 🎯 Project Objectives

Take the chat, crunch the data, and see whether the conversation shows signs that the other person **might be interested** — because apparently asking them directly is harder than building an entire analytics dashboard. 💀📊

The main objectives of Love Metric are to:

- Analyze real-world chat exports from supported platforms.
- Measure who initiates conversations and who contributes more.
- Analyze reply times and overall responsiveness.
- Examine engagement, warmth, questions, and conversation depth.
- Study emoji usage and word patterns.
- Identify observable communication patterns and behavioral trends.
- Detect changes in communication over time.
- Generate a **Connection Score** based on measurable communication dimensions.
- Present the results through an easy-to-understand visual report.
- Keep chat analysis primarily client-side to support user privacy.
- Turn the classic **“Do they like me or am I just delulu?”** question into a fun data-analysis experiment. 😭📊

## 🧠 The Big Disclaimer

The result **does NOT guarantee** that someone likes you, dislikes you, is romantically interested in you, or will become interested in you.

**Love Metric is just a fun project that analyzes communication patterns.**

A high score does **not** mean:

> 💍 “Congratulations, you’re getting married.”

And a low score does **not** mean:

> 😭 “It’s over. Delete the chat.”

The results should be treated as **interesting observations, not proof of someone's feelings**.

At the end of the day, the only truly reliable way to know how someone feels is still **actual human communication.** ❤️

---

# 📌 Project Status

**Active Student / Personal Research Project**

The repository currently contains three progressively developed versions:

```text
v1 → Initial communication analysis
v2 → Expanded analysis and improved reporting
v3 → Evidence-based communication patterns and interpretation
```

The versions are preserved separately so the development progression can be studied and compared.

---

# 👨‍💻 Author

**Ratnesh**

Engineering Student

GitHub:  
https://github.com/Ratnesh-Coder

---

# 📄 License

This project is maintained as a personal/student project.
