# private.xml in Karabiner

I have been using [Karabiner](https://github.com/JeongMinCha/karabiner-privatexml).
This application is priceless for Mac OS X User who want to map keys in keyboard.

Your private XML file is located at
```
/Users/$(whoami)/Library/Application\ Support/Karabiner/private.xml
```
$(whoami) means your user name.

## The simplest example
You may use Karabiner to map a key to another key, 
right? If you just want to do it, 
you should write your _private.xml_ file like this:
```
<item>
	<name>JIS_KANA to COMMAND_R</name>
	<identifier>private.jis_kana_to_command_r</identifier>
	<autogen>__KeyToKey__ KeyCode::JIS_KANA, KeyCode::COMMAND_R</autogen>
</item>
```
This code means mapping "JIS_KANA" to "COMMAND_R"

## The list of KeyCodes
If you want to see the list of KeyCodes, you can visit [here](https://github.com/tekezo/Karabiner/blob/master/src/bridge/generator/keycode/data/KeyCode.data).
You can use ```Command + F``` or ```Control + F``` to find something you want.
