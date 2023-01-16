![color_picker](https://user-images.githubusercontent.com/76603653/212703874-820b0238-e079-4b33-b764-39022709bc11.png)


# Color Picker for TouchPortal
- [Color Picker](#On-Screen-Color-Picker)
  - [Description](#description) 
  - [Features](#Features)
    - [Actions](#actions)
        - [Get Color from Mouse](#tp.plugin.color_picker.mainactions)
        - [Get Position from (X,Y)](#tp.plugin.color_picker.mainactions)
        - [Save / Load Colors](#tp.plugin.color_picker.mainactions)
        - [Copy Color to Clipboard](#tp.plugin.color_picker.mainactions)
        - [Change Name Style](#tp.plugin.color_picker.mainactions)
    - [States](#states)
        - [Color Picker | Main States](#tp.plugin.color_picker.mainstates)
        - [Color Picker | Current](#tp.plugin.color_picker.currentstates)
        - [Color Picker | Color 1-10](#tp.plugin.color_picker.color1states)
  - [Bugs and Support](#bugs-and-suggestion)
  
# Description
 **Get Color from ANYTHING on your monitors and utilize the color code for it.**
 <br>Simply hover your mouse over it and click the action inside of Touch Portal and the states will be populated for that button

# Features
- Copy colors to clipboard or use in other places (RGB / HEX / INT / NAME)
- Quick and easy access to any color you can see on your monitors.
- Change color sources in OBS Studio based on mouse input with OBSint

## Actions

<details id='tp.plugin.color_picker.mainactions'><summary><b>Category:</b> Color Picker / Eye Dropper Tool <small><ins>(Click to expand)</ins></small></summary>


| Action Name | Description | Format | Data | On Hold | 
| --- | --- | --- | --- | --- |
| Get Color From Mouse | Get Color from Mouse | Get Color From Mouse and save to [1]  |  1. Type: choice<Br> Default: 0<br> Possible choices: ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9', '10'] |  No |
| Save/Load Colors | Save / Load Colors to or from config | [1] colors to OR from file to [2] | 1. Type: choice<br>Default: Save <br>Possible choices: ['Save', 'Load'] 2. Type: file   Default: Default  |  No |
| Get Color from (X, Y) | Get Color from (X, Y) location | Get Color From Position X:[1] Y:[2] Value Name: [3] | 1. Type: number Default: 0 <br>Min Value: -50000 / Max Value: 50000 <br>2. Type: number<br>Default: 0 <br>3. Select Custom Name  | No  |
| Copy Color to Clipboard | Copy Color Code / Name to Clipboard | Copy [2] to clipboard from Button [1] | 1. Type: choice   Default: Current Possible choices: ['Current', '1', '2', '3', '4', '5', '6', '7', '8', '9', '10'] <br> 2. Type: choice <br>Default: HEX Possible choices: ['HEX', 'RGB', 'INT', 'NAME', 'OBS']  |  No |
| Change Name Style | Change Naming Style for Color Names | Change the naming style to:[1] | 1. Type: choice <br> Default: Basic Possible choices: ['Basic', 'Full', 'Best of']  |  No |
</details>


## States
<details id='tp.plugin.color_picker.mainstates'><summary><b>Category:</b> Color Picker / Eye Dropper Tool <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.current_text_name_style | Color Picker: Text Name Style |  |   |
| .state.last_mouse_x | Color Picker: Last Mouse Location - X |  |   |
| .state.last_mouse_y | Color Picker: Last Mouse Location - Y |  |   |
| .state.config_loaded | Color Picker: Current Config Loaded |  |   |
</details>

<details id='tp.plugin.color_picker.currentstates'><summary><b>Category:</b> Color Picker | Current <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_current | Color Picker: COLORICON |  |   |
| .state.text_current | Color Picker: TEXT |  |   |
| .state.hex_color_current | Color Picker: HEX |  |   |
| .state.rgb_color_current | Color Picker: RGB |  |   |
| .state.int_color_current | Color Picker: INT  |  |   |
| .state.obs_color_current | Color Picker: OBS |  |   |
</details>

<details id='tp.plugin.color_picker.color1states'><summary><b>Category:</b> Color Picker | Color 1 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button1 | Color Picker: COLORICON [B1] |  |   |
| .state.text_color_button1 | Color Picker: TEXT  |  |   |
| .state.hex_color_button1 | Color Picker: HEX [B1]  |  |   |
| .state.rgb_color_button1 | Color Picker: RGB [B1] |  |   |
| .state.int_color_button1 | Color Picker: INT [B1] |  |   |
| .state.obs_color_button1 | Color Picker: OBS [B1] |  |   |
</details>

<details id='tp.plugin.color_picker.color2states'><summary><b>Category:</b> Color Picker | Color 2 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button2 | Color Picker: COLORICON [B2] |  |   |
| .state.text_color_button2 | Color Picker: TEXT [B2]  |  |   |
| .state.hex_color_button2 | Color Picker: HEX [B2]  |  |   |
| .state.rgb_color_button2 | Color Picker: RGB [B2] |  |   |
| .state.int_color_button2 | Color Picker: INT [B2] |  |   |
| .state.obs_color_button2 | Color Picker: OBS [B2] |  |   |
</details>

<details id='tp.plugin.color_picker.color3states'><summary><b>Category:</b> Color Picker | Color 3 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button3 | Color Picker: COLORICON [B3] |  |   |
| .state.text_color_button3 | Color Picker: TEXT [B3]  |  |   |
| .state.hex_color_button3 | Color Picker: HEX [B3]  |  |   |
| .state.rgb_color_button3 | Color Picker: RGB [B3] |  |   |
| .state.int_color_button3 | Color Picker: INT [B3] |  |   |
| .state.obs_color_button3 | Color Picker: OBS [B3] |  |   |
</details>

<details id='tp.plugin.color_picker.color4states'><summary><b>Category:</b> Color Picker | Color 4 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button4 | Color Picker: COLORICON [B4] |  |   |
| .state.text_color_button4 | Color Picker: TEXT [B4]  |  |   |
| .state.hex_color_button4 | Color Picker: HEX [B4]  |  |   |
| .state.rgb_color_button4 | Color Picker: RGB [B4] |  |   |
| .state.int_color_button4 | Color Picker: INT [B4] |  |   |
| .state.obs_color_button4 | Color Picker: OBS [B4] |  |   |
</details>

<details id='tp.plugin.color_picker.color5states'><summary><b>Category:</b> Color Picker | Color 5 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button5 | Color Picker: COLORICON [B5] |  |   |
| .state.text_color_button5 | Color Picker: TEXT [B5]  |  |   |
| .state.hex_color_button5 | Color Picker: HEX [B5]  |  |   |
| .state.rgb_color_button5 | Color Picker: RGB [B5] |  |   |
| .state.int_color_button5 | Color Picker: INT [B5] |  |   |
| .state.obs_color_button5 | Color Picker: OBS [B5] |  |   |
</details>

<details id='tp.plugin.color_picker.color6states'><summary><b>Category:</b> Color Picker | Color 6 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button6 | Color Picker: COLORICON [B6] |  |   |
| .state.text_color_button6 | Color Picker: TEXT [B6]  |  |   |
| .state.hex_color_button6 | Color Picker: HEX [B6]  |  |   |
| .state.rgb_color_button6 | Color Picker: RGB [B6] |  |   |
| .state.int_color_button6 | Color Picker: INT [B6] |  |   |
| .state.obs_color_button6 | Color Picker: OBS [B6] |  |   |
</details>

<details id='tp.plugin.color_picker.color7states'><summary><b>Category:</b> Color Picker | Color 7 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button7 | Color Picker: COLORICON [B7] |  |   |
| .state.text_color_button7 | Color Picker: TEXT [B7]  |  |   |
| .state.hex_color_button7 | Color Picker: HEX [B7]  |  |   |
| .state.rgb_color_button7 | Color Picker: RGB [B7] |  |   |
| .state.int_color_button7 | Color Picker: INT [B7] |  |   |
| .state.obs_color_button7 | Color Picker: OBS [B7] |  |   |
</details>

<details id='tp.plugin.color_picker.color8states'><summary><b>Category:</b> Color Picker | Color 8 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button8 | Color Picker: COLORICON [B8] |  |   |
| .state.text_color_button8 | Color Picker: TEXT [B8]  |  |   |
| .state.hex_color_button8 | Color Picker: HEX [B8]  |  |   |
| .state.rgb_color_button8 | Color Picker: RGB [B8] |  |   |
| .state.int_color_button8 | Color Picker: INT [B8] |  |   |
| .state.obs_color_button8 | Color Picker: OBS [B8] |  |   |
</details>

<details id='tp.plugin.color_picker.color9states'><summary><b>Category:</b> Color Picker | Color 9 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button9 | Color Picker: COLORICON [B9] |  |   |
| .state.text_color_button9 | Color Picker: TEXT [B9]  |  |   |
| .state.hex_color_button9 | Color Picker: HEX [B9]  |  |   |
| .state.rgb_color_button9 | Color Picker: RGB [B9] |  |   |
| .state.int_color_button9 | Color Picker: INT [B9] |  |   |
| .state.obs_color_button9 | Color Picker: OBS [B9] |  |   |
</details>

<details id='tp.plugin.color_picker.color10states'><summary><b>Category:</b> Color Picker | Color 10 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.icon_color_button10 | Color Picker: COLORICON [B10] |  |   |
| .state.text_color_button10 | Color Picker: TEXT [B10]  |  |   |
| .state.hex_color_button10 | Color Picker: HEX [B10]  |  |   |
| .state.rgb_color_button10 | Color Picker: RGB [B10] |  |   |
| .state.int_color_button10 | Color Picker: INT [B10] |  |   |
| .state.obs_color_button10 | Color Picker: OBS [B10] |  |   |
</details>

<br>

# Bugs and Suggestion
Open an issue on github or join offical [TouchPortal Discord](https://discord.gg/MgxQb8r) for support.

