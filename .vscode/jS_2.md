
まず、if / elseの例を示す。

```javascript

var testStatus = 'ok';
if (testStatus === 'ok') {
    console.log('ok status');
} else if (testStatus === 'Bad') {
    console.log('bad status')
} else {
    console.log('Else status')
}
```

## 条件例

+ 等価   :   a === b

+ 否定   :   a !== bs

他、以上、以下など、その他プログラミング言語で使用されているものがある。

注意点  
== より === を使った方が良い。

```javascript  
// 例
23 == '23' -> true
23 === '23' -> false
```

## 条件が変数の場合

例えば

```javascript

const test = '';
if (!test) {
    console.log('Faulty value')
}
```

+ Faulth values  
   以下の値の場合、falseとして扱われる。  
   <h4> undefined, null, 0, '', NaN <h4>

+ Truety values  
  Faulty valus以外はtureとして扱われる。  
        
## 条件のBoolean Logic

+ AND : &&  
(条件 && 条件)

+ OR  : ||  
  (条件 || 条件)

+ NOT : !  
(!条件)

# 条件演算子 (Thernary Operator)

条件処理を１行で書く

```javascript
//条件 ? True処理: False処理
var age = 15;
var isAdult = age >= 20 ? '成年': '未成年';
console.log('Jane is ' + isAdult) //未成年
```

# Switch　

他のプログラミング言語でも良く出てくる。Pythonにはないかもしれないが、、、。   
以下に例を示す。
```
var A = 'C'
switch (A) {
    case 'B':
        console.log('Bの場合')
        break;
    case 2:
    case 'C':
        console.log('2 or Cの場合')
        break;
    default:
        console.log('条件に合わない')
}
```