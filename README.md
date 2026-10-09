# /call-me power for Kiro

<img src="assets/logo.png" alt="/call-me" width="96">

Let Kiro ring your iPhone, read you a question or a status update, and get your
spoken answer back as text. It can also text you and wait for your reply. Use it
to keep a long spec or agent task moving while you are driving, at the gym or
away from the desk.

/call-me is a voice relay, not a voice assistant. Kiro does the thinking; /call-me
carries the question to your phone and your answer back.

## What is inside

| File | For |
|---|---|
| `plugin.json` | Power manifest |
| `mcp.json` | The hosted MCP server, `https://callmemcp.com/mcp` (Streamable HTTP, no API key) |
| `skills/call-me/SKILL.md` | When and how Kiro should call or text you |

Nothing runs on your machine. The power points Kiro at the hosted server and
teaches the agent when to use it.

## Setup

1. Install [/call-me](https://callmemcp.com/go/kiro) on your iPhone and open
   **My Number**. Those 10 digits are all Kiro needs.
2. In Kiro, open **Powers**, choose **Add Custom Power**, then **Import power
   from GitHub**, and paste `https://github.com/radres/kiro-power-call-me`.
3. Try it without ringing anyone: *"text the /call-me demo line 5550001234 to
   check it works"*. The demo line answers by itself.
4. Then give Kiro your number: *"my /call-me number is …, call me when the tests
   pass"*.

Connecting costs nothing. Reaching a real phone needs an active subscription in
the iPhone app, with a free trial for eligible accounts.

## Tools

| Tool | What it does |
|---|---|
| `call` | Rings your iPhone, reads the text aloud, returns your spoken reply as text |
| `poll_result` | Finishes a call that was still ringing |
| `text` | Push-notification message, no ring |
| `wait_for_reply` | Delivers your texts and voicemails back to Kiro |
| `set_thread_title` | Names the conversation thread on your phone |
| `setup` | First-setup instructions and the App Store link |

Your number is the only credential: whoever has it can reach your phone, nobody
else can. Calls and texts are rate limited, and blocking a thread in the app
silences that sender for good.

## Privacy policy

https://callmemcp.com/privacy

## Support

Email serdar.oztetik@gmail.com, or open an issue at
https://github.com/radres/kiro-power-call-me/issues. Terms:
https://callmemcp.com/terms

## License

MIT
