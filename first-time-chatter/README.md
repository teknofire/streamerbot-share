# First time chatter

This is a quick set of actions that can be used to trigger various actions in streamer-bot based on a users chatting for the first time ever.

This is really just an example of how it can be done and would need to be highly customized to the streamers specific OBS setup.

## Setup 

Download the `first-time-chatter.txt` and import into Streamer.Bot

After installing the actions there are a few things you'll need to setup in OBS to handle the actions.

1. A GDI Text overlay that will be used to display a message on stream. You will need to modify the `First time chat display` -> `OBS GDI Text` sub-action in order to specify the scene and source for this in Streamerbot.
2. Add any additional overlays that should be shown and/or any sounds that you would like to play. There are example sub-actions already for this and they can be modified or removed to suit your setup.
3. Make sure to keep a 1 second delay at the end if you have any animations that happen on show/hide of layers in OBS.

## Actions

### Raid Suspend FTC

This action will suspend all the actions in the `First Time Chat Actions` group after a raid happens for 1 minute. This way when a large raid happens all the new users we won't get a flood of triggers for this action.

To extend this modify the delay - _note that the delay is in milliseconds (`MS`)_

### First time chat trigger

This is used to detect when a user chats for the first time in twitch chat. Nothing needs to be modified here. When a new chatter is found it will execute the `First time chat display` action.

### First time chat display

This is an example of what can be done.

1. Will modify the content of a GDI Text overlay with some text with the users name and a message.
2. Display some other overlays like a icon or personal image at the same time for 

