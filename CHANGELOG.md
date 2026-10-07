# Changelog

All notable changes to Cue for macOS. Versions follow [Semantic Versioning](https://semver.org).
Downloads for every version are on the [Releases](https://github.com/ysta32/cue-releases/releases) page.

## [1.0.0] — 2026-10-07

The first public release. Free for everyone, no invite needed.

### Added
- **Create an account in the app.** Type your first name and you're in. Invite codes still work.
- **Check for Updates…** in the Cue menu, plus a note in Settings when a new version is out.
- Alarm-style requests ("wake me up at 7", "set an alarm for 8 pm to take pills") now make a
  timed task with a reminder at that time, so nothing you say gets lost.

### Changed
- The privacy notice and policy are rewritten for the public release, in plain language.
- Send Feedback falls back to the public issue tracker when you're offline.
- Release downloads are now `Cue-<version>-mac.zip`, with a SHA-256 checksum next to each one.

### Removed
- Leftover alarm cards from the change preview. Alarms left the app in 0.9.0.
- The "Coming soon" placeholder in Settings → Integrations.

## [0.9.0] — 2026-10-06 · Release candidate

The redesign build, shared with testers ahead of 1.0.

### Added
- **A new look.** Light and dark themes, the bubble-shaped Q, a floating sidebar and a calmer Today.
- **Command palette** (⌘K): fuzzy search over actions, tasks, events and categories.
- **Syllabus import**: paste or drop a syllabus, review the deadlines and add them all at once.
- **Class schedule**: paste a timetable and Cue makes the semester's class events.
- **Focus mode**: pomodoro cycles on the task timer, with credit when you check a task off.
- **Evening wrap-up** and **Week in review**, with a weekly recap and a streak badge.
- **At-risk deadlines**: a badge, a Today group, and an honest answer when you ask Q about them.
- **Workload heatmap** on the month view, with a heads-up before a crunch.
- **Recurring tasks**, **snooze**, **subtasks**, **task reminders**, and **links and files** on tasks.
- **Menu bar next-up**: a countdown to your next event and an Up next list.
- **Agenda export** as text, Markdown or CSV, with copy, save, print and share.
- **Spoken briefing**: Cue can read your day aloud.
- **Calendar feed (ICS)** in and out, plus event locations that sync with Google Calendar.
- **Bulk changes by voice**, such as deleting several tasks at once. Always confirmed, with one Undo.

### Changed
- Search is typed right in the sidebar.
- Estimates are a normal-length guess for the task and are never learned from your history.
- An open task is a compact form instead of rows of pills, and clicking outside closes it.

### Fixed
- Deleted tasks stay deleted, even when an old upload is replayed.
- Repeating tasks keep their wall-clock time across daylight-saving changes, and the next
  occurrence always lands after today.
- A damaged local file can no longer upload sample tasks or delete real ones.
- Many voice fixes: filler words in titles, late-night "today/tomorrow", and push-back phrasing.

### Removed
- Routines and Alarms, to keep Cue focused on tasks, events and your calendar.
- Plan my day, Quick wins and the speaker button from Today's header.

## [0.1.0-beta.1] — 2026-10-01 · First beta

The first build for testers.

### Added
- Voice and typed capture from anywhere with **⌥Space**, using on-device Whisper to correct
  the transcript.
- The **Today** view, Canvas feed import, and questions about your schedule ("what's due
  tomorrow?", "am I free at 3?").
- **Google Calendar** and **Apple Calendar**: events come in, and adds, edits and deletes go
  back to your calendar automatically.
- Faster replies: most requests are handled on the spot by Cue's own parser, and the rest
  come back in about 1.3 seconds.

[1.0.0]: https://github.com/ysta32/cue-releases/releases/tag/v1.0.0
[0.9.0]: https://github.com/ysta32/cue-releases/releases/tag/v0.9.0
[0.1.0-beta.1]: https://github.com/ysta32/cue-releases/releases/tag/v0.1.0-beta.1
