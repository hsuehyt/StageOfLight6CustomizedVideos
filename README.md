# Stage of Light - Six Customized Videos

![Stage of Light Scene Preview](https://github.com/hsuehyt/StageOfLight6CustomizedVideos/blob/main/README/Screenshot%202024-11-19%20143629.png)

**Stage of Light - Six Customized Videos** is a Unity project designed for NTNU Art Museum. It enables the projection of six customized videos onto the respective walls and floors of the immersive projection space, "Stage of Light." This project leverages a Windows-based dome projection system integrated with **Resolume Arena** to display the Unity project's build folder seamlessly.

---

## Table of Contents
1. [Features](#features)
2. [Getting Started](#getting-started)
3. [Adding Your Video](#adding-your-video)
4. [Video Format and Recommendations](#video-format-and-recommendations)
5. [Building the Project](#building-the-project)
6. [Demo Video](#demo-video)
7. [Credits](#credits)

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

### Multi-Surface Projection Mapping

- **Consistency:** Ensure consistency in backgrounds and transitions across all six videos to create a cohesive and seamless experience.  
- **Hardware Performance:** Test your system’s ability to play six video streams simultaneously without lag or performance drops.  
- **Testing and Calibration:** Align and thoroughly test videos to avoid distortion and cropping, particularly for the elongated room layout.

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

[![Watch the Demo Video](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20132004cropped.png)](https://youtu.be/3P2WE4laE2U)

---

## Credits

- **Original Unity Project Design:** [李綠恩 Lu-En Li](https://github.com/LeeMegumi)  
- **Project Revision and Tutorial Demonstration:** [薛佑廷 Yuting Hsueh](https://github.com/hsuehyt)

### Supervising Institutions
- **Advanced Display Technology & Interdisciplinary Talent Cultivation Project Office**, Ministry of Education  
- **NTNU Advanced Display Technology Integration & Promotion in Art Venues**  
- **NTNU Art Museum**