Hello!, welcome to the wais-hudv4 readme file where you can find answers to your questions or use some code.

# HUD Show/Hide Trigger

- Such an event is available in the existing event client. It accepts True or False arguments

Example:
```
    TriggerEvent('wais:hudHide', true or false) Only using boolean value
    TriggerClientEvent('wais:hudHide', source, true or false) Only using boolean value
```

# Use of Notification

- There are 3 types for notification usage: information, warning and error. The types you use other than these types will automatically change to information. If you do not specify a duration, 2.5 seconds will be determined automatically.

```
    text = string
    type = string -> Only have information, warning and error
    duration = number

    TriggerEvent('wais:notification', text, type, duration)
    TriggerClientEvent('wais:notification', source, text, type, duration)
```

# Saltychat Range

- For Saltychat distance settings, you need to enter the saltychat config.json file and enter the distances one by one in Config.SaltychatRange as follows

```
    Element (Example "Whisper") 1 => It is the name of distance
    Element (Example 30) 2 => This part accepts only numbers and lengthens or shortens in the microphone bar in the hud according to the distance

    Config.SaltychatRange = {
        ["3.0"]  = { "Whisper",  30},
        ["7.0"]  = { "Normal",   65},
        ["15.0"] = { "Shouting", 100},
    }
```

# CONTACT

If there is a problem or you want to ask a question Discord: Ayazwai#3900 or [Discord 0RESMON](discord.gg/0resmon)
