# Changelog

All notable changes to Cue for macOS. Versions follow [Semantic Versioning](https://semver.org).
Downloads for every version are on the [Releases](https://github.com/ysta32/cue-releases/releases) page.

## [1.3.1] — 2026-10-08

Today now tells you why a task is first.

### Added
- **See why a task is near the top.** Today shows a short reason under each task, and in its
  tooltip.

### Changed
- Your morning summary notification, wrap-up, the agenda export and Today's tips follow the same
  smart order as Today, and notifications update when that order changes.

### Fixed
- Canvas items you deleted stay deleted, even if Canvas briefly drops them from your feed. Old
  deletion records clear themselves once the item has been gone from Canvas for 30 days.
- Safer requests: there is now a limit on one capture field.

## [1.3.0] — 2026-10-07

A fresh look, and your timer, working hours and weekly review now match on every Mac.

### Added
- **A new look.** A new pixel Q logo and app icon, and a redesign of Today, capture, the task
  editor, focus, history, the weekly review and Settings. A **Text size** setting is in
  Settings → Appearance.
- **Your timer follows you.** Time logged on a task and your working hours sync between Macs.
  Logged time never goes down unless you reset it.
- **Focus from anywhere.** "focus on physics for 50 minutes" or "stop focusing"; the time counts
  toward the task.
- **Smarter order.** Cue learns from your deadlines and how you finish work, and uses it to order
  Today and to answer "what should I do first?".
- **Better new-item cards.** Edit the place and notes before you save, and turn Add to Google
  Calendar on or off for new events when Google Calendar is connected with permission to add events.

### Changed
- At risk uses your working hours and logged time, so Q agrees with the badge on your Mac. When
  something is at risk, Q offers to start a focus session on it from Today.
- The weekly review matches on every Mac.
- "Due soon" shows the time Cue planned for each day, not an even split.

### Fixed
- Adding something that is already on a list does nothing.
- A trailing "urgent" is understood, and a bare 11:59 means the end of the day.
- A crash can no longer bring back things you deleted on another Mac.
- Canvas items you deleted stay deleted.

## [1.2.0] — 2026-10-07

Your tasks follow you between Macs, and Cue understands more of what you say.

### Added
- **More follows you.** A task's checklist, extra links and reminder choice sync to your other
  Mac, and so do your class schedule and the locations of Apple Calendar events.
- **Places and notes from speech.** "study group at Levine 101 at 6" saves the place as the
  location; "dinner at 7, bring the charger" saves the extra words as a note.
- "Delete the laundry one" now works.

### Changed
- The plan no longer counts work due earlier again on later days.
- Pairing codes have an extra limit on how often they can be tried across all Macs.

### Removed
- Cue no longer speaks: the spoken briefing and spoken answers are gone. Q still answers in text.

## [1.1.0] — 2026-10-07

Plan a whole week by voice, use Cue on a second Mac, and plainer messages when something goes wrong.

### Added
- **Plan your week.** "study 6 hours this week" or "gym 3 times this week" shows a card of sessions
  in your free time, from today through Sunday (on a Sunday, through the following Sunday).
- **Use Cue on another Mac.** Settings → Account → Use Cue on another Mac gives a code that works
  once, for 10 minutes.
- **Edit by voice.** Move, rename or delete a task by saying so; Cue asks which one if several fit.
- Task locations sync between Macs.
- Help → Cue Help and Help → Contact Support, and credits and links in About.
- **Connect again** for Google Calendar when it lacks permission to change events.

### Changed
- Setup has an account step you can skip, asks before downloading the 480 MB voice model, and
  leaves Open Cue when I log in off.
- Errors read as plain sentences. Cue says when you're offline, when notifications or the
  microphone are off, and when a request was saved only in Cue.
- Real accounts no longer see sample tasks. Failed saves can be retried. Error logs keep only the
  type of error, never what you wrote.

## [1.0.0] — 2026-10-07

The first public release. Free for everyone, no invite needed.

### Added
- **Create an account in the app.** Type your first name and you're in. Invite codes still work.
- **Check for Updates…** in the Cue menu, plus a note in Settings when a new version is out.
- Alarm-style requests ("wake me up at 7", "set an alarm for 8 pm to take pills") now make a
  timed task with a reminder at that time, so nothing you say gets lost.
- Reminders that come with a request follow later changes to it. A reminder you pick on your Mac
  is never overwritten.

### Changed
- The privacy notice and policy are rewritten for the public release, in plain language.
- The privacy notice and policy now say that Apple Calendar events, if you connect it, are copied
  to Cue's server so Q and planning can use them.
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
