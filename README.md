# Blender Generative AI Addon
A research script based on *Artificial Intelligence* for Blender, this is a multi-steps development project, with **LLM Local System** focus in mind. This script/addon is intended to serve the purpose to *generate unique images and video sequences*, within **Blender Nodes Editor** and based on Public Checkpoint Models OR/AND **Private custom Models and LoRas**. It includes an integrated learning machine process as well as a model exporter script.

<img src="https://img.shields.io/badge/Blender-3.6.5/4-green" /> <img src="https://img.shields.io/badge/Python-3.8-blue" /> <img src="https://img.shields.io/badge/Addon-1.3.5a-yellow" /> <img src="https://img.shields.io/badge/CAN-X.1567D-red" /> <img src="https://img.shields.io/badge/BL-GAIA-orange" />



## Acknowledgments

```py
NOTE: This project is derived from the K.Sharon & Yorha4D work, called "ComfyUI-BlenderAI-node".
Link: https://github.com/AIGODLIKE/ComfyUI-BlenderAI-node
Release: 1.2.9 - Licensed under GNU General Public License v3.0
```

*"I decided to re-write this addon for several reasons. The first was that the original translation was in Chinese and that some errors appeared due to non-standard characters. The second was that the interface deserved to be redesigned to integrate into my workflow. The third was that I wanted to add functions for animation and the video sequencer. And the last because I couldn't contact the developers of the project and offer my collaboration."*

<img alt="Win 11" src="/media/win11_logo.png" width="90">


---

## Features & Updates

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

### Todo List: [See next steps development phases](TODO_LIST.md) *Updated: 26/10/2023*



<img alt="preview_v135" src="/media/addon_preview_v125.png">

---

## ComfyUI Installation and Modules

After installing **ComfyUI** with your prefered plateform (i am using **Stability Matrix**), make sure you install the additional modules. To install these modules, open a CMD window in the \ComfyUI\custom_nodes folder. And "git clone" each one of them. By adding the link after "git clone".

- ComfyUi-Manager
- [ComfyUI-Impact](https://github.com/ltdrdata/ComfyUI-Impact-Pack)
- [ComfyUI-Inspire](https://github.com/ltdrdata/ComfyUI-Inspire-Pack)
- WAS Nodes Suite
- Animate Diff
- Prompt-Expansion
- [Derfuu-ComfyUI_ModdedNodes](https://github.com/Derfuu/Derfuu_ComfyUI_ModdedNodes)


## Learning from users, saving data as collection?

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

## LLM Structure

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

## Infos

* Author: **Uriel Deveaud** - [Kore Teknology](https://github.com/KoreTeknology) 

<img src="https://img.shields.io/badge/CG Art-red" /> <img src="https://img.shields.io/badge/3D Blender-red" /> <img src="https://img.shields.io/badge/Python Dev-red" /> <img src="https://img.shields.io/badge/GAME Engine-darkorange" /> <img src="https://img.shields.io/badge/VR Environmental-darkorange" /> <img src="https://img.shields.io/badge/AI Training-darkorange" />

* License: This project is released under the GPL License.
* This work is dedicated to all Blender users ;)
