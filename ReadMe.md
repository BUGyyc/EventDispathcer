# 事件派发

## 派发事件

### 不带参数
```CEventDispatcherObj.dispatchEvent(new CEvent(CEventName.TEST_EVENT),this);```


### 带参数
```CEventDispatcherObj.dispatchEvent(new CEvent(CEventName.TEST_EVENT,"hello world"),this);```


## 监听事件
```
CEventDispatcherObj.addEventListener(CEventName.TEST_EVENT,eventCallback);
```

```
public void eventCallback(CEvent evt){
    Debug.Log("evt  params -- "+evt.eventParams);
}
```



## 移除事件

```CEventDispatcherObj.removeEventListener(CEventName.TEST_EVENT,eventCallback);```
