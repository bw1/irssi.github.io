---
layout: page
title: beep
permalink: documentation/beep/
---
# faq-beep
![line](line.svg)

## shell
### bash
  *  man:

```
bell-style (audible)
	  Controls what happens when readline wants to ring  the  terminal
	  bell.  If set to none, readline never rings the bell.  If set to
	  visible, readline uses a visible bell if one is  available.   If
	  set to audible, readline attempts to ring the terminal's bell.
```

## terminal multiplexer
### screen
  *  man:

```
C-a C-g     (vbell)       Toggles screen's visual bell mode.

vbell [on|off]

Sets the visual bell setting for this window.  Omitting  the  parameter
toggles  the  setting.  If vbell is switched on, but your terminal does
not support a visual bell, a `vbell-message' is displayed in the status
line  when the bell character (^G) is received.  Visual bell support of
a terminal is defined by the termcap variable `vb' (terminfo: 'flash').
Per default, vbell is off, thus the audible bell  is  used.   See  also
`bell_msg'.
```

### tmux
  *  man:

```
bell-action [any | none | current | other]
		Set action on window bell.  any means a bell in any win-
		dow linked to a session causes a bell in the current win-
		dow of that session, none means all bells are ignored,
		current means only bells in windows other than the cur-
		rent window are ignored and other means bells in the cur-
		rent window are ignored but not those in other windows.

bell-on-alert [on | off]
		If on, ring the terminal bell when an alert occurs.

visual-bell [on | off]
		If this option is on, a message is shown on a bell
		instead of it being passed through to the terminal (which
		normally makes a sound).  Also see the bell-action
		option.

```

## terminal emulator

### putty
  *  [Config](https://the.earth.li/~sgtatham/putty/0.70/htmldoc/Chapter4.html#config-bell)

### xterm
![menu](xterm-menus.png)
  *  [xterm](https://invisible-island.net/xterm/xterm.html)

### lxterminal
![menu](lxterminal.png)

### konsole
![menu](konsole.png)

## kernel

```
# modprobe pcspkr
```

### alsa
![alsa](alsamixer.png)

## see also
  *  [Visual-Bell](http://www.faqs.org/docs/Linux-mini/Visual-Bell.html)
