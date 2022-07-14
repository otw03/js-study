# js ****배열 중복 제거하는 방법 set()****

### **set() 사용하여 배열에서 중복 제거하는 방법**

**`Set`** 객체는 자료형에 관계 없이 [원시 값](https://developer.mozilla.org/ko/docs/Glossary/Primitive)과 객체 참조 모두 유일한 값을 저장할 수 있습니다.

```jsx
const array = ['C', 'A', 'B', 'A', 'C', 'D', 'C', 'C', 'E', 'D'];
console.log(array);	// ['C', 'A', 'B', 'A', 'C', 'D', 'C', 'C', 'E', 'D']

let result1 = [...new Set(array)];
console.log(result1);	// ['C', 'A', 'B', 'D', 'E']

let result2 = Array.from(new Set(array));
console.log(result2);	// ['C', 'A', 'B', 'D', 'E']
```

**Set**은 **유니크**한 값만을 담을 수 있기 때문에 **배열을 Set 형태로 만들어 중복을 제거하고,**

다시 **배열 안에서 전개연산자(...)**를 사용하여 중복이 제거된 배열로 만들거나,

**Array.from()**을 사용하여 중복이 제거된 Set으로부터 배열로 만들면 됩니다.  




[[출처] **Set - JavaScript - MDN Web Docs**](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Set)

[[출처] **JavaScript 배열 중복 제거하는 방법 5가지 | 작성자 김씩씩**](https://jsikim1.tistory.com/227)