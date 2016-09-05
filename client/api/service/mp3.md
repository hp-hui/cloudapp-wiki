## mp3

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| load | filePath:string | void | load audio file to play |
| play | oncomplete:LuaFunction | void | |
| getDuration | void | number | |
| getCurrentTime | void | number | |
| setCurrentTime | double | void | |
| startRecord | filePath:string | void | |
| stopRecord | void | void | |
| setSampleRate | number | void | default 11025 |

### Samples
```lua
local mp3 = registry.getService("mp3")
mp3:setSampleRate(8000)
mp3:startRecord("data:///record.mp3")

sleep(5)
mp3:stopRecord()
sleep(2)
mp3:load("data:///record.mp3")

print("duration", mp3:getDuration())
mp3:play()
sleep(2)
print("CurrentTime", mp3:getCurrentTime())
mp3:setCurrentTime(1)
sleep(3)
print("CurrentTime", mp3:getCurrentTime())
mp3:setCurrentTime(2)
```
