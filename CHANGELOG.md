# Changelog

All notable changes to the **Vibe Up 2.0** apps (Android and iOS)
are summarized here, snapshot by snapshot. When a snapshot is tagged in
*this* repository and archived, it is given its own DOI — see the
[version history table](./README.md#version-history) in the README for
DOIs and links to full release notes.

Only tagged snapshots carry a DOI. Entries dated before this repository
existed were never archived and will not be given a DOI retrospectively;
they are recorded so that the history is complete and so that research
conducted on an earlier version can identify what that version contained.

Because the two apps release on their own cadences, entries below group
releases by period rather than pairing them one-to-one.

This changelog describes changes to the private, closed-source
Android and iOS repositories. It contains summaries only —
no source code, implementation details, or internal documentation.

Changes to the platform (backend) it runs on are recorded separately,
in the platform's own citation repository.

The format is loosely based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

---

## [2026.08.01] — 2026-08-31

**Components in this snapshot:** Android v2.2.2 · iOS v2.1.0

**DOI:** https://doi.org/10.5281/zenodo.22202239

### Android (v2.2.2)

Voice input for aEMA survey questions was introduced in v2.2.1 (2026-08-10);
v2.2.2 refines it. Both are summarized here.

#### Added
- Voice recording as an answer option for survey questions, with on-device
  transcription, matching the iOS app.
- A label beside the voice recording button so its purpose is clear, and a
  live audio spectrum display while recording.
- Recordings are limited to one minute and are stopped if the app is sent to
  the background.
- Participants are guided to system settings when microphone access has been
  permanently declined.

#### Changed
- Transcribed speech is placed into the survey answer immediately after
  recording finishes.
- Voice recording indicators now change within a fixed area, so the recording
  panel no longer jumps.
- Participants are signed out when they are withdrawn or their account is
  deleted; returning to sign-in no longer clears data held on the device.
- The mobile number is pre-filled when a session ends because the sign-in has
  expired.
- Non-speech annotations are removed from transcripts.
- eGift card value updated.

#### Fixed
- Crash in the app tour after the "Get Help" button was moved into the
  overflow menu.
- Bottom navigation buttons could stay hidden behind the voice recording panel.
- Multiple dialogs could appear stacked on top of one another.
- Incomplete voice recording uploads on slower devices.
- A recording is kept rather than lost if the microphone fails mid-recording.
- Padding and sizing issues on survey and cognitive task introduction screens.
- The Coin Canyon introduction image now fits the screen.

### iOS (v2.1.0)
#### Added
- Voice recording as an answer option for survey questions, with a progress
  indicator, a live audio spectrum display and a labelled record button.
- On-device transcription of voice answers.

#### Changed
- Simplified the voice recording screen: the retry and continue buttons and the
  live transcript preview were removed, and the recording indicators now fade
  in place.
- Recordings are limited to one minute and are stopped if the app is sent to
  the background.
- Non-speech annotations are removed from transcripts.
- Updated navigation bar styling for the current iOS release, and added a
  press animation to task cells.
- Updated to the current version of the underlying Conductor platform SDK.
- eGift card value updated.

#### Fixed
- A recording is kept when the audio session is interrupted.
- The microphone button resets when voice capture is cancelled or stopped, and
  participants are guided to system settings when microphone access has been
  permanently declined.
- Back chevron colour on the updated navigation bars.
- The EEfRT introduction skipping a page when moving forward.
- The Coin Canyon introduction image now fits the screen.
- Sizing of panels when they are first shown.

---

## 2026-06 — Android v2.2.0 · iOS v2.0.4–v2.0.5

### Android (v2.2.0)
#### Added
- Tasks can be locked by the study configuration rather than by the app, and
  locked tasks are grouped together in a single list on the dashboard.

#### Fixed
- Surveys could be submitted twice.
- Required-answer validation triggered when simply moving to the next question.
- Push notifications used the wrong credentials.

### iOS (v2.0.4–v2.0.5)
#### Added
- Tasks can be locked by the study configuration; locked tasks are shown in the
  list instead of being hidden, with surveys and recommendations combined into
  one list so they group together.
- Dialog shown after an interrupted task, matching the Android app.

#### Fixed
- The "Day 8" message shown when a participant skipped past the EEfRT task,
  including a correction for participants already affected.
- Interruption handling in the typing task.

## 2026-03 — Android v2.1.3 · v2.1.4

### Android (v2.1.3, v2.1.4)
#### Fixed
- The "Day 8" message shown when a participant skipped the EEfRT task; the
  experiment phase is corrected for participants already affected.
- Crash when the dashboard task list changed.
- Survey screens occasionally failing to load.

## 2026-02 — Android v2.0.3 → v2.1.2 · iOS v2.0.2 · v2.0.3

### Android (v2.0.3 – v2.1.2)
#### Changed
- Clearer loading behaviour on the dashboard when the device is offline.
- Phase 3 congratulations message reworded and the participant information
  link updated.
- Updated to a newer version of the underlying Conductor platform SDK.

#### Fixed
- Crashes when a dialog message could not be retrieved.
- Outstanding activity records are now submitted when a task closes.
- EEfRT timeout handling.

### iOS (v2.0.2, v2.0.3)
#### Changed
- Phase 3 congratulations and welcome message copy updated.
- Participant information link updated.

#### Fixed
- Requests that could hang instead of timing out.

## 2025-10 → 2026-01 — Android v2.0.0 → v2.0.2 · iOS v2.0.1

Android v2.0.0 is the first release of the rebuilt **Vibe Up 2.0** app.

### Android (v2.0.0 – v2.0.2)
#### Added
- Vibe Up 2.0 study logic: experiment phases 1–6 including completion and
  expired states, phase-specific dashboard messaging, and a redesigned
  Overview screen.
- The EEfRT (Effort Expenditure for Rewards Task) in full: introduction and
  task screens, two-step calibration, two-attempt logic, reward calculation
  and payout rounding, an ineligible screen, interruption handling and
  completion screens.
- Cognitive tasks stay locked until both the surveys and the EEfRT task are
  complete.
- Content for the three intervention modules.

#### Changed
- Survey navigation moved to left/right buttons, "answered" reworded to
  "steps", and the navigation separated from the answer options.
- The typing task keyboard rejects AI writing assistance and hardware
  copy/paste, and handles external keyboard input.
- Consent, privacy policy, participant information and support links updated.
- Layouts reworked for small devices and for current Android versions.
- Surveys scroll to the top of the window as each question is shown.
- Clearer dashboard message before the trial starts.

#### Fixed
- Phase detection now accounts for submissions that have been sent but not yet
  received by the study server.
- Repeatable intervention tasks no longer show a "time remaining" label.
- Expired surveys are hidden, and completed intervention content remains
  available in the final phase.
- Two keyboards appearing at once in the typing task.

### iOS (v2.0.1)
#### Changed
- Improved coin collection in the Coin Canyon task.
- The "time remaining" label is hidden for repeatable intervention tasks.

#### Fixed
- Phase detection now accounts for submissions that have been sent but not yet
  received by the study server.
- Intervention tasks appear in the expired phase.
- Surveys scroll to the top of the window as each question is shown.
- Introduction pages on small devices.
- The typing task prompt is no longer selectable.

## 2025-08 → 2025-09 — iOS v1.1.0 · v2.0.0

The rebrand of the iOS app to **Vibe Up 2.0**, together with the EEfRT task and
the intervention modules.

### iOS (v1.1.0)
#### Added
- The EEfRT (Effort-Expenditure for Rewards Task) as a first-class task:
  introduction screens, two-step calibration, reward calculation, completion
  and ineligible screens, and a trial sequence that rotates per experiment
  phase.
- EEfRT resilience: the task resumes correctly after the app is backgrounded
  or closed, and attempts are counted across interruptions.
- Intervention modules, with their dialogs and imagery.
- An uploading screen with a final upload indicator and a "waiting for
  connection" message.
- Overview button, "time remaining" label, "all caught up" messaging, and
  pre-trial messaging counting down to the start of the trial.

#### Changed
- Renamed from Mind GRID to Vibe Up 2.0 throughout, including the app name and
  icon.
- Minimum supported iOS version raised to iOS 16.
- Phase detection brought in line with the Android app and extended through
  phase 6; the day counter updates at midnight.
- Cognitive tasks stay locked until both the surveys and the EEfRT task are
  complete; locked activities are shown beneath available ones.
- App tour screens updated, and wording unified with the Android app.
- Settings links, contact address and eGift card value updated.

#### Fixed
- Day counter stopping at 30, and intervention content appearing twice near the
  end of the trial.
- Completed intervention content stays visible when nothing else is available.
- Task and trial ordering on the dashboard.

### iOS (v2.0.0)
#### Added
- Long press on a task to submit it individually.

#### Changed
- Survey navigation reworded from "answered" to "steps" and moved to
  left/right buttons, with the navigation separated from the answer options.
- "Treatment intervention" renamed to "intervention".
- The EEfRT completion message was updated, and is not shown when the reward
  criteria are not met.
- Landscape orientation removed.

#### Fixed
- Rating question options being highlighted at random.
- Timers in the Back to Front task when returning to the app.
- Duplicate dialogs, including the module complete dialog.
- Phase 1 cognitive tasks now behave the same as later phases.
- Pluralisation of the estimated duration shown on the dashboard.

## Earlier history

Vibe Up 2.0 was built from two earlier products in the same codebases —
**Mind GRID** (2022–2025) and the original **Vibe Up** (2020–2022) — and
version numbering restarted at each change of identity. Those releases
belong to different studies and are not part of Vibe Up 2.0, so they are
not summarized here; they remain recorded in the component repositories.

---

<!--
Template for a new entry:

## [yyyy.mm.micro] — yyyy-mm-dd

**Components in this snapshot:** Android vX.X.X · iOS vX.X.X

**DOI:** 10.xxxx/zenodo.xxxxxxx

### Android (vX.X.X)
#### Added / Changed / Fixed / Removed / Security
- ...

### iOS (vX.X.X)
#### Added / Changed / Fixed / Removed / Security
- ...

Only include a component's section if it shipped a new version since
the last snapshot. Only include a subheading (Added/Changed/etc.) if
it has entries. Keep descriptions at the feature/behavior level —
no source code, file names, internal ticket numbers, or architecture
details.
-->
