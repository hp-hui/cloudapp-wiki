## device

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| getDiskInfos | void | [DiskInfoList](#diskinfo) | get disk infos |
| sms | [SMSTable](#smstable) | boolean | |
| auth | msg:string, callback:LuaFunction | boolean | ios only, finger auth. |
| call | phonenumber:string | boolean | |
| getPasteboardText | void | string | |
| setPasteboardText | value:string | |
| getNetworkType | void | string | |
| canOpenURL | url:string | boolean | |
| openURL | url:string | boolean | |
| hasApp | appidentifier:string | boolean | |
| openApp | appidentifier:string | boolean | |
| getUUID | void | string | get device uuid | |
| loadFont | fontPath:string, fontname:string | void | |
| playSoundFile | path:string | void | |
| clearSoundCache | void | void | ios only |
| vibrate | void | void | |
| setScreenOrientation | currentOrientation:ScreenOrientation | boolean | android only |

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| userAgent | string | rw |
| statusBarHidden | boolean | rw |
| statusBarStyle | StatusBarStyle | rw, refer to StatusBarStyleDefault,StatusBarStyleLightContent |
| batteryLevel | number | read only. |
| flashlight | boolean | rw |
| wlan | boolean | read only. |
| statusBarHeight | number | read only,android only |

### Constants
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| LANDSCAPE | ScreenOrientation | |
| PORTRAIT | ScreenOrientation | |
| StatusBarStyleDefault | StatusBarStyle | |
| StatusBarStyleLightContent | StatusBarStyle | |


DiskInfo
========
```js
{
    {
        "freeSpace": 123,
        "totalSpace": 456,
        "deviceName": "/dev/disk1",
        "format": "nfs"
    }
    ...
}
```
SMSTable
========
```js
{
    "message": "xxx",
    "numbers": [
        13811111111,
        13822222222
    ]
}
```
