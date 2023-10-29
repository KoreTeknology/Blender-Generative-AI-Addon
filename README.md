<img alt="preview_v135" src="/media/header_addon.png">

A research script based on *Artificial Intelligence* for Blender[^1], this is a multi-steps development project, with **LLM Local System**[^2] focus in mind. This script/addon is intended to serve the purpose to *generate unique images and video sequences*, within **Blender Nodes Editor** and based on Public Checkpoint Models[^3] OR/AND **Private custom Models and LoRas**[^4]. It includes an integrated learning machine process as well as a workflows exporter script.

<img src="https://img.shields.io/badge/Windows-11-purple" /> <img src="https://img.shields.io/badge/Blender-3.6.5/4-c11b3f" /> <img src="https://img.shields.io/badge/Python-3.10-blue" /> <img src="https://img.shields.io/badge/Addon-3.6.5-yellow" /> <img src="https://img.shields.io/badge/CAN-X.1567D-943585" />



## :radio_button: Acknowledgments

```py
NOTE: This project is derived from the K.Sharon & Yorha4D work, called "ComfyUI-BlenderAI-node".
Link: https://github.com/AIGODLIKE/ComfyUI-BlenderAI-node
Release: 1.2.9 - Licensed under GNU General Public License v3.0
```

*"I decided to re-write this addon for several reasons. The first was that the original translation was in Chinese and that some errors appeared due to non-standard characters. The second was that the interface deserved to be redesigned to integrate into my workflow. The third was that I wanted to add functions for animation and the video sequencer. And the last because I couldn't contact the developers of the project and offer my collaboration."*

---

## :radio_button: Objectives

The objectives of this project are to offer different digital creation tools, using Blender as the main platform and only in local environment. At a time when Blender 4x is in the process of being officially released, the main goal is to deliver this addon as soon as this new version of our favorite software is released. Here is a non-exhaustive list of planned features:

- **Create images from prompts (background image, textures, hdri, titles)**
- **Create images from images (styles, tones, themes)**
- **Create texts from prompts (subtitles)**
- **Create images sequences from prompts/images (video strips, animations)**
- **Create audio strips from prompts/images (voices, music themes)**

---

## :radio_button: Features & Updates *(3.6.5 Beta Addon Release)*

- Image API generation (using a NEW **Node Editor** window)
- **ComfyUI Server** connection for local sessions ([ComfyUI](https://github.com/comfyanonymous/ComfyUI) via [Stability Matrix](https://github.com/LykosAI/StabilityMatrix) ) PC Only!
- **Stable diffusion models** custom nodes, support *SD 1.5*, *2.0* and *XL 1.0* ([See tested Models List](TESTED_MODELS.md))
- **Custom** checkpoints, LoRas, VAE loading/merging nodes
- **Processing** Text-2-Single images and Image sequences, **rendering/storing**
- **Processing** Script-2-Prompt GPT-2 based custom nodes
- **Processing** **3D scene**-2-rendered image custom nodes
- **Processing** image-2-**Images-Sequence_Strip** option
- **Preferences** Panel (Server Settings, LLM Settings, Options)
- **NodeTree Editor Tools** Panel (N) with Presets collection
- **Automatic generated content saving** in .blend file

### Todo List: [See next steps development phases](TODO_LIST.md) *Updated: 26/10/2023*



<img alt="preview_v135" src="/media/addon_preview_v125.png">

---

## :radio_button: ComfyUI Installation and Modules

After installing [**ComfyUI**](https://github.com/comfyanonymous/ComfyUI) with your prefered plateform (i am using **Stability Matrix**), make sure you install the additional modules. Then you need to install [GIT software](https://git-scm.com/) (if it is not done already) on your computer. To install these modules, open a CMD window in the \ComfyUI\custom_nodes folder. And "git clone" each one of them. By adding the link after "git clone".

- [ComfyUi-Manager](https://github.com/ltdrdata/ComfyUI-Manager)
- [ComfyUI-Impact](https://github.com/ltdrdata/ComfyUI-Impact-Pack)
- [ComfyUI-Inspire](https://github.com/ltdrdata/ComfyUI-Inspire-Pack)
- [WAS Nodes Suite](https://github.com/WASasquatch/was-node-suite-comfyui)
- [Animate Diff](https://github.com/ArtVentureX/comfyui-animatediff)
- [Prompt-Expansion](https://github.com/meap158/ComfyUI-Prompt-Expansion)
- [Derfuu-ComfyUI_ModdedNodes](https://github.com/Derfuu/Derfuu_ComfyUI_ModdedNodes)

---

## :radio_button: Blender Addon Installation

- Go to the user preferences screen (Edit -> User Preferences).
- Select the “Addons” tab.
- Click “Install from File…” and select the downloaded zip file.
- Click the checkbox on the left to enable the add-on.
- Click “Save User Settings” to make sure the addon is enabled when you restart Blender.
- Set the parameters to fit your GPU system and paths.
- Open the new nodes editor, and press N to open the addon panel.
- Start generating contents :)

---

## :radio_button: Presets, Templates and Snippets

The addon offers 2 types of presets, full nodetrees and node groups. When the user saves a preet, it is automatically kept in specific folders. This allows, among other things, to share your “workflows” or nodetrees with other users. Here is the list of presets provided in this addon and their usage:

- **Basic setups**
  - Simple text-2-image
  - Advanced text-2-image
  - Simple image-2-image
  - Advanced image-2-image
- **Advanced setups**
  - LoRas Merging
  - VAEs Merging
  - Complex text-2-image
  - Complex image-2-image
- **Animation setups**
  - Basic images Sequence
  - Advanced images sequence
- **Film making setups**
  - VFX movie (Inpaint)

---

## :radio_button: Learning from users, training from experience

Objectives: Collecting user data and processing it locally allows you to create personalized artistic and technical models, ready to be used in a new nodetree.
- Many options: Structural, Lineal, Hierachical...
- Json files storage path


<table>
<tr>
<th align="center", width="100%">Data Types</th>
</tr>
</table>

<ul>
      <li><b>Actions History</b>
        <ul>
          <li>What is the last action done by a specific user?</li>
          <li>What is the most repeating actions?</li>
        </ul>
      </li>
      <li><b>Space Orbits</b>
        <ul>
          <li>What is the mid distance from the object origin in edit mode?</li>
          <li>What is the mid distance of action from the world origin?</li>
        </ul>
      </li>
      <li><b>Time Sequences</b>
        <ul>
          <li>What is the mid time between same actions?</li>
          <li>What is the time between same files edition?</li>
        </ul>
  </li>
      <li><b>User Types</b>
        <ul>
          <li>What is the skills level of a specific user?</li>
          <li>What is the most needed skill by user type</li>
        </ul>
      </li>
       <li><b>user Project Types</b>
        <ul>
          <li>What is the project types? Architecture, Industrial Design, etc...</li>
          <li>What is graphical type associated with the project? Realistic scene, cartoon, etc...</li>
        </ul>
      </li>
</ul>

---

## :radio_button: LLM Structure

The addon has 3 modes: Analyse/Prepare/Write, external file from session start.

- ANALYSE: write an external file
- PREPARE: images data
- WRITE: .ckpt/tensors

```diff
- NOTE: ...
```


<table>
<tr>
<th align="center", width="880">Data Processing</th>
</tr>
</table>

<ul>
      <li><b>Real-time Support</b>
        <ul>
          <li>Suggest a serie of optional processes and combos</li>
          <li>Suggest a serie of optional Shortcuts</li>
          <li>Suggest a serie of optional parametric objects</li>
          <li>Suggest a serie of optional Texturing processes</li>
        </ul>
      </li>
      <li><b>Real-time Auto-Correct</b>
        <ul>
          <li>Show errors based on 3 main error types*</li>
        </ul>
      </li>
</ul>

<table>
<tr>
<th align="center", width="880">Data Backend</th>
</tr>
</table>

<ul>
      <li><b>Local Files</b>
        <ul>
          <li>Write data as text file (txt, Json, Xml)</li>
          <li>Write data as new file (.bai) aka csv alternate</li>
        </ul>
      </li>
  <li><b>Temporary Files</b>
        <ul>
          <li>Realize 3 reality states A-X-B (data morphing)</li>
          <li>Compare 2 states A/B</li>
        </ul>
      </li>
</ul>

---

## :radio_button: Infos

* Author: **Uriel Deveaud** - [Kore Teknology](https://github.com/KoreTeknology) 
* License: This project is released under the GPL License.
* This work is dedicated to all Blender users around the world ;)

[^1]: **Blender** is the free and open source 3D creation suite. It supports the entirety of the 3D pipeline—modeling, rigging, animation, simulation, rendering, compositing and motion tracking, even video editing and game creation. Please, visit the [Blender Official Website](https://www.blender.org/).

[^2]: Large language models (LLM) are very large deep learning models that are pre-trained on vast amounts of data. The underlying transformer is a set of neural networks that consist of an encoder and a decoder with self-attention capabilities.

[^3]: Checkpoints are snapshots of your working model during the training process and stores it in a non-volatile memory. In machine learning and deep learning experiments, they are essentially the things which one uses to save the current state of the model so that one can pick up from where they left.

[^4]: LoRA (Low Rank Adaptation) is a new technique for fine-tuning deep learning models that works by reducing the number of trainable parameters and enables efficient task switching.
