# Velox
Velox - A real-time, voice-powered AI personal assistant infused with sarcasm, class, and real utility. This assistant can speak, understand your voice, read back generated content, search the web, send emails, check the weather, and even save your notes, all with a touch of wit.

### Key Features:
- Real-time voice interaction with Google Gemini via LiveKit Agents
- Responds like a classy, sarcastic butler ("Friday" style)
- Gets current weather updates for any city
- Performs live web search via DuckDuckGo
- Sends emails using Gmail SMTP
- Saves AI-generated or user-input text to local files
- Maintains personality and context during sessions
- Designed with extensibility for custom tools

### Tech Stack:
| Tech / Library               | Purpose                                    |
| ---------------------------- | ------------------------------------------ |
| **LiveKit Agents**           | Real-time audio, session orchestration     |
| **Google Gemini (Realtime)** | Voice AI via Generative AI                 |
| **LangChain Tools**          | Web search integration via DuckDuckGo      |
| **Python + asyncio**         | Asynchronous agent logic and tool handling |
| **SMTP / smtplib**           | Secure email sending                       |
| **dotenv**                   | Secure environment configuration           |
| **Pydantic / Typing**        | Structured arguments for tools             |

### How It Works?
User: "Can you search weather of Karachi?"
Waniya: "Of course sir, I will now be looking up Karachi's weather - I do hope your brilliance was properly conveyed."

### Folder Structure:
project-waniya/ <br>
├── main.py         
├── prompts.py <br>
├── tools.py  <br>
├── .env     <br>
├── requirements.txt  <br>
└── README.md         <br>

### Run the Assistant:
python main.py

#### The assistant greets you with:
"Hi, my name is Waniya, your personal assistant. How may I help you?"

### Available Tools:
| Tool                | Description                                                   |
| ------------------- | ------------------------------------------------------------- |
| `get_weather`       | Retrieves live weather information via `wttr.in`              |
| `search_web`        | Uses DuckDuckGo for a quick and private web search            |
| `send_email`        | Sends structured email via Gmail SMTP                         |
| `save_text_to_file` | Saves generated or spoken content to a timestamped local file |
