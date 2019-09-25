### �鿴�ٷ��ĵ�����ES6����һ�λ��ܣ������Լ���ͷ��ϰ��    
1��  ```let```ֻ�ڴ��������Ч���ⲿ�޷���ȡ�����ã��Ҳ����ڱ���������,ֻ������һ��
```JavaScript
{
    let a=0;
    console.log(a);//0
}
a;//����a is not defined
```
* ���� i ���� var �����ģ���ȫ�ַ�Χ����Ч������ȫ����ֻ��һ������ i, ÿ��ѭ��ʱ��setTimeout ��ʱ������� i ָ����ȫ�ֱ��� i ����ѭ�����ʮ�� setTimeout ����ѭ���������ִ�У����Դ�ʱ�� i ���� 10��

* ���� j ���� let �����ģ���ǰ�� i ֻ�ڱ���ѭ������Ч��ÿ��ѭ���� j ��ʵ����һ���µı��������� setTimeout ��ʱ������� j ��ʵ�ǲ�ͬ�ı�������������12345��
```
for (var i = 0; i < 10; i++) {
  setTimeout(function(){
    console.log(i);
  })
}
// ���ʮ�� 10
for (let j = 0; j < 10; j++) {
  setTimeout(function(){
    console.log(j);
  })
}
// ��� 0123456789
```
***
2 �� ```const```����һ��ֻ�����������ɸı䣬�����������ʼ�����ݣ����򱨴�
```
const PI = "3.1415926";
PI  // 3.1415926

const MY_AGE;  //����    
```
***
3���⹹��ֵ�������ֲ���
* �ṹ��Դ���⹹��ֵ���ʽ���ұ߲��֣�  
* �ṹ��Ŀ�꣺�ṹ��ֵ���ʽ����߲��֣�
##### ����ģ�͵Ľ⹹
```javascript
һ��������
 let [a, b, c] = [1, 2, 3];
   // ��ʱ a=1,b=2,c=3
����Ƕ����
  let [a, [[b],c]] = [1, [[2], 3]];
   // ��ʱ a=1,b=2,c=3
����������
  let [a, , c] = [1,2,3];
   //��ʱ a=1,c=3
�ġ�����ȫ�⹹��
   let[a=1,b]=[];
   //��ʱ a=1,b=undefined
�塢ʣ���������
   let[a,...b]=[1,2,3];
   //��ʱ a=1,b=[2,3]
�����ַ�����
  let [a,b,c,d,e,f]='potato';
  //��ʱ a=p,b=o,c=t......
//ps:һ����Ŀ���в�������ʱ����������������ֵ����Ŀ
 1������ES6�⹹����
     var a=1,b=2;
     [a,b]=[b,a];
 2������������н���
    var a=1,b=2;
    a=[b,b=a][0];
   ```
  ##### ����ģ�͵Ľ⹹
  ```javascript
  һ��������
  let {foo,bar}={foo:'xxx',bar:'yyy'};
  //��ʱfoo='xxx',bar='yyy';
  let {baz:foo}={baz:'ddd'};
  //��ʱfoo='ddd'
  ������Ƕ�׿ɺ���
  let {p: [x, {y}]} ={p: ['hello', {y: 'world'}] };
  console.log(x);//hello
  console.log(y);//world
  -----����----
  let {p: [x, {  }] } = {p: ['hello', {y: 'world'}] };
console.log(x);//hello
��������ȫ�⹹
let {p:[{y}, x]}={p: [{y:'world'}]};
console.log(x);//undefined
console.log(y);//world
�ġ�ʣ���������
let {a, b, ...rest} = {a: 10, b: 20, c: 30, d: 40};
console.log(a);//10
console.log(b);//20
console.log(rest);//{c: 30, d: 40}
�塢�⹹Ĭ��ֵ��
let {a: x = 10, b: y = 5} = {a: 3};
console.log(x);//3
console.log(y);//5
  ```