# Blender Generative AI Addon
A research script based on *Artificial Intelligence* for Blender, this is a multi-steps development project, with **LLM Local System** focus in mind. This script/addon is intended to serve the purpose to *generate unique images and video sequences*, within **Blender Nodes Editor** and based on Public Checkpoint Models OR/AND **Private custom Models and LoRas**. 

<img src="https://img.shields.io/badge/Blender-3.6.5-green" /> <img src="https://img.shields.io/badge/Python-3.7-blue" /> <img src="https://img.shields.io/badge/Addon-0.8.1a-yellow" /> <img src="https://img.shields.io/badge/CAN-X.1567D-red" />

---

## Features in progress

- Image API generation (using a new Node Editor window)
- ComfyUI Server connection for local sessions
- Single image and Images sequence rendering/storing
- Custom checkpoints, LoRas, VAE loading
- Script-2-Prompt GPT-2 based custom node

---

## Saving user data as Data collection

- Many options: Structural, Lineal, Hierachical...
- Internal data, External files (new extension type?)

---

## User Interface Access

- New editor window
- Intelligent Nodes panel (N)

---

<table>
<tr>
<th align="center", width="880">Data Types</th>
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

## Step 1

The addon has 3 modes: Analyse/Support/Both

- ANALYSE: write an external file
- SUPPORT: suggest and fix
- INTERACTIVE: both

The addon write an external file from session start, including data from:

- Every time the user is duplicating vertex without moving them
- Every time an object has face´s oriention in wrong direction (inside)
- Every time an object has a scale different then 1

```diff
- NOTE: ...
```

---

## Infos

* Author: **Uriel Deveaud** - [Kore Teknology](https://github.com/KoreTeknology) 

<img src="https://img.shields.io/badge/CG Art-1995-red" /> <img src="https://img.shields.io/badge/3D Blender-2002-red" /> <img src="https://img.shields.io/badge/Python Dev-2005-red" /> <img src="https://img.shields.io/badge/3D Trainer-2008-red" /> <img src="https://img.shields.io/badge/Coding Trainer-2010-red" /> <img src="https://img.shields.io/badge/GE-2015-darkorange" /> <img src="https://img.shields.io/badge/VR-2017-darkorange" /> <img src="https://img.shields.io/badge/AI-2020-darkorange" />

* License: This project is released under the GPL License.
* This work is dedicated to all Blender users ;)
