# The Friendly Neighbourhood Bot

The bustling online community of Midtown Tech (your Discord server) is a vibrant hub for brilliant young minds, much like the students of Peter Parker's own high school. Here, aspiring heroes of code share their discoveries, collaborate on groundbreaking projects, and even unwind with friendly banter. However, even in a neighborhood as friendly as Midtown, chaos can creep in. Misplaced messages, forgotten announcements, and the occasional "Goblin" (read: troll) attempting to disrupt the peace threaten the very order of this digital city.

Just as Spider-Man swings through the streets of New York, protecting its citizens, Midtown Tech needs its own friendly neighborhood guardian. The faculty, overwhelmed by the sheer volume of activity, has put out a call for innovative solutions. Your mission, young developer, is to construct the core intelligence of a new kind of "Friendly Neighborhood Bot". This bot will not only help maintain order and keep the digital streets clean but also empower the community to better organize their knowledge and interactions, ensuring Midtown Tech remains a safe and inspiring place for all.

Your Mission: Build the Friendly Neighborhood Bot

Your task is to develop a Discord bot named "Friendly Neighborhood Bot" with the following core functionalities. Remember, this bot should operate entirely within the Discord environment, using only the Discord API and your bot's internal logic – no external APIs, databases, or web interfaces are allowed.

Core Functionalities:

Welcome to the Neighborhood & Initial Orientation:

When a new student (member) joins Midtown Tech, your Friendly Neighborhood Bot must immediately send a warm, personalized welcome message in a designated #orientation channel.

Simultaneously, the bot should automatically assign a default role (e.g., "New Student" or "Aspiring Hero") to the newly joined member. This helps new members immediately feel part of the community, just like joining a new class.

Spider-Sense: Basic Content Moderation:

The Friendly Neighborhood Bot must actively monitor all messages across the server for "chaos-inducing" elements – much like Spider-Man's spider-sense tingling for danger. This includes a predefined list of keywords (e.g., "villainous spam", "unauthorized link", "off-topic disruption", "menacing threats").

If a message contains any of these forbidden keywords, the bot must:

Immediately delete the offending message, swinging in to remove the threat.

Send a polite, private warning message to the user who sent it, reminding them of Midtown Tech's code of conduct and encouraging constructive communication.

(Hint: Ensure your bot has the necessary permissions to manage messages and send DMs.)

Daily Bugle Briefings: Self-Cleaning Announcements:

Midtown Tech needs a way to broadcast important announcements (like daily headlines from the Daily Bugle) without cluttering the #announcements channel indefinitely.

Implement a command (e.g., !bugle <your message here>) that allows authorized users (e.g., those with "Faculty" or "Administrator" roles) to post official announcements.

These announcements should be posted in a designated #announcements channel.

Crucially, after a configurable duration (e.g., 24 hours), the Friendly Neighborhood Bot should automatically "shred" these old briefings to keep the channel tidy, unless they have been manually "pinned" by a human moderator (like a permanent headline).

(Hint: You'll need to manage a simple in-memory timer for this. Persistence across bot restarts is not required for this task.)

Aunt May's Wisdom: Quick Info Retrieval:

To help students quickly find essential information, the Friendly Neighborhood Bot should act as a basic knowledge base, sharing wisdom much like Aunt May.

Implement a command (e.g., !wisdom <topic>) where <topic> can be one of several predefined keywords (e.g., "rules", "resources", "contact").

Based on the <topic> provided, the bot should respond with a predefined block of text relevant to that topic.

!wisdom rules: Displays Midtown Tech's core rules.

!wisdom resources: Provides a list of essential learning resources or helpful links (predefined in your bot's code).

!wisdom contact: Gives information on how to contact faculty or administrators.

Why This Task is Important and Relevant:

Real-World Application: Moderation, onboarding, and information management are critical for any successful online community, especially large Discord servers.

Core Bot Concepts: This task forces you to understand fundamental Discord bot programming concepts: event handling (member joins, messages sent), command parsing, role management, permissions, and message manipulation.

Problem-Solving: You'll need to think about how to manage state (e.g., for timed deletions) and implement robust logic within the constraints of a self-contained application.

Foundation for Future Projects: Mastering these basics will provide a strong foundation for building more complex, feature-rich bots in the future.

Go get 'em, tiger! Midtown Tech needs its Friendly Neighborhood Bot.
