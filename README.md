# GSoC '24 Report - VLC : The Ultimate Media Player

**Student:** Darshan Jain ([@Thrillseekr](https://code.videolan.org/Thrillseekr))

**Organization:** [VideoLAN](https://www.videolan.org/)

**Project:** [VLC Qt Interface Redesign](https://summerofcode.withgoogle.com/programs/2024/projects/qOI0v3an)

**Time zone:** Indian Standard Time (UTC + 5:30)

**Mentor:** Pierre Lamot
<br>

---

## VLC 4.0 Project
VLC 4.0 introduces a modern Qt interface that enhances usability while maintaining the familiar experience users love. This update brings a fresh look, making interaction smoother for billions of users worldwide. VLC remains a versatile, open-source multimedia engine, offering broad compatibility across platforms and devices, making it a top choice for media playback.

### VLC Qt Interface 
The VLC 4.0 Qt interface brings a sleek, modern design that enhances usability and visual appeal. Prioritizing clarity and ease of use, this interface offers an intuitive experience. Its versatility shines across both Windows and GNU/Linux, providing consistent multimedia performance and accessibility for users on various platforms.
 
The video section is a modern design with quick access to recently watched content, making navigation easy. The music section is organized into Artists, Albums, Tracks, and Genres for effortless browsing. Tracks are neatly listed with sorting options by title, artist, and more. Playlists are customizable and seamless, offering easy control for creating the perfect media mix.

---

## Milestones

### 📌 Jan - May : Contributions before Official Coding Period

⇒ MR: [!4841](https://code.videolan.org/videolan/vlc/-/merge_requests/4841) (Merged)\
&nbsp;&nbsp;&nbsp; Commit: [32896e88](https://code.videolan.org/videolan/vlc/-/commit/32896e8848c7421f00d962e381eb457486462f37?merge_request_iid=4841) qml: fix Mismatching string in MusicArtist.qml

⇒ MR: [!5047](https://code.videolan.org/videolan/vlc/-/merge_requests/5047) (Merged)\
&nbsp;&nbsp;&nbsp; Commit: [50960ca5](https://code.videolan.org/videolan/vlc/-/commit/50960ca5531e9e8b43e3a41a28cd928b6d2d4da2?merge_request_iid=5047) qt: mlplaylist: Display duration from MediaLibrary

⇒ Issue: [#28341](https://code.videolan.org/videolan/vlc/-/issues/28341)\
&nbsp;&nbsp;&nbsp; MR: [!4984](https://code.videolan.org/videolan/vlc/-/merge_requests/4984) (Merged)\
&nbsp;&nbsp;&nbsp; Commit: [4aecd897](https://code.videolan.org/videolan/vlc/-/commit/4aecd897f708d8f41e35b9d50081d82dd70c63f6?merge_request_iid=4984) qt: Update CSD Icons to Segoe Fonts available in different Windows Version

⇒ Issue: [#28505](https://code.videolan.org/videolan/vlc/-/issues/28505)\
&nbsp;&nbsp;&nbsp; MR: [!5045](https://code.videolan.org/videolan/vlc/-/merge_requests/5045) (Merged)\
&nbsp;&nbsp;&nbsp; Commits:\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; • [f4a2f119](https://code.videolan.org/videolan/vlc/-/commit/f4a2f119199788316da7a11fbd06fd7b263984ba?merge_request_iid=5045) qt: mlalbummodel: Sort Title by Alphabetical Order\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; • [5cd2d7ae](https://code.videolan.org/videolan/vlc/-/commit/5cd2d7aec11914d0e6c6ef0b5e7c02aeb1bc3e3b?merge_request_iid=5045) qt: MusicArtistsAlbums: add Release Year Sorting Criteria for Albums

⇒ MR: [!5081](https://code.videolan.org/videolan/vlc/-/merge_requests/5081) (Merged)\
&nbsp;&nbsp;&nbsp; Commit: [32896e88](https://code.videolan.org/videolan/vlc/-/commit/32896e8848c7421f00d962e381eb457486462f37?merge_request_iid=4841) qt: CSDWindowButton: import org.videolan.vlc 0.1 library for rendering MainCtx\

⇒ Issue: [#28422](https://code.videolan.org/videolan/vlc/-/issues/28422)\
&nbsp;&nbsp;&nbsp; MR: [!4892](https://code.videolan.org/videolan/vlc/-/merge_requests/4892) (Merged)\
&nbsp;&nbsp;&nbsp; Commits: [c55688b7](https://code.videolan.org/videolan/vlc/-/commit/c55688b7fcd3b231c45bc84a4e2860a37c475fa8?merge_request_iid=4892) qml: Renamed File ScrollingText.qml

<br>

### 📌 May 1 - May 26 : Community Bonding Period
During the community bonding period, I actively engaged with mentors, senior members, and fellow contributors to learn more about their projects and working domains within VLC. I also resumed contributions to the VLC Qt Interface and dedicated time to exploring and learning [GammaRay](https://github.com/KDAB/GammaRay) (a powerful tool developed by KDAB for inspecting and debugging Qt applications) and its features. This interaction and learning laid a strong foundation for my GSoC journey.

<br>

### 📌 May 27 - Aug 19 : Coding Period

#### ✔ Task 1  : Introducing Minimal View for Player
&nbsp;&nbsp;&nbsp; The Minimal View in VLC is a simplified interface mode designed to focus on core media playback functions\
&nbsp;&nbsp;&nbsp; while minimizing distractions. Key features include:

- **Compact User Interface:** The interface is streamlined, showing only essential playback controls like play, pause, and volume.
- **Reduced Controls:** Advanced settings and non-critical features like playlists are hidden, ensuring a clutter-free experience.
- **Focus on Content:** The emphasis is on media playback by maximizing screen space and minimizing distractions.
- **Customizable Appearance:** Users can customize which controls remain visible and switch between Minimal View and detailed views.

&nbsp;&nbsp;&nbsp; **Implementation in VLC:**
- **Qt Interface:** Access Minimal View options in VLC Preferences.
- **Keyboard Shortcut:** Activate Minimal View using `Ctrl+H`.
- **View Menu:** Enable Minimal View from the top-right View menu.

#### &nbsp;&nbsp;&nbsp; Commits:
- [qt: MainCtx: Expose Minimal View Property](https://code.videolan.org/Thrillseekr/vlc/-/merge_requests/13/diffs?commit_id=af01e00eaff39a1cfc73d2bc10640b7b002d7a86)
- [qt: Update Makefile & meson.build with PlayerToolbarVisibility & MinimalView class](https://code.videolan.org/Thrillseekr/vlc/-/merge_requests/13/diffs?commit_id=e2b0c35e699d4a40fa4e22c5794085edd039945a)
- [qt: Menus: Add QmlAudioContextMenu for Music Playback and Update Player Menus with close() function](https://code.videolan.org/Thrillseekr/vlc/-/merge_requests/13/diffs?commit_id=17577fc9fed6c60efa2db945116a4d85819f0f41)
- [qml: Player: Update PlayerPlaylistVisibility State Machine](https://code.videolan.org/Thrillseekr/vlc/-/merge_requests/13/diffs?commit_id=47dc9ebc0097d33d30bad2b87734f02db64661ef)
- [qml: Player: Update Player.qml Minimal View and other features](https://code.videolan.org/Thrillseekr/vlc/-/merge_requests/13/diffs?commit_id=e9422ce0e55617a987c80bac40e4b8f8284de2ba)
- [qml: Menus: Access Minimal View from View Menu and Shortcut "CTRL + H"](https://code.videolan.org/Thrillseekr/vlc/-/merge_requests/13/diffs?commit_id=3d0692170575d7c6bf3ad674da8e9704d5b29de8)
- [qml: Player: Implementing Force Unlock to Player components](https://code.videolan.org/Thrillseekr/vlc/-/merge_requests/13/diffs?commit_id=34ff48c4c800966be9f5bc1910f52598313bf2c6)

#### 📌 July 12 : Mid - Term Evaluations

#### ✔ Task 2  :

#### ✔ Task 3  :
