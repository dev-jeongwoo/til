# Array

## some()

배열 아의 어떤 요소라도 주어진 판별 함수를 통과하는지 테스트

빈 배열에서 호출하면 무조건 `false`반환

```javascript
arr.some(callback[, this.Args])
```

### 매개변수

#### callback

**currentValue**

현재 처리할 요소

**index**(optional)

처리할 요소의 인덱스

**array**(optional)

some을 호출한 배열

#### this.args(optional)

### 반환값

callback 이 어떤 배열 요소에 참인 값을 반환하는 경우 true, 그 외엔 false