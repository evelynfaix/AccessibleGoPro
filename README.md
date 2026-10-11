# AccessibleGoPro

AccessibleGoPro is a project to make GoPro cameras easier to use for blind and low-vision people through an accessible iPhone app.

The goal is to create a VoiceOver-friendly interface that speaks camera status, exposes the most important controls, and helps users operate the camera without needing to see the device screen.

This project is inspired by the OpenGoPro repository, which defines how to communicate with GoPro devices and provides examples for integration across languages and platforms.

## Why this project matters

Many cameras and devices are designed around visual interfaces. For blind and low-vision users, this creates a major barrier to using the same features that sighted users take for granted.

AccessibleGoPro aims to address that by:

- exposing GoPro status in spoken form
- making key controls accessible through VoiceOver
- using clear, simple auditory feedback for actions and state changes
- allowing blind users to operate basic functions without requiring visual inspection of the camera screen

## Project goals

The first version of the project focuses on a realistic and achievable MVP:

- connect to a GoPro from an iPhone
- read battery level aloud
- read current camera mode aloud
- read whether the camera is recording
- start and stop recording
- take a photo
- switch between photo and video modes
- announce important status changes and errors clearly

## How this relates to OpenGoPro

The OpenGoPro repository provides the protocol and developer resources needed to communicate with GoPro cameras. This project uses that ecosystem as a foundation for building a more accessible user experience.

In practical terms, this means:

- using OpenGoPro as the technical base for GoPro communication
- building a simpler and more accessible mobile interface on top of it
- adapting the API data into spoken, screen-reader-friendly output for blind users

## Why iOS first

This project begins with iOS because the creator has an iPhone and because VoiceOver is a powerful built-in accessibility tool on iPhone. The initial version is designed for accessible iPhone control, while future work may expand to Android, desktop tools, or additional hardware support.

## Proposed MVP flow

A simple first experience could look like this:

1. User opens the app and connects to their GoPro.
2. App announces connection status and camera name.
3. App reads battery level, recording status, and current mode.
4. User taps a button or uses VoiceOver to start/stop recording.
5. App speaks confirmation like "Recording started" or "Photo captured."
6. User can navigate between camera modes and settings with spoken feedback.

## Key accessibility principles

This project follows accessibility-first design:

- everything important must be announced aloud
- all controls must be readable by VoiceOver
- gestures should be simple and discoverable
- status should be spoken clearly and consistently
- haptic and spoken feedback should confirm important actions

## Repository structure

This repository will evolve over time, but the initial structure is expected to include:

- `README.md` — project overview and goals
- `docs/` — design notes, requirements, and accessibility guidance
- `app/` — iOS app source code
- `demos/` — prototype demonstrations and experiments
- `issues/` — contributor tasks and feature ideas

## Contributing

This project is meant to be collaborative.

We welcome help from:

- iOS and Swift developers
- blind and low-vision testers
- accessibility experts
- developers familiar with GoPro APIs, BLE, and Wi‑Fi communication
- people who can help design clearer and more usable spoken user experiences

If you want to contribute, open an issue, suggest a feature, or help prototype the first version.

## Roadmap

### Phase 1: Research and prototype

- confirm the best GoPro communication path using OpenGoPro
- build a simple connection prototype
- create a first VoiceOver-friendly interface
- test spoken status updates and confirmation messages

### Phase 2: MVP user flow

- camera status read aloud
- photo and video controls
- basic mode switching
- accessible connection and error handling

### Phase 3: More complete accessibility

- better spoken summaries of settings
- support for more GoPro features
- more robust testing with blind users
- option to expand to Android or other platforms

## Community and collaboration

This project is especially interested in community input from blind and low-vision users, because they will best understand what makes an interface actually usable.

The first goal is not to build a perfect product immediately. The first goal is to build a working, testable, and accessible proof of concept that can be improved with feedback.

## License

This project is currently in early development. License details may be added as the project evolves.

## Contact

This project is intended to be open and collaborative. If you are interested in joining, contributing, or testing the app, please open an issue or reach out through the repository.

---

AccessibleGoPro is a starting point for building a camera experience that works for blind and low-vision users — not just for people who can see the screen.
