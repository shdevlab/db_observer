 db_observer module ✨️
===

___**디비 파일 옵저버 입니다!**___

___**made by shdevlab**___



# what is that?

디비 파일 변경 및 값 삭제 등을 감지하는 모듈입니다.


# example

```js
let observe = require("db_observer");

let observer = observer.getInstance({
  "db": "sdcard/test.db"
});

observer.on("change", (type, value) => {

});

observer.start();

function onStartCompile() {
  observer.stop();
}
```