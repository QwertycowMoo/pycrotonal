# A Keyboard Synthesizer called Pycrotonal 
Kevin Zhou kjzhou2 | Moderator Kyle Liu kuihual2

### Project Purpose
My project will create a customizable microtonal synthesizer playable by the keyboard on your machine. This should be fully functional instrument that anyone can run on any machine.

### Motivation
As a CS+Music student, I would like to do a project with the recent things I've learned in my electronic music. We've learned a lot about audio synthesis and audio buffers, so I wanted to do a project with synthesizers within Python, since that is the language that I'm most comfortable with. I noticed that our CS+Music curriculum only touches on microtonal music, so I wanted to explore this aspect of music more. As well, I've been interested in starting to make my own instruments electronically, and this would be a step in that direction.

### Tech, Tools, and Style
Programming Language: Python 3.9+
Libraries:`PYO`, `Pynput` 
GUI: `Tkinter` 
Style: PEP8 style and using `pylint` to enforce
Testing: `unittest` package 
Target Audience: Musicians

### Scope of the Project
* Limitations include my ability to work with a keyboard and make a musically viable interface for a microtonal keyboard

### GUI
See File in Repo 

### Timeline

Week 1:
- Set up basic GUI with all knobs for audio effects
- Create synthesizer and connection to audio output
- Implement FM, Reverb, and Distortion Effects
- Should be able to play manually with tests and code injection

Week 2:
- Create mapping function for different Equal Divisions of the Octave
- Listen for keyboard input (and MIDI if implementing)
- Show fundemental frequency that synth is supposed to play 
- Change mapping with command line

Week 3:
- Connect the keyboard input with the synthesizer
- Show the key pressed and frequency played on the GUI
- Show a visual representation of the EDO mapping on the GUI
- Have polyphony for the instrument
- Have an ADSR envelope for each note played

## Rubrics
### Week 1
| Requirements      | Points |Notes                                                                                                                                                                                                                                                    |
|-------------------|--------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Week 1 Functional |        |                                                                                                                                                                                                                                                          |
| Layout Design     | 1      | Create a mock of the GUI and show what is adjustable                                                                                                                                                                                                     |
| View              | 4      | Create a functional GUI with (+1)Knob for FM frequency and Knob for FM amplitude (+1)Buttons with basic scale to test audio output (+1) Input for Equal Division of the Octave (Implemeted Later)  (+1 )Reverb wetness and Distortion amount (+1) Ability to pick waveform All GUI elements should show output in the console when changed|
| Audio Output      | 3      | Audio is able to played from PYO to the computer speakers                                                                                                                                                                                                |
| Waveform Choice   | 2      | Change the waveform based on GUI choice                                                                                                                                                                                                                  |
| FM modulation   | 3      | Frequency Modulation Amplitude (+1), Modulation Index (+1) correctly applied (+1) to original waveform|
|Audio Effects | 2 |Reverb(+1), and Distortion(+1) applied correctly to base waveform      |
| Testing/Linting   |        |                                                                                                                                                                                                                                                          |
| Pylint            | 2      | If pylint score is above 80/100                                                                                                                                                                                                                          |
| Unit Tests        | 5      | +0.5 per unit test                                                                                                                                                                                                                                       |
| Manual Tests      | 3      | Describe user flow and show GUI screenshots screenshots                                                                                                                                                                                                              |
| Bonus             |        |                                                                                                                                                                                                                                                          |
| Waveform Image    | 1      | Show a realtime image of the current waveform being played                                                                                                                                                                                               |
## Week 2
| Requirements                   | Points | Notes                                                                                                                                                                                                                                                                                           |
|--------------------------------|--------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Week 2 Functional              |        |                                                                                                                                                                                                                                                                                                 |
| Keyboard Input                 | 4      | Use Pynput to listen for keyboard input |
| Microtonal EDO Keyboard Design | 3      | Have a design on how the keyboard will be split into different EDO Bonus(+1) for being able to support any number of EDO from 1 - 44                                                                                                                                                            |
| Create Adjustable EDO Keyboard | 3      | Implement the adjustable EDO keyboard using pynput. - When a key is pressed, the command line output should be the frequency of the fundemental |
|Baseline EDO keyboard implementation | 2 | Baseline is 10 EDO, 12 EDO, 24 EDO, and 44 EDO. Different EDO scales should map similarly to keys on the keyboard |
| Command line input             | 3      | Implement a CLI to change the EDO                                                                                                                                                                                                                                                               |
|                                |        |                                                                                                                                                                                                                                                                                                 |
| Testing/Linting                |        |                                                                                                                                                                                                                                                                                                 |
| Pylint                         | 2      | If pylint score is above 80/100                                                                                                                                                                                                                                                                 |
| Unit Tests                     | 8      | +0.5 per unit test                                                                                                                                                                                                                                                                              |
|                                |        |                                                                                                                                                                                                                                                                                                 |
| Bonus                          |        |                                                                                                                                                                                                                                                                                                 |
| MIDI Input                     | 2      | Be able to support MIDI messages as well from an actual keyboard                                                                                                                                                                                                                                |
### Week 3
| Requirements                   | Points | Notes                                                                                                                                                                                                                                    |
|--------------------------------|--------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Week 3 Functional              |        |                                                                                                                                                                                                                                          |
| Connection with Keyboard Input | 3      | Connect keyboard input to PYO synth                                                                                                                                                                                                      |
| Responsive Keyboard GUI        | 3      | Show the current mapping of what keyboard key plays what frequency. Preferable if there graphic instead of a list Not required but preferred if the actual regular 12 EDO is highlighted                                                 |
| Static Keyboard                | 2      | Show graphical mapping of Keyboard                                                                                                                                                                                                       |
| ADSR                           | 2      | Attack Decay Sustain Release for a specific note                                                                                                                                                                                         |
| Show Current Key Played        | 2      | Show the current key and frequency played                                                                                                                                                                                                |
| Polyphony                      | 3      | Allow multiple notes to be played at a time                                                                                                                                                                                              |
|                                |        |                                                                                                                                                                                                                                          |
|                                |        |                                                                                                                                                                                                                                          |
| Testing/Linting                |        |                                                                                                                                                                                                                                          |
| Pylint                         | 2      | If pylint score is above 80/100                                                                                                                                                                                                          |
| Unit Tests                     | 3      | +0.5 per unit test above previous week's                                                                                                                                                                                                 |
| Manual Test Plan               | 5      | Manual Test plan +5 if multiple pages detailing changing EDO and keyboard output -1 for each functionality implemented but not covered by manual test plan (Details of implementation will be fleshed out further as develop progresses) |
|                                |        |                                                                                                                                                                                                                                          |

Grading Template Links:
[Week 1](https://docs.google.com/spreadsheets/d/1tzTAX9tFxHbvWCDR5G_ZVpftYv6urMZ_IlgcIbvcQxM/edit?usp=sharing)

[Week 2](https://docs.google.com/spreadsheets/d/1vdt2SnkPDcYIfjoazAjfRPtcZJdISaCoGx9ybnzF_z0/edit?usp=sharing)

[Week 3](https://docs.google.com/spreadsheets/d/1B_bXreNge4Smk6w0DAA8bqfNxSQofaXvXi-DLhqPLJM/edit?usp=sharing)
