# Stage of Light - Six Customized Videos

![Stage of Light Scene Preview](https://github.com/hsuehyt/StageOfLight6CustomizedVideos/blob/main/README/Screenshot%202024-11-19%20143629.png)

**Stage of Light - Six Customized Videos** is a Unity project created for NTNU Art Museum. It enables the seamless projection of six customized videos across the walls and floors of the immersive exhibition space, "Stage of Light." This project uses a Windows-based dome projection system integrated with **Resolume Arena**, ensuring the Unity project's build folder runs smoothly for immersive visual experiences.

This project also incorporates multimedia tools such as Keijiro.Klak.SPOUT for Spout-based video output and iam1337.extOSC for Open Sound Control (OSC) functionality, providing a versatile framework for interactive and immersive installations.  

For a solution using a single panoramic video, please refer to [Stage of Light - One Panoramic Video](https://github.com/hsuehyt/StageOfLight1PanoramicVideo).

---

## Table of Contents
1. [Features](#features)
2. [Getting Started](#getting-started)
3. [Adding Your Videos](#adding-your-videos)
4. [Video Format and Recommendations](#video-format-and-recommendations)
5. [Building the Project](#building-the-project)
6. [Demo Video](#demo-video)
7. [Preview of Six Surfaces](#preview-of-six-surfaces)
8. [Credits](#credits)

---

## Features

- **Simplified Workflow:** Flat videos are easier to create than 360° panoramic videos, reducing the need for advanced content creation skills.  
- **Optimized for Room Shape:** Tailored for the elongated room, minimizing distortion and ensuring accurate alignment with projection surfaces.  
- **Flexible and Modular:** Quickly update or replace individual videos without reprocessing the entire project, allowing for customized storytelling.  

---

## Getting Started

### Prerequisites
- Unity Editor **2021.3.6f1** or later (2021.3.6f1 is recommended).

### Installation
1. Clone or download the project:
   ```bash
   git clone https://github.com/hsuehyt/StageOfLight6CustomizedVideos
   ```
2. Extract the zip file (if downloaded) and add the project to Unity Hub.
3. Open the project in Unity.

### Opening the Scene
1. Navigate to `Assets/StageOfLight/`.
2. Open the scene named **`6CustomizedVideos`**.
3. Click **Play** to test the scene.

---

## Adding Your Videos

![Adding Your Videos Preview](https://github.com/hsuehyt/StageOfLight6CustomizedVideos/blob/main/README/Screenshot%202024-11-19%20160751.png)

1. Import your videos into `Assets/StageOfLight/`.
2. In the **Hierarchy** panel, select `VideoPlayers`.
3. In the **Inspector** panel, under the component `Video Players > Video Clip`, drag and drop each video into its corresponding slot (e.g., Ground to Ground, Wall Canted to Wall Canted) to assign content to replace the demo content.
4. Test the videos by playing the scene.

---

## Video Format and Recommendations

### Format Specifications

| Surface              | Resolution   |
|-----------------------|--------------|
| Ground 地板           | 4096x910     |
| Ground Canted 斜地板  | 4096x960     |
| Wall Canted 斜面牆    | 4096x828     |
| Wall Left 左邊牆面 (facing canted wall) | 1988x1128    |
| Wall Right 右邊牆面 (facing canted wall) | 1988x1128    |
| Wall Vertical 有門的牆 | 4096x1128    |

### Encoding with Adobe Media Encoder
- **Preset:** `H.264 > Match Source - Adaptive Low Bitrate`  
- For better quality, use `Match Source - Adaptive Mid Bitrate` or `Match Source - Adaptive High Bitrate`.

⚠ **Note:** High bitrate settings may cause playback issues for longer videos due to increased file sizes.

---

## Building the Project

1. Open **File > Build Settings** in Unity.
2. Ensure **StageOfLight/6CustomizedVideos** is checked in **Scenes in Build**.
3. Click **Build**, and follow the prompts to create the build folder.

---

## Demo Video

[![Watch the Demo Video](https://img.youtube.com/vi/rCksp6MYeFc/0.jpg)](https://youtu.be/rCksp6MYeFc)

---

## Preview of Six Surfaces

### Top Angle View
![Top Angle View](https://github.com/hsuehyt/StageOfLight6CustomizedVideos/blob/main/README/Screenshot%202024-11-20%20005038.png)

### Right Angle View
![Right Angle View](https://github.com/hsuehyt/StageOfLight6CustomizedVideos/blob/main/README/Screenshot%202024-11-20%20005312.png)

---

## Credits

- **The Original Unity Project Developer:** [李綠恩 Lu-En Li](https://github.com/LeeMegumi)  
- **The Project Maintainer and Developer:** [薛佑廷 Yuting Hsueh](https://github.com/hsuehyt)  
- **Integrated Tools:**  
  - **Keijiro.Klak.SPOUT** from [Keijiro's Scoped Registry](https://github.com/keijiro)  
  - **iam1337.extOSC** from [OpenUPM](https://package.openupm.com)  

### Supervising Institutions
- **教育部 前瞻顯示科技與跨領域人才培育計畫 總計畫辦公室 Advanced Display Technology & Interdisciplinary Talent Cultivation Project Office, Ministry of Education**
- **臺師大 前瞻顯示科技導入藝術場域建置與推廣計畫 NTNU Advanced Display Technology Integration & Promotion in Art Venues**  
- **臺師大 美術館 NTNU Art Museum**