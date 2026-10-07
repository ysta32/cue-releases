# Cue — privacy notice

Effective October 7, 2026.

Here's what we collect, why, and where it goes.

## What we collect

- **Captures**: whatever you type or say into the capture bar (for example, "read chapter 3
  before Friday"), and your **/ask conversation replies** (Cue's chat-style follow-ups).
  Speech-to-text uses Apple's on-device speech recognition when your Mac supports it; when it
  doesn't, Apple's speech servers are used instead, so audio may leave your device in that case.
  Either way, only the resulting text reaches Cue. With **Better voice accuracy** on (Settings →
  General, on by default on Apple silicon Macs), Cue also listens to the same recording again
  with a speech model that runs entirely on your Mac (OpenAI's Whisper, downloaded once from
  Hugging Face). That second listen never sends your audio anywhere.
- **Tasks and events** created from your captures, and the outcome of each capture (what Cue
  understood it as).
- **Imported details**: Canvas assignment details and Google Calendar event details, if you
  connect those, plus the **Canvas feed URL** and **Google Calendar tokens** themselves. If you
  allow it when connecting Google Calendar, Cue can also add, change and delete events on your
  own Google Calendar, only when you confirm a change in the app.
- **Apple Calendar events**, if you connect Apple Calendar: the Mac app reads your calendars
  with your permission and copies their events (titles, start and end times, calendar names,
  links and notes) to Cue's server, so Q and planning can see them like Google Calendar events.
  Disconnecting Apple Calendar in Settings removes those copies from the server.
- **LLM cost records** (how much a request cost), for keeping usage in budget.

## Where it goes

Everything you enter is stored on Cue's server.

By default, when Cue's fast built-in parser can't confidently understand a capture, more than
just that capture's text is sent to OpenAI's API (currently the `gpt-6-luna` model) to help
parse it: your existing task titles, courses, imported event details, your task categories, and
recent /ask conversation history may be included too, so Cue has enough context to understand
you. This "try the fast parser first" behavior is Cue's default mode, not a hard guarantee for
every request — a future mode could send more. See OpenAI's API data usage policy for how they
handle that data.

## Who can see it

Only the Cue team can see your data, and only to run the service and fix bugs.

## How long we keep it

We keep your data until you delete your account. Deleting your account erases it (see below).

## Logs

Our server logs avoid personal content — they record things like request timing and outcome
codes, not the text of what you typed or said.

Crash reports (technical details only, no task text) are sent only with your permission or if you turn on automatic sending.

## Deleting your data

In the Mac app, Settings → Account → **Export My Data…** saves a copy of everything stored for
your account (as a JSON file), and **Delete Account…** erases your account and all of its data
from our server right away. Deletion is permanent: there's no undo, and every Mac signed in to
the account is signed out. Cue forgets a Google Calendar connection on our server, but doesn't
yet revoke it at Google; remove Cue under your Google account's third-party access as well.

## Questions

Report a problem or ask a privacy question: github.com/ysta32/cue-releases/issues
