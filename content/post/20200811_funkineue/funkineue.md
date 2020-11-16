+++
date = 2020-11-16T12:00:00-04:00
title = "funkineue"
writer = "Bob White"
draft = false
image = "funkineue.jpg"
showonlyimage = false
categories = ["birdhouse"]
keywords = ["key", "words"]
topics = ["topic 1"]
tags = ["cycling74", "jitter", "Ableton", "ISF", "vidvox"]
weight = 1
description = "ADSR-ISF test 01"
+++

| DATE | URL | DESCRIPTION |
| :--- | :--- | :--- |
| 20201116 | [Instagram](https://www.instagram.com/p/CHoJvRDnqDK/?utm_source=ig_web_copy_link) | |
| 20201116 | [Vimeo](https://vimeo.com/479936980) | |
| 20201116 | [github](https://github.com/lg3bass/20200811_funkineue) | git archive |



<!--more-->


## 20200811_funkineue

### HISTORY

- 20201116 Project published/archived.


### LINKS

- [Instagram](https://www.instagram.com/p/CHoJvRDnqDK/?utm_source=ig_web_copy_link)
- [YouTube](https://www.youtube.com/watch?v=VHcZMNqLWe4)
- [Vimeo](https://vimeo.com/479936980)


### description

Funkineue - First complete test of my M4L Step sequencer driving ISF visuals realtime in Live.  Seizure inducing I know.  Just testing the limits with the entire kitchen sink.

### FILES

	VIDEO:
	20200811_funkineue_01-trim.mp4
	
	ABLETON PROJECT:
	20200811_funkineue_09.als
	
	M4L DEVICES:
	/M4L/ADSR-ISF_1.368.amxd
	/M4L/ADSR-sound_v0.18.amxd
	/M4L/ADSR-world-out_0.1.amxd
	/M4L/ADSR-automation_v0.03.amxd
	
	M4L SETTINGS:
	/M4L/json/9_track4-8n.json
	/M4L/json/9_track3-8n.json
	/M4L/json/9_track2-8n.json
	/M4L/json/9_track1-8n.json
	
	ISF SHADERS:
	/ISF-files/funkineue03.fs
	
	FINALE MUSIC:
	/Finale/032011_funkineue_score.musx
	/Finale/032011_funkineue_score_FINAL.pdf



### Enhancements

	[ ]	PITA to load the json every time.  Need to have this load automatically
	[ ] Also sucks to have to load a shader and click qmetro and mode.  This operation should be consolidated.
	[ ]	When you playback cold in arangement view the automation doesn't trigger till values change. I have to let it play through to the next scene to see the correct automation.
	[ ] Separate the ADSR grid from the ISF.  This way you can use different rendering (ISF, JXS, VMM).
	[ ] Master track viewer should default to 720x405 automatically.  Activating this should be a one button process.  However if I have to move this to a second screen maybe I do need 2 buttons.


### Bugs

	[ ]	adsr-gridwindow too big,  Consolidate all the save/load buttons.
	[ ] shader sometimes doesn't display when you mess with the device(on|off|fileManagement)
	[ ] When you change the tempo in girdwindow it messes with the sample tempo. 
		- Changed the tempo to 160 in gridwindow.  Sample shows as 160 in edit view on track.  Must be connected somehow.
	[ ] Noticed that if you run a song in arrangement view a long time, over and over, CPU resources get consumed.  Especially if you are doing a lot of automation work. Not sure why this is happening but eventually it causes the audio to stutter.  Simply closing the project and reloading frees up CPU resources
	[ ] After "load" button background doesn't match grid width.
	[ ]	I think the "ADSR-ISF_1.368 > adsrScene" automation is messing this up. Perhaps scene 1 is trying to load

