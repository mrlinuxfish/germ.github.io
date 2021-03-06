---
nav_order: 5
description:  Ginny Quickstart
layout: post
title: Ginny and ASETNIOP
---

# Unboxing Ginny
Thanks for buying one of these little guys, it's a little wonky but I'm sure you'll have some fun with it!

If you bought a Ready, plug in your cables. If you're building your own use _very light_ switches, I recommend swapping out springs to around 20gf or less! Hit the reference diagrams and Gergo Build guide if you got a kit. Trust in your flux!


# Modes
This keyboard uses a modified version of the [Asetniop](http://asetniop.com/layouts/) engine. This keyboard is powered by the onboard steno engine of Georgi! As such there is a ton of overlap :)

# Languages

In addition to having a chord -> character keymap, Asetniop also has chords for various common words. For example if you stroke SETO your keyboard will emit "good ". There's a whole ton of these [listen on the Asetniop website](http://asetniop.com/combinations/) and will boost your typing speed! However these are language dependent, you can configure the language used in keymaps/default/keymap.c and editing the #include for your language.

As of right now the following languages are supported: English, en-dvorak, en-colemak, Danish, Dutch, Finnish, French, German, Hungarian, Italian, Norwegian, Polishh, Portuguese, Romanian, Spanish, Swedish, Turkish. 

# Layout
I'm not going to cover how to use Asetniop here, instead [use the online trainer to learn the map](http://asetniop.com/try/tablet/), and play [this wonderful game for a bit](https://github.com/Kyrremann/FreshKeebInLA). After that hit keybr and get grinding until your muscle memory takes over!

There are 4 layers on this board. If you're ever stuck, *just press all the keys twice!*

### Base (Default)
This is where all of your normal typing will happen. Letters, spaces, shifts, etc. This will be customized to your language! As well there are 9 "quick fire" binds that you can configure in your keymap.c

### Numbers (ATNP)
Press ATNP (Devil horns) to switch to numeric/symbol input mode. This is the same as on the Asetniop site and is language agnostic

### Commands (ESIO)
Press ESIO to switch to your command layer, this has Control, Alt, Meta, Function Keys, etc. Refer to gen/aset/cmd-keymap.c

### User (ASETNIOP)
Press ASETNIOP to switch to your user layer, these are configured directly in your keymap.c. Put any kind of text macros, frequent shortcuts, ~~passwords~~, in this layout.

### Command Mode (ETNI)

Due to the size of the board, key combos can be a pain if there is a conflict. What do you do when the key you're trying to chord overlaps with another that you need? Enter Command mode. Command mode buffers all of the keys that are pressed while it's active; once you exit command mode the keys are all pressed down, and then released in one go. So inserting say 'Ctrl+Shift+S' could be done in the following way 'Command Mode/Ctrl/Shift/S/Command Mode'.

Note: There are a good number of alternative binds for modifiers and you can always add definitions to your firmware! If you find a bind that you're using frequently, don't just whack it in over and over again in command mode, add it to your keyboard!
