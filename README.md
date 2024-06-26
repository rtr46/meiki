# meiki
meiki lets you look up words with a gamepad while playing Japanese video games (on windows)

meiki is like [JL](https://github.com/rampaa/JL) or ClipboardReader+Yomichan, but for gamepads! It uses [jpdb.io](jpdb.io) for parsing + translating

meiki is probably perfect for devices like the steam deck, asus rog ally or lenovo legion go

## download
[Click here to download](https://github.com/rtr46/meiki/releases)

## features
- clipboard monitoring for japanese text and automatically parse + translate via jpdb.io
- popup displaying tokens, readings, translations and frequencies of sentences (default button RT)
- adding furigana (enabled by default)
- popup scrolling via gamepad (right analogue stick)
- game/emulator pausing while the popup is being displayed (disabled by default, default simulated pause key F4)
- sentence logging
- marking sentences and words as known (default button disabled)
- marking sentences as unknown (default button disabled)
- saving screenshots (default button disabled)

![screenshot of meiki no popup](https://github.com/rtr46/meiki/assets/171138461/f5eace9d-262a-41ce-ba79-90cfdaed3a4e)

https://github.com/rtr46/meiki/assets/171138461/2eae7ee2-8099-495d-adce-d8d74cdb2a47

## getting started
- first you need a [jpdb.io](https://www.jpdb.io) account and and api key. the api key is available to all jpdb.io accounts and can be found at the bottom of the settings page
- you need a game that meiki can help you with
- you need to texthook the game with something like [textractor](https://github.com/Artikash/Textractor) or [agent](https://github.com/0xDC00/agent/releases)
- those texthookers have to be configured to copy the text of the game into the clipboard
- meiki monitors the clipboard for japanese text and parses+translates it via jpdb
- meiki can display a popup which shows all tokens, words, readings, meaning and frequencies of the text line (default button RT)

## tips
- the default button for showing the meiki popup is RT
- depending on the game you are playing the default buttons may be not suited. you can change the defaults in the meiki.config.ini file
- maybe you want to keep separate config files for separate games
- you can enable features like marking sentences as known or unknown via gamepad button press in the config
- you can also enable a function to pause the game/emulator while showing the popup. this can be useful if a game doesn't have "push to continue"
  - this feature works in a way, where meiki simulates a (configurable) keyboard press to pause and unpause the game
- the main feature is the popup that can be controlled by RT, but you can also just move the popup to a second monitor and keep it there

## known bugs
- !!! meiki uses the edge browser to display the overlay, but in order to do that, it kills all other msedge.exe processes !!!
- only tested with xbox gamepads... there are probably problems with other controllers
- the screenshot function only screenshots a fixed 1920x1080 size. it should work as long as your game runs on your primary monitor which hopefully is FHD. otherwise it wouldn't really work well
- there may be some funkiness when running multiple monitors
- there may be some funkiness with the popup. try to maximize it and then press RT (or whatever you set the popup button to) two or three times slowly to make sure it works
