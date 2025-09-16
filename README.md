# 🔊 Live-Soundboard

A straightforward soundboard for live streaming, gaming, and voice chat. Play sounds and easily route them to any application like OBS or Discord using a virtual audio cable.

## 📖 Background

This project started with a simple goal: to have the perfect sound effect ready for any moment in a multiplayer game with friends. It has since evolved into a more powerful tool for streamers and content creators, but at its heart, it's about adding a bit of fun and personality to your online interactions.

## ✨ Features

*   **🎧 Flexible Audio Routing:** Directly output audio to any playback device, including virtual audio cables like VB-Cable, allowing for easy integration with streaming software like OBS or voice chat applications.
*   **⌨️ System-Wide Hotkeys:** Trigger sounds from anywhere on your computer, even when the soundboard is minimized or you're in a full-screen game. (Requires `pynput`)
*   **🎛️ Sound Customization:** Adjust the volume for each sound individually and apply audio effects like Reverb and Delay.
*   **📂 Sound Organization:** Group your sounds into tabs for better organization and quick access.
*   **🔍 Quick Search:** Easily find the sound you're looking for with a built-in search bar that filters sounds in the current tab.
*   **💅 Modern Interface:** A sleek, dark-themed interface that is easy to navigate.

## 🚀 Getting Started

### 📋 Prerequisites

*   Python 3.x
*   An installed virtual audio cable, such as [VB-CABLE Virtual Audio Device](https://vb-audio.com/Cable/).

### 💻 Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/Live-Soundboard.git
    cd Live-Soundboard
    ```

2.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    > **Note:** The `pedalboard` and `pynput` packages are optional but included in `requirements.txt` for a full-featured experience. `pedalboard` is for audio effects, and `pynput` is for global hotkey support.

3.  **Download the sound pack:**
    A starter sound pack is available [here](https://files.catbox.moe/qvrvbo.zip). Download and extract the `sounds` folder into the root directory of the project.

4.  **Run the application:**
    ```bash
    python soundboard.py
    ```

## Usage

### OBS Integration

The integration with OBS is not automatic, but it is straightforward. Here's how to set it up:

1.  **In the Soundboard Application:**
    *   Go to `File > Settings`.
    *   In the `Audio Output Device` dropdown, select your virtual audio cable's **input** device (e.g., `CABLE Input (VB-Audio Virtual Cable)`).
    *   Click `OK` to save.

2.  **In OBS Studio:**
    *   In the `Sources` panel, click the `+` button and add an `Audio Input Capture` source.
    *   Name it something descriptive, like "Soundboard".
    *   In the properties for the new source, select your virtual audio cable's **output** device (e.g., `CABLE Output (VB-Audio Virtual Cable)`) from the `Device` dropdown.
    *   Click `OK`.

Now, any sound played from the soundboard will be routed through the virtual cable and captured by OBS as a separate audio source, which you can then mix into your stream.

### Adding and Managing Sounds

*   **Add Sounds:** Click the "Add Sound(s)" button to open a file dialog and select one or more audio files. They will be added to the "Default" group.
*   **Edit Sounds:** Right-click on any sound button to open a context menu where you can:
    *   **Edit Properties:** Change the sound's name, volume, and group. You can also enable and configure effects here.
    *   **Assign Hotkey:** Set a global hotkey for the sound.
    *   **Relink Missing File:** If a sound file has been moved, you can relink it to its new location.
    *   **Delete Sound:** Remove the sound from the soundboard.
*   **Manage Groups:** Go to `Edit > Manage Groups` to add, rename, or delete sound groups (tabs).

## 📝 License

This project is licensed under the **GNU Lesser General Public License v3.0**. See the [LICENSE](LICENSE) file for more details.
