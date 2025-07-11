# 🕸️ The Friendly Neighbourhood Bot

The bustling online community of Midtown Tech (your Discord server) is a vibrant hub for brilliant young minds, much like the students of Peter Parker's own high school. Here, aspiring heroes of code share their discoveries, collaborate on groundbreaking projects, and even unwind with friendly banter.  

However, even in a neighborhood as friendly as Midtown, chaos can creep in. Misplaced messages, forgotten announcements, and the occasional "Goblin" (read: troll) attempting to disrupt the peace threaten the very order of this digital city.

Just as Spider-Man swings through the streets of New York, protecting its citizens, Midtown Tech needs its own friendly neighborhood guardian. The faculty, overwhelmed by the sheer volume of activity, has put out a call for innovative solutions.

---

## 🛠️ Your Mission: Build the Friendly Neighborhood Bot

Your task is to develop a Discord bot named **"Friendly Neighborhood Bot"** with the following core functionalities.  
> **Note:** The bot should operate entirely within the Discord environment, using only the **Discord API** and your bot's internal logic – **no external APIs, databases, or web interfaces are allowed**.

---

## 🔑 Core Functionalities

### 1. Welcome to the Neighborhood & Initial Orientation

- When a new student (member) joins **Midtown Tech**, your Friendly Neighborhood Bot must:
  - Send a warm, personalized welcome message in a designated `#orientation` channel.
  - Automatically assign a default role (e.g., `"New Student"` or `"Aspiring Hero"`) to the newly joined member.

This helps new members immediately feel part of the community, just like joining a new class.

---

### 2. Spider-Sense: Basic Content Moderation

- The bot must actively monitor all messages across the server for “chaos-inducing” elements – much like Spider-Man’s spider-sense tingling for danger.

#### Forbidden Keywords Include:
- `"villainous spam"`
- `"unauthorized link"`
- `"off-topic disruption"`
- `"menacing threats"`

#### On detecting these:
- The bot should **immediately delete** the offending message.
- Then, **send a polite, private warning message** to the user, reminding them of Midtown Tech's code of conduct and encouraging constructive communication.

> 💡 *Hint:* Ensure your bot has the necessary permissions to manage messages and send DMs.

---

### 3. Daily Bugle Briefings: Self-Cleaning Announcements

- Implement a command (e.g., `!bugle <your message here>`) that allows **authorized users** (e.g., with `"Faculty"` or `"Administrator"` roles) to post official announcements.

#### Requirements:
- Post the message in a designated `#announcements` channel.
- After a configurable duration (e.g., **24 hours**), the bot should **automatically delete** (shred) these messages to keep the channel tidy.
- If the message is **pinned by a human moderator**, it should be retained.

> 💡 *Hint:* Use an in-memory timer. Persistence across bot restarts is not required.

---

### 4. Aunt May's Wisdom: Quick Info Retrieval

- Implement a command (e.g., `!wisdom <topic>`) where `<topic>` is one of the predefined keywords:
  - `rules`
  - `resources`
  - `contact`

#### Bot should respond with predefined messages:

- `!wisdom rules`: Displays Midtown Tech's core rules.
- `!wisdom resources`: Provides a list of essential learning resources or helpful links.
- `!wisdom contact`: Gives information on how to contact faculty or administrators.

---

## 🎯 Why This Task is Important and Relevant

- **Real-World Application:** Moderation, onboarding, and information management are critical for any successful online community.
- **Core Bot Concepts:** Understand event handling (e.g., member joins, messages sent), command parsing, role management, permissions, and message manipulation.
- **Problem-Solving:** Learn to manage state (e.g., timed deletions) and implement robust logic within constraints.
- **Foundation for Future Projects:** This lays the groundwork for building more complex and feature-rich bots.

---

Midtown Tech needs its **Friendly Neighborhood Bot**.
