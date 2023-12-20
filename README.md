### Answer

* 1.JavaScript: 字串反轉

```javascript
function reverseString(str) {
  return str.split('').reverse().join('');
}
```

* 2.JavaScript: 陣列過濾

```javascript
function getNumbersGreaterThan5(arr) {
  return arr.filter(number => number > 5);
}
```

* 3.JavaScript: 重構
* 此為合併姓名的函示，姓名之前加入空格。改使用filter，將 firstName 和 lastName 放入陣列中，然後使用 filter(Boolean) 來去除值為 undefined 或 null的元素。之後使用 join 方法將陣列中的元素連接成一個字符串，以空格分隔。

```javascript
function formatName(firstName, lastName) {
  const formattedName = [firstName, lastName].filter((name) => name);
  return formattedNameParts.join(' ');
}
```

* 4.React: 條件渲染
* 可以使用if判斷，以下是使用三元條件範例

```javascript
function ConditionalRendering({ isLoggedIn }) {
  return (
    <div>
      {isLoggedIn ? (//content1) : (//content2)}
    </div>
  );
}
```

* 5.React: 組件
* 建立一個count.js檔案，引入react，最後export出去使用

```javascript
function Counter() {
  const [count, setCount] = useState(0);
      
    onst increaseCount = () => {
      setCount(count + 1);
    };
      
        const decreaseCount = () => {
          setCount(count - 1);
        };
      
        return (
          <div>
            <p>Count: {count}</p>
            <button onClick={increaseCount}>Increase</button>
            <button onClick={decreaseCount}>Decrease</button>
          </div>
        );
      }
      
      export default Counter;
```