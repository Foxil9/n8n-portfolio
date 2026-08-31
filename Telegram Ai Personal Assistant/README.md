# Project Summary — Telegram Chat Bot

!Telegram Personal Assistant-modified.png

**The problem:** This solves a convenience problem more than a business one, so you can focus more on running the business and less on daily admin. Sometimes you don't want to open a website and update information, especially when there's a lot of it. Or you don't want to switch between three different apps just to get one thing done. Having someone handle that for you quickly, and understanding you by voice, saves a lot of time!

**The solution I provide:** This workflow allows a personal assistant “Jackie” to manage everything you find boring, summarize emails, manage the calendar and even make new tasks for you. Jackie understands both voice and text. You know the best part? This can be expanded even if you don’t understand n8n. Just go the tools section in the AI Agent node and add a new tool, fill in the required fields and you are done.

**The Logic Behind:** I use a Telegram node to check for a new message, and then check whether the message is text or voice. If text, it will be handed immediately to the AI agent. If the message is a voice message, it will be handed to an AI Transcription Tool using an HTTP Request, and then handed to the AI agent. From there, the AI agent will fulfill your request based on that message.

**What I learned from this project:** I learned how to manage binary data and transform it, I learned how to use AI Agents and link tools to them (Even external ones!), I learned how to properly use HTTP Requests to integrate what isn’t available in n8n out of the box

Try it Yourself! All workflows can be accessed in my github page.

You'll need to set up any missing credentials for this to work. If self-hosting, the instance needs a public IP/URL. n8n Cloud works out of the box with no hosting required.”
