# 💗 Love Metric

### Because "who texts first?" apparently needed a dashboard.

Love Metric is a browser-based chat analysis project that takes exported WhatsApp and Instagram conversations and turns them into measurable communication patterns.

Ever wondered who sends more messages, who usually starts the conversation, how long replies take, or whether the chat has slowly turned into a one-person podcast? Love Metric explores questions like these using observable signals from chat data.

It looks at things like **message balance, reply times, engagement, warmth, emotional support, conversation depth, emoji usage, word patterns, activity, and communication trends**.

This started as a fun project and a curiosity-driven experiment. It is not a relationship oracle. It will not tell you whether someone is "the one", decode a "hmm", or explain why they replied with just "okay".

> [!IMPORTANT]
> Chat data can show communication patterns. It cannot reveal someone's private feelings, romantic intentions, psychological state, faithfulness, or whether a relationship will last. Please don't make life decisions based on a chart. Talk to the person. Revolutionary, we know.

---

## 🎯 What does it actually do?

Love Metric helps explore questions such as:

- Who contributes more to the conversation?
- Who usually starts the conversation?
- How quickly does each person respond?
- Is communication reasonably balanced?
- How often do people ask questions or send substantive replies?
- Which emojis and words appear most often?
- How does communication change over time?
- Are there noticeable patterns in warmth, support, engagement, or consistency?

In short: it turns a chat export into a collection of statistics and visualizations. Whether those statistics explain the entire relationship is a different question — and very much outside this app's job description.

## 💡 How it works

The analysis runs directly in your browser. The basic flow looks like this:

```text
        CHAT EXPORT
             │
             ▼
      ┌─────────────────┐
      │  File Detection │
      └────────┬────────┘
               │
               ▼
      ┌─────────────────┐
      │ Message Parsing │
      └────────┬────────┘
               │
               ▼
      ┌─────────────────────────────┐
      │    Communication Analysis  │
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
           │   Visual Report  │
           ├──────────────────┤
           │ Overview         │
           │ Patterns         │
           │ Reply Times      │
           │ Emojis           │
           │ Words            │
           │ Activity         │
           └──────────────────┘
```

No server-side relationship counselling is involved.

---

## 🧩 Project versions

The repository contains three versions. Each one builds on the previous version, because apparently one attempt at measuring conversations wasn't enough.

```text
LoveMetric/
│
├── README.md
├── LICENSE
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

### Version 1 — The beginning

`v1/index.html`

The first version establishes the core analysis engine.

**Main capabilities**

- WhatsApp and Instagram chat analysis
- Message parsing and sender identification
- Message-count analysis
- Reciprocity and conversation-initiation analysis
- Reply-time analysis
- Engagement measurement
- Emotional-warmth and emotional-support indicators
- Conversation-depth measurement
- Communication consistency and temporal trends
- Emoji and word-frequency analysis
- Connection score and confidence level
- Interactive charts

**Connection score**

Version 1 calculates a weighted score from seven communication signals:

| Dimension | Weight |
|---|---:|
| Reciprocity | 20% |
| Responsiveness | 15% |
| Engagement | 15% |
| Warmth | 15% |
| Emotional Support | 10% |
| Conversation Depth | 15% |
| Consistency | 10% |

The score is a **communication-pattern estimate**, not a scientifically validated measurement of affection or compatibility. A percentage is not a personality test. Sorry.

### Version 2 — More data, fewer guesses

`v2/index.html`

Version 2 expands the analysis experience and improves the interface and report presentation.

**Added and refined capabilities**

- Improved landing page
- WhatsApp `.txt` parsing
- Instagram `.json` and `.html` parsing
- Multiple chat-file support
- Drag-and-drop file upload
- Sample conversation mode
- Connection-score presentation and confidence indicator
- Reply-time visualization
- Emoji analysis by participant
- Word-frequency and language-category visualization
- Daily activity analysis
- Conversation span and active-day analysis
- Longest communication streak
- Most-active-day detection
- Browser-based processing

**Report sections**

- **Overview:** connection score, communication metrics, and breakdown
- **Reply Times:** response-time visualization
- **Emojis:** emoji usage by person
- **Words:** word frequency and language categories
- **Activity:** messages over time, most active day, longest streak, and conversation span

### Version 3 — Receipts, not just vibes

`v3/index.html`

Version 3 puts more emphasis on observable dimensions, supporting evidence, and cautious interpretation.

**Seven communication dimensions**

1. **Reciprocity** — how communication is distributed
2. **Responsiveness** — reply timing and response patterns
3. **Engagement** — questions, follow-ups, and substantive responses
4. **Warmth** — affectionate and supportive language signals
5. **Emotional Support** — apparent supportive responses to difficult or emotionally revealing messages
6. **Conversation Depth** — message substance and depth of exchanges
7. **Consistency** — how regularly communication occurs

The application combines these dimensions into a connection score and can identify patterns such as:

- High warmth
- Deep conversation
- Emotional support
- Surface-level connection
- High chemistry with uncertain consistency
- Increasing closeness
- Declining engagement
- Stable connection
- Asymmetric participation

These labels describe **patterns in the messages**, not facts about what someone is thinking.

**Evidence behind the interpretation**

Depending on the report, supporting signals can include:

- Message contribution percentage
- Conversation initiation percentage
- Median reply time
- Reply-time asymmetry
- Question frequency
- Affectionate-language frequency
- Conversation trends
- Substantive-message ratio
- Average conversation-session length

The idea is simple: show the signals behind an interpretation instead of presenting a dramatic label with absolutely no receipts.

---

## 📥 Supported chat exports

| Platform | Format | Support |
|---|---|---|
| WhatsApp | `.txt` | ✅ |
| Instagram | `.json` | ✅ |
| Instagram | `.html` | ✅ |
| Multiple files | Supported formats | ✅ |

Multiple Instagram message files can be processed together.

### WhatsApp

Export a conversation without media:

```text
WhatsApp
  → Chat menu
  → More
  → Export chat
  → Without media
```

### Instagram

Request an information export through Meta's account information/export workflow. Love Metric can process supported message exports in JSON or HTML format.

---

## 📊 What gets measured?

Here's the less-romantic, more-technical explanation.

| Metric | What it examines |
|---|---|
| **Reciprocity** | Message contribution, conversation initiation, and participation balance |
| **Responsiveness** | Median reply time, reply-time distribution, per-person response behavior, and response asymmetry |
| **Engagement** | Questions, follow-up behavior, message activity, and substantive responses |
| **Warmth** | Affectionate and supportive language patterns |
| **Emotional Support** | Apparent supportive responses after messages containing signals of difficulty or emotional disclosure |
| **Conversation Depth** | Message length, substantive messages, questions, follow-up exchanges, and session length |
| **Consistency** | How regularly communication occurs during the analyzed period |
| **Temporal Trends** | Whether measured communication patterns appear to be increasing, declining, stable, or inconsistent |

A fast reply can indicate responsiveness. It does **not** automatically indicate romantic interest. Sometimes people are just on their phones. Shocking, I know.

## 📈 Visualizations

Love Metric uses interactive charts to make large chat exports easier to explore.

Visualizations cover:

- Connection dimensions
- Reply times
- Emoji usage
- Word frequency
- Daily activity
- Communication trends

Less scrolling through thousands of messages; more exploring the patterns. Your thumbs may rest.

---

## 🔐 Privacy

Privacy matters here, especially because chat exports can contain very personal conversations.

Love Metric is designed to process uploaded chat files **locally inside the browser**:

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

The chat-analysis process does not require a dedicated application backend.

> Runs entirely in your browser — nothing is uploaded.

**A small but important privacy note:** The repository uses external frontend resources such as Google Fonts and Chart.js. Chat-analysis data is processed in the browser, but external resources may still involve network requests. Consider your browser and network environment when evaluating privacy requirements.

Also, only analyze conversations you have the right to access and use. Other people's messages are still their personal data, even if you have an export file.

---

## 🛠️ Technology stack

| Technology | Purpose |
|---|---|
| **HTML5** | Application structure |
| **CSS3** | Responsive interface and styling |
| **JavaScript** | Chat parsing and analysis engine |
| **Chart.js** | Interactive data visualization |
| **Google Fonts** | Typography |
| **FileReader API** | Reading local chat exports |
| **Browser APIs** | Client-side file processing |

The project uses a lightweight, client-side architecture without a dedicated application backend.

---

## 🚀 Getting started

Good news: no elaborate setup ritual is required.

### Prerequisites

You need:

- A modern web browser
- A supported WhatsApp or Instagram chat export
- Git, if you want to clone the repository

No Node.js, Python, database, or backend server is required for the current versions.

### Run locally

Clone the repository:

```bash
git clone https://github.com/Ratnesh-Coder/LoveMetric.git
```

Navigate into the project:

```bash
cd LoveMetric
```

Open the version you want to try:

```text
v1/index.html
v2/index.html
v3/index.html
```

You can open an `index.html` file directly in a modern browser. You can also use a local static server during development.

### Example workflow

1. Open Love Metric.
2. Choose a supported chat export.
3. Drop the file into the application.
4. Start the analysis.
5. Let the parser do its thing.
6. Explore the calculated metrics.
7. Check out the visualizations.
8. Interpret the results like a reasonable human being.

A built-in sample conversation is also available to test the interface without using a personal chat export.

---

## ⚠️ A reality check: limitations

Love Metric is a communication-analysis and visualization project. It is **not** a mind-reading system, relationship detector, therapist, or replacement for an honest conversation.

Chat data alone cannot reliably determine:

- Whether someone is secretly in love
- Whether someone is faithful or cheating
- Whether someone is attracted to another person
- Someone's private feelings outside the conversation
- Someone's psychological diagnosis
- Whether a relationship will last

Communication styles vary between people. Context, personality, culture, schedules, and circumstances all matter. Numerical scores and detected patterns should therefore be treated as **descriptive indicators of the analyzed conversation**, not objective facts about the people involved.

Please do not confront someone because a chart said their reply time increased by 17%. That's between you, them, and perhaps a very normal conversation.

---

## 📌 Project status

**Active personal / student project**

The repository currently contains three progressively developed versions:

```text
v1 → Initial communication analysis
v2 → Expanded analysis and improved reporting
v3 → Evidence-based communication patterns and interpretation
```

The versions are preserved separately so their development and differences can be explored.

## 🤖 AI assistance & acknowledgements

This project was developed with AI assistance using **Anthropic Claude**.

Claude assisted with code generation, feature implementation, debugging, UI/UX improvements, analytical logic, and documentation.

The project concept, objectives, feature requirements, and overall development direction were defined by me. I reviewed the generated implementation and worked through the development process to understand the concepts behind chat parsing, communication metrics, behavioral analysis, statistical interpretation, and data visualization.

**Note:** AI-generated code and suggestions are subject to ongoing review, testing, understanding, and improvement.

---

## 👨‍💻 Author

**Ratnesh**  
Engineering Student

GitHub: [Ratnesh-Coder](https://github.com/Ratnesh-Coder)

---

## 📄 License

This project is maintained as a personal/student project.
