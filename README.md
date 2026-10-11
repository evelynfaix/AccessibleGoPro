# AccessibleGoPro

AccessibleGoPro is a project to make GoPro cameras easier to use for blind and low-vision people through an accessible iPhone app.

The core goal is to enable blind users to record video, manage all camera settings, and control key GoPro features without needing to see the camera screen.

This project is inspired by the OpenGoPro repository, which defines how to communicate with GoPro devices and provides examples for integration across languages and platforms.

## Why this project matters

Many camera systems are designed around visual feedback. For blind and low-vision users, that creates a major barrier to basic recording tasks such as starting a capture, switching modes, checking battery, and managing settings.

AccessibleGoPro aims to remove that barrier by:

- speaking camera status aloud using VoiceOver
- exposing all important GoPro settings in an accessible menu
- allowing blind users to change resolution, frame rate, ISO, white balance, and other settings without sight
- confirming actions with spoken feedback and haptic cues
- making video recording and camera management independent for blind users

## Video-first mission with complete settings control

This project is especially focused on video capture because recording video is one of the most important GoPro use cases. But to make GoPro truly accessible, users need to be able to adjust all settings to fit their needs.

The first version is designed around these core tasks:

**Recording:**
- start recording video
- stop recording video
- confirm recording state aloud
- announce battery level while recording
- announce mode and settings before and during capture

**Settings management:**
- read current values for all available camera settings
- change resolution and frame rate
- adjust ISO and exposure
- control white balance and color
- manage audio settings
- adjust stabilization and lens options
- set up timelapse or slow motion
- manage file format and codec settings
- adjust any other GoPro feature

**Status and feedback:**
- announce important status changes and errors
- confirm each setting change aloud
- read available options for each setting
- help users understand what each setting does

## Project goals

The first version of the project focuses on a realistic and achievable MVP:

- connect to a GoPro from an iPhone
- read battery level and current mode aloud
- read all current camera settings
- start and stop recording
- take a photo
- switch between photo and video modes
- **allow changing all major camera settings (resolution, frame rate, ISO, white balance, etc.)**
- announce important status changes and errors clearly
- provide spoken confirmation for every setting change

## How this relates to OpenGoPro

The OpenGoPro repository provides the protocol and developer resources needed to communicate with GoPro cameras and access their full feature set. This project uses that ecosystem as a foundation for building a more accessible user experience.

In practical terms, this means:

- using OpenGoPro as the technical base for GoPro communication
- leveraging the OpenGoPro protocol to expose all available camera settings
- building a simpler and more accessible mobile interface on top of it
- adapting the API data into spoken, screen-reader-friendly output for blind users
- translating complex camera settings into clear, understandable language

## Why iOS first

This project begins with iOS because the creator has an iPhone and because VoiceOver is a powerful built-in accessibility tool on iPhone. The initial version is designed for accessible iPhone control, while future work may expand to Android, desktop tools, or additional hardware support.

## Proposed MVP flow

A simple first experience could look like this:

1. User opens the app and connects to their GoPro.
2. App announces connection status and camera name.
3. App reads battery level, recording status, and current mode.
4. App offers a menu of settings to adjust.
5. User navigates through settings using VoiceOver.
6. User selects a setting (e.g., "Resolution") and hears current value.
7. App offers options: "1080p at 60fps, 2.7K at 30fps, 4K at 24fps..."
8. User selects a new option.
9. App speaks confirmation: "Resolution changed to 4K at 24fps."
10. User can start recording or adjust more settings.

## Key accessibility principles

This project follows accessibility-first design:

- everything important must be announced aloud
- all controls must be readable by VoiceOver
- gestures should be simple and discoverable
- status should be spoken clearly and consistently
- haptic and spoken feedback should confirm important actions
- recording actions should be easy to trigger without looking at the screen
- settings should be presented in a logical, hierarchical way
- every setting change should be confirmed aloud

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
- people who know GoPro settings and can help translate them into clear spoken descriptions

If you want to contribute, open an issue, suggest a feature, or help prototype the first version.

## Roadmap

### Phase 1: Research and prototype

- confirm the best GoPro communication path using OpenGoPro
- build a simple connection prototype
- map all available GoPro settings and their possible values
- create a first VoiceOver-friendly settings interface
- test spoken status updates and confirmation messages
- confirm support for basic video recording and settings control

### Phase 2: MVP user flow

- camera status read aloud
- complete settings management interface
- photo and video controls
- basic mode switching
- accessible connection and error handling
- recording start/stop confirmations
- clear spoken descriptions of each setting and its options

### Phase 3: More complete accessibility

- better spoken summaries of settings and their effects
- support for advanced GoPro features and presets
- more robust testing with blind users
- option to expand to Android or other platforms
- voice command support for common settings changes

## Community and collaboration

This project is especially interested in community input from blind and low-vision users, because they will best understand what makes an interface actually usable.

The first goal is not to build a perfect product immediately. The first goal is to build a working, testable, and accessible proof of concept that can be improved with feedback.

## License

This project is currently in early development. License details may be added as the project evolves.

## Contact

This project is intended to be open and collaborative. If you are interested in joining, contributing, or testing the app, please open an issue or reach out through the repository.

---

AccessibleGoPro is a starting point for building a camera experience that works for blind and low-vision users — enabling them to record video and manage all camera settings independently.
