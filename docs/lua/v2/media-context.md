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

You can create a media context in lua via a url.

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

|                    | YAB  | WXV Core |
| ------------------ | :--: | :------: |
| media_context      | None | Full 1   |
| audio/video key    | None | Full 1   |
| lua media_context  | None | Full 1   |
| paused             | None | Full 1   |
| duration           | None | Full 1   |
| current_time       | None | Full 1   |
| volume             | None | Full 1   |
| playback_rate      | None | Full 1   |
| play               | None | Full 1   |
| pause              | None | Full 1   |
| on_playback_change | None | Full 1   |
