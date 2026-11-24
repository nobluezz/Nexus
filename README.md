# Nexus

Welcome. Nexus is a free app for Mac and Windows that gives you a team of AI agents, arranged as a tree of skills.

- A **company tree** is for work. It has departments such as Sales, Marketing, Operations and Finance. Each department has its own agent and a set of jobs it can run.
- A **personal tree** is for the rest of life: Life Admin, Money, Health & Habits, Career, Learning, Travel & Events, Writing & People. It is private to you, and nobody can be invited to it.

You can have either tree or both. Agents can chat, run skills, make real files (PDF, Word, Excel), remember what you teach them and run on a schedule. If you connect a Google or Microsoft 365 account, they can also read your mail, calendar and files. They never send an email or invite anyone until you approve it.

Nexus is free. There are no plans, seats or trials.

If you use Claude Code, Nexus also shows a live map of your Claude sessions on your own computer (**This Mac**, or **This PC** on Windows), and a **Centers** page for running your own security center or GitHub center skills on a project.

## Download

Version 0.1.11

| Your computer | Download |
|---|---|
| Mac with Apple silicon (M1 or newer) | [Nexus-0.1.11-mac-arm64.dmg](https://github.com/nobluezz/Nexus/releases/download/v0.1.11/Nexus-0.1.11-mac-arm64.dmg) |
| Mac with an Intel processor | [Nexus-0.1.11-mac-x64.dmg](https://github.com/nobluezz/Nexus/releases/download/v0.1.11/Nexus-0.1.11-mac-x64.dmg) |
| Windows 10 or 11 (64-bit) | [Nexus-Setup-0.1.11-x64.exe](https://github.com/nobluezz/Nexus/releases/download/v0.1.11/Nexus-Setup-0.1.11-x64.exe) |

Not sure which Mac you have? Choose Apple menu → About This Mac. "Chip: Apple M…" means Apple silicon. "Processor: Intel" means Intel. Nexus needs macOS 13 or newer.

Newer versions appear on the [releases page](https://github.com/nobluezz/Nexus/releases). Nexus doesn't update itself, so check back here now and then.

## Opening it the first time

The installers are not signed with a paid Apple or Microsoft developer certificate, so each system asks you to confirm once.

**Mac**

1. Open the disk image and drag Nexus into Applications.
2. Open Nexus. macOS says it can't verify the app. Choose **Done**.
3. Open **System Settings → Privacy & Security**, scroll down and choose **Open Anyway**.
4. macOS may ask for your login password so that Nexus can keep its key in your keychain. Choose **Always Allow**.

**Windows**

1. Run the installer. It installs for you only and needs no administrator.
2. SmartScreen says "Windows protected your PC". Choose **More info → Run anyway**.

## What you need

**Your own Claude access.** Nexus doesn't come with AI credits, and nobody else pays for your use. Choose one in **Settings → AI**:

- **An API key** from [console.anthropic.com](https://console.anthropic.com). Anthropic bills you for what your agents use, so set a spending limit there. Nexus also shows your spending and keeps a monthly limit of its own.
- **Your Claude plan.** Choose **Add Nexus to Claude** and chat with your tree inside the Claude app. Schedules and other background runs still need an API key.

Until you choose, Nexus runs in demo mode so you can look around.

## Your data

Everything stays on your computer: your trees, chats, files and saved keys. Nothing is sent to the people who make Nexus. Your messages go to Anthropic when an agent answers, and to Google or Microsoft only if you connect those accounts.

- Mac: `~/Library/Application Support/Nexus`
- Windows: `%APPDATA%\Nexus`

Saved keys are encrypted with a key held by the macOS Keychain or Windows data protection, so they only open for you on your computer.

## Connecting Google or Microsoft 365

Open **Integrations** in Nexus and choose Connect. Sign-in happens in your own browser, and you choose what to allow (mail, calendar, files).

- **Google:** sign-in is still in Google's testing stage, so for now it works only for people on a short list. If Google says access is blocked, that is the reason.
- **Microsoft:** the permission screen says the app is unverified. A work or school account may need its administrator's approval first.

## Known limits

- **This PC** (the map of Claude sessions on Windows) is new in 0.1.11. It is checked on a Windows machine at GitHub with made-up sessions. If yours don't show up, please open an issue.
- On Windows a few of the map's panels aren't there yet: running dev servers, scheduled jobs, the calendar, and file thumbnails. Sessions run inside WSL aren't shown.
- The Intel Mac version has not yet been tried on an Intel Mac.
- To share a company tree with teammates, someone has to run a Nexus company server. The app explains this when you invite someone.

## Updating and removing

- **Update:** download the newer version and install it over the old one. Your data stays. On a Mac, the keychain question comes back once: choose Always Allow.
- **Remove on a Mac:** drag Nexus from Applications to the Trash. To remove your data too, delete `~/Library/Application Support/Nexus`.
- **Remove on Windows:** Settings → Apps → Nexus → Uninstall. To remove your data too, delete `%APPDATA%\Nexus`.

## Problems or questions

Open an [issue](https://github.com/nobluezz/Nexus/issues) on this page. Please don't paste API keys or anything private into an issue.

---

Nexus is free to use. This page holds the downloads only. The app's source code is not published here.
