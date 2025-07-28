---
title: Media Context
description: Lua V2 Media context API
parent: V2 API
---
# Lua v2 Media context API

This API allows you to control media related elements ([audio](../../htmlpp/audio.md) & [video](../../htmlpp/video.md)).

## HTML++

The [audio](../../htmlpp/audio.md) and [video](../../htmlpp/video.md) elements have an extra `media_context` key with a table.

```lua
audio.media_context.pause()
```

## Lua

You can create a media context in lua via a url, the url can only point to an audio file, video files will not work.

```lua
local ctx = media_context('https://.../audio.mp3')
```

## Media Context Table

Properties:

- paused - A boolean stating if the media element is paused (non editable)
- duration - A float in seconds of how long the media is (non editable)
- current_time: A float in seconds of the current moment being played
- volume - A number 0 to 1 defining 0% to 100% volume of the media
- muted - A boolean, separate from volume, that defines if audio should play
- playback_rate - A float between 0 and 4 that defines the speed of the media
- loop - A boolean that defines if the media should loop when it reaches the end

Functions:

- play() - Plays/Unpauses the media element
- pause() - Stops/Pauses the media element

Events:

- on_playback_change => callback(paused) - Fired when the user or lua pauses or unpauses the media, the current pause state is passed

## Support

|                    | YAB                    | WXV Core            |
| ------------------ | :--------------------: | :-----------------: |
| media_context      | <span none>None</span> | <span full>1</span> |
| audio/video key    | <span none>None</span> | <span full>1</span> |
| lua media_context  | <span none>None</span> | <span full>1</span> |
| paused             | <span none>None</span> | <span full>1</span> |
| duration           | <span none>None</span> | <span full>1</span> |
| current_time       | <span none>None</span> | <span full>1</span> |
| volume             | <span none>None</span> | <span full>1</span> |
| playback_rate      | <span none>None</span> | <span full>1</span> |
| play               | <span none>None</span> | <span full>1</span> |
| pause              | <span none>None</span> | <span full>1</span> |
| on_playback_change | <span none>None</span> | <span full>1</span> |
