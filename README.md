# 🔊 OBS-Friendly-Soundboard

A user-friendly soundboard that seamlessly integrates with OBS and other streaming software using virtual audio cables (like VB-Cable).

## ✨ Features

*   **Easy OBS Integration:** Connects with OBS via virtual audio cables for hassle-free audio routing.
*   **Customizable Sound Packs:** Load your own sounds and organize them with ease.
*   **Hotkey Support:** Assign global hotkeys to your favorite sounds for quick access.
*   **Audio Effects:** Apply effects like reverb and delay to your sounds.
*   **Dark Theme:** A sleek, modern interface that's easy on the eyes.

## 🚀 Getting Started

### 📋 Prerequisites

*   Python 3.x
*   [VB-CABLE Virtual Audio Device](https://vb-audio.com/Cable/) (or any other virtual audio cable)

### 💻 Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/OBS-Friendly-Soundboard.git
    cd OBS-Friendly-Soundboard
    ```

2.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    > **Note:** The `pedalboard` and `pynput` packages are optional. `pedalboard` is for audio effects, and `pynput` is for global hotkey support. They are included in `requirements.txt` for a full-featured experience.

3.  **Download the sound pack:**
    A starter sound pack is available [here](https://files.catbox.moe/qvrvbo.zip). Download and extract the `sounds` folder into the root directory of the project.

4.  **Run the application:**
    ```bash
    python soundboard.py
    ```

## 📝 License

This project is licensed under the **GNU Lesser General Public License v3.0**. See the [LICENSE](LICENSE) file for more details.
