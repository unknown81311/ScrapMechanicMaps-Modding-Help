---
sidebar_position: 2
title: File Path References
hide_title: true
sidebar-label: 'File Path References'
---

### File Path References

This page lists available file path references and which folders they represent.

```
"$MOD_DATA"
```
Represents the root directory of the current mod. <br></br>

:::info note
This path can only be used from within a workshop mod. <br></br>
Some functions do not work with this (for example <code>guiInterface:setImage()</code> ). <br></br>
It is recommended to use <code>$CONTENT_DATA</code> instead.
:::

<br></br>

```
"$CONTENT_DATA"
```
If used in a mod, this represents the root directory of the current mod. <br></br>
If used in the game files, this represents the <code>Challenges/MasterMechanicTrials</code> <br></br>
directory in the game files.

<br></br>

```
"$CONTENT_UUID"
```
Represents the root directory of the content with the given UUID. <br></br>
To use this, replace <code>UUID</code> with the UUID of a mod or blueprint. <br></br>
The UUID can be found in the content's <code>description.json</code> file <br></br>
in the <code>localId</code> entry. <br></br>

<br></br>

```
"$GAME_DATA"
```
Represents the <code>Data</code> directory in the game files. <br></br>

<br></br>

```
"$SURVIVAL_DATA"
```
Represents the <code>Survival</code> directory in the game files. <br></br>

<br></br>

```
"$CHALLENGE_DATA"
```
Represents the <code>ChallengeData</code> directory in the game files. <br></br>

<br></br>

```
"$CACHE_DATA"
```
Represents the <code>Cache</code> directory in the game files. <br></br>

<br></br>

```
"$TEMP_DATA"
```
Represents the <code>Temp</code> folder in the <code>%LocalAppData%/Axolot Games/Scrap Mechanic/</code> directory. <br></br>
This folder normally only exists while the game is running, though it only gets deleted if <br></br>
the game is closed using the <code>Exit Game</code> button in the main menu. <br></br>
It is <strong>not</strong> deleted if the game is closed in any other way. <br></br>
