# Event Handling



## 이벤트 하나에 핸들러 두개 이상 추가하기

이벤트 하나에 핸들러를 두개 이상 추가하려면 어떻게 해야할까?



##### 1. inline javascript 구문에 핸들러 두번 사용하기

```html
<input type="text" v-on:input="handler1(); handler2();">
```



##### 2.  핸들러 배열을 전달하기

```html
<input type="text" v-on:input="[handler1(), hander2()]">
```



##### 3. 함수로 감싸기

```html
<input type="text" v-on:input="handler">
```

```javascript
...
methods: {
   hander: function() {
       hdlr1();
       hdlr2();
   },
   hdlr1: function() {
       
   },
   hdlr2: function() {
       
   },
}
...
```



##### 참조

https://stackoverflow.com/questions/38744932/how-to-call-multiple-functions-with-click-in-vue





