# 🎵 Music Player Service


A modular and extensible **iOS Music Player** built using **MVVM architecture with Combine**. This project demonstrates the application of key design patterns while supporting multiple music sources (Local files and Spotify-mock), real-time playback management, queue handling, and UI state notifications.


 📍 Repository: [GirdharGopal21/Music-Player-Service-](https://github.com/GirdharGopal21/Music-Player-Service-.git)

---


## 🚀 Features


### 🎶 Multiple Music Sources

- ✅ **Local Files**: Play songs stored on the device

- ✅ **Spotify Mock**: Simulated streaming integration

- 🔌 Unified `MusicSourceProtocol` to abstract implementation

- 🧱 Easily extendable for new platforms (e.g., YouTube, Apple Music)


### ⏯ Playback Control

- Play, pause, skip next, and previous controls

- Maintain accurate playback state

- Works seamlessly with a dynamic playlist queue


### 🗂 Playlist Queue Management

- Add/remove tracks

- Reorder tracks on the go

- Automatic transition on track completion


### 📡 Real-time State Notifications

- Reactive UI via **Combine**

- Playback status: playing, paused, stopped

- Progress: current time & total duration

- Broadcast to multiple UI components


### 💡 MVVM + Combine Architecture

- Clear separation of concerns

- Observables for real-time communication

- Clean and testable ViewModel logic


### 🔒 Singleton Music Player Instance

- Central audio session management

- Prevents multiple audio conflicts

- Ensures consistent playback behavior


---


## 🛠 Technologies Used

- Swift 5.5+

- Combine

- MVVM Architecture

- AVFoundation

- Xcode 13+

---


## 🧠 Design Patterns Implemented

| Pattern         | Purpose                                      |
|-----------------|----------------------------------------------|
| Strategy        | Encapsulate multiple music source behaviors  |
| Observer        | Notify UI with Combine publishers            |
| Singleton       | Single music player instance                 |
| Command         | Handle user actions like play/pause          |

---


## 🗂 Project Structure



Music-Player-Service-/
├── Models/
│   └── Track.swift, PlaybackState.swift
├── Sources/
│   └── LocalFileSource.swift, SpotifyMockSource.swift
├── ViewModel/
│   └── PlayerViewModel.swift
├── Services/
│   └── MusicPlayerService.swift
├── Views/
│   └── PlayerView\.swift, PlaylistView\.swift



---

## 🧪 Setup & Run

1. Clone the repo:

   bash

    git clone https://github.com/GirdharGopal21/Music-Player-Service-.git

   cd Music-Player-Service-


3. Open the project in Xcode:


   bash

   open Music-Player-Service-.xcodeproj
   

5. Build & run on iOS Simulator or real device.


---


## 🔧 Adding New Music Sources


To add support for a new platform:


1. Create a class that implements `MusicSourceProtocol`

2. Handle source-specific initialization and playback

3. Register it with `MusicPlayerService`

No changes needed in existing code!

---

## 🙌 Contributions

Feel free to:

* ⭐ Star the repo

* 🐛 Report bugs

* 📥 Submit pull requests

---

## 📄 License

MIT License © [Girdhar Gopal](https://github.com/GirdharGopal21)

---
