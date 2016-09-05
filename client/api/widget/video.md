## video
video widget

### Properties
| Property      | Type          | Description   |
| ------------- | ------------- | ------------- |
| src | string | |
| sourceType | string | File / Streaming / Unknown |
| repeatMode | string | One / None |
| controlStyle | string | Embedded / Fullscreen / None |
| scalingMode | string | AspectFit / AspectFill / Fill |
| allowsAirPlay | boolean | android Unsupport |
| currentPlaybackTime | number | |
| currentPlaybackRate | number | android Unsupport |
| duration | number | readonly |
| playableDuration | number | readonly, video buffered duration |

### APIs
| Property      | Parameters    | Return Type   | Description   |
| ------------- | ------------- | ------------- | ------------- |
| seekingForward | void | void | |
| seekingBackward | void | void | |
| endSeeking | void | void | android Unsupport |
| play | void | void | |
| pause | void | void | |
| stop | void | void | |

### callback list
| Property      | Parameters    | Description   |
| ------------- | ------------- | ------------- |
| onloadstate | void | |
| onplaybackstate | void | |
| onpreparedtoplay | void | |
| onplaybackfinish | void | |

### Constants
LoadStateUnknown
LoadStatePlayable
StatePlaythroughOK
LoadStateStalled
PlaybackStateStopped
PlaybackStatePlaying
PlaybackStatePaused
PlaybackStateInterrupted
PlaybackStateSeekingForward
PlaybackStateSeekingBackward
FinishReasonPlaybackEnded
FinishReasonPlaybackError
FinishReasonUserExited

### xml schema
```xml
<video src="xxx" >
```

### xml sample
```xml
<video src="http://xxx.xxx.xxx/xxx.mp4"/>
```

### lua sample
```lua

```
