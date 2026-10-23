# Almond — Character Room

A lightweight, local-first character chat app published as a subfolder of the owner's GitHub Pages site.

## Open the app

https://anubhutigoswami125.github.io/almond/

## First-time setup

1. Open https://console.groq.com/keys and create a Groq API key.
2. Open Almond and choose **Settings**.
3. Paste your key. The default endpoint is `https://api.groq.com/openai/v1/chat/completions`.
4. The default model is `openai/gpt-oss-20b`. If Groq changes model availability, use a currently available model ID from https://console.groq.com/docs/models.
5. Save settings and test the connection, then start chatting.

## Features

- Jimin fictional test character (fan-made roleplay character, not the real person)
- Character creation, editing, deletion, avatar image URL
- Streaming replies through Groq's OpenAI-compatible Chat Completions API
- Character memory editable by the user, plus optional AI memory summarization
- Local browser storage for characters, chats, settings, and memories
- Character JSON import/export and full-library backup export/import
- Three themes: rich maroon/pink, dark brown/beige, and black/grey
- No Hatchable dependency, no Google sign-in, no app account

## Privacy and limitations

- The API key is stored in this browser's local storage and sent directly to Groq. It is not embedded in this repository. Anyone with access to this browser profile may be able to use the key.
- Chat history and memories are stored in this browser only. They do not sync across devices or browsers. Export backups regularly.
- Groq's free-tier model availability and rate limits can change.
- This static version has no backend. If the browser reports a CORS/network error, the API provider may be blocking direct browser requests; a small backend proxy would then be required.
