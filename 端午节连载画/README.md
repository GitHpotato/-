### ���³��μ����ű��ԣ��������¼һ�£��Ժ�Ҳ�ھ���¼�Լ���ΪС����ĳɳ����̡�  
***
##### *��Markdown�����Ǻ���Ϥ�������Ű���һ�㣬��Ǹ��;*  
### 1���оٳ��õ����ڱ�ǩ�鼶��ǩ�Ϳձ�ǩ
* ����Ԫ�أ�������Ԫ����ͬһ���ϣ�Ԫ�ؿ�/�߼�����/�ײ��߾಻�����ã�Ԫ�ؿ��Ϊ�������ݿ�Ȳ��ɸı�  
    * ���磺a��big��br��code��em��i��img��input small��span��strong��label��q
* �鼶Ԫ�أ�ÿ���鼶Ԫ�ض�����һ�п�ʼ��Ԫ�ؿ�/�߼�����/�ײ��߾���Զ��壬Ԫ��Ĭ������º�����Ԫ�ؿ��һ��  
  * ���磺 ```div��dl��form��hϵ�С�menu��p��pre��ul��ol```
* ��Ԫ�أ�ָ������HTML�У�û������
  * ���磺```br��hr��input��img��link```
***
### 2��display����Щ����ֵ˵�����ǵ�����
```javascript
 * display:none;//��Ԫ�ز��ᱻ��ʾ
 * display:block;//��Ԫ���Կ鼶Ԫ��չʾ��ǰ���л��з�
 * display:inline;//Ĭ��ֵ��������Ԫ����ʾ����ǰ���з�
 * display:inline-block;//���ڿ鼶Ԫ��
 * display:table;//��Ԫ���Կ鼶�������ʾ  
 ```
 ***
### 3��̸̸position�ļ��ֶ�λ
```javascript
 * positipon:static;//Ĭ��ֵ��û�ж�λ;
 * position:relative;//��Զ�λ���������ԭ����ռ��λ��Ϊ��׼����ƫ�ƣ�
 * position:absolute;//���Զ�λ������ڵ�һ����Ĭ�϶�λ����ĸ�Ԫ�ؽ��ж�λ��
 * position:fixed;//�̶���λ���������������ڽ��ж�λ���Ҳ�������Ļ������
 ```
  ***
 ### 4����˵һ�º���ģ��
 * ����ģ�������֣�
   * W3C��׼����ģ��
   * IE�Ĺ������ģ��
 * W3C����ı�׼��ģ�Ͱ�����
 ```
   * margin border padding content
 ```
 * ��׼��ģ����Ԫ�ص�width=content��
 * IE�����ģ�ʹ������׼��ģ����ͬ���������ڣ�
   * �����ģ����Ԫ�ص�width=content+padding+border
 * ��CSS3�У�
 ```javascript
   * box-sizing:content-box
   * box-sizing:border-box
   * box-sizing:inherit
   * box-sizing: inherit;//�涨Ӧ�Ӹ�Ԫ�ؼ̳� box-sizing���Ե�ֵ��
   ```
 * ��box-sizingָ������ģ������
   * content-boxָ������ģ��ΪW3C����׼��ģ��)
   * border-boxΪIE����ģ�ͣ������ģ�ͣ�
 ***
  ### 5��H5��CSS3��������
* ���廯��ǩ��
 ``` header��footer��nav��section��aside��article```
 * ��Ƶ��Ƶ��```audio��video```
 * ���ƣ�```canvas```
 * ��ק��```draggable``` ����Ϊtrue ���Ա���ק
 * ���ش洢��
 * ```localStorage``` - û��ʱ�����Ƶ����ݴ洢��
 * ```sessionStorage``` - ���һ��```session```�����ݴ洢��
 *    ���û��ر���������ں����ݻᱻɾ����
 * ���¼���```onresize��ondrag��onscroll��onmousewheel��onerror��onplay��onpause```
 #### CSS3�������� 
 * ***ѡ����***��
 ```
    * :last/first-childѡ��Ԫ����/β�Ӵ�
    * :nth-child(num/even/odd)ѡ��ָ��/ż��/����
    * :checkedѡ��ÿ����ѡ�е�Ԫ��
    * ::selectionѡ���û�ѡȡ��Ԫ�ز���
```
 * ***α��*** 
 ```
   * a:link{color:skyblue}ѡ��δ���ʵ�����
   * a:hover{color:skyblue}����ƶ���������
   * a:avtive{color:skyblue}ѡ�е�����
 ```
  * ***�����ͱ߿�*** 
 ```
    * background-size:�涨����ͼ�ߴ�
    * background-origin:�涨����ͼƬ�Ķ�λ����
    * ����ͼƬ���Է����� content-box��padding-box �� border-box ����
    * border-radius:Բ��
    * box-shadow/text-shadow:��Ӱ
    * border-image:�߿�ͼƬ
    * translate():Ԫ�شӵ�ǰλ���ƶ������ݸ�����left(x����)��top(y����)����
```
 ***
### 6��̸̸����������������
 * ���������Ϊ����߶�̮��
 * ��Ϊ��Ԫ�ظ�����ʹ��Ԫ�ظ߶��޷���������ɸ߶�̮��
 * �������ڸ�Ԫ����������```overflow:auto/hidden```�Ϳ�����
 * ��һ����������ķ����������������Ԫ�ص�ǰ�����ӿ�```div```
 * ������ʽ```clear��both;```
  ***
### 7��̸̸ajax�е�get��post����дһ��ajax
  get��post����ajax����õ���������ʽ���У�
 * ***get����*** 
   * get�д�����������URL��β������ ����������URL��ַ��β�����ݲ����Ŀ��ˣ����������=ֵ����ʽ����&��������
   * get��������ͻ��˿ɼ�����˲���ȫ
   * ��Ϊ���ڵ�ַ����ƴ�Ӳ������Դ���������С��2KB���ң�
 * ***post����*** 
   * post�д����Ƿ���http�����У�
   * ����������˸���ȫ���Ҵ�����������
 * ***��дajax***
  ```javascript
 function hxp_ajax(obj){
     if(obj.type.toLowerCase()=='get'){
         var arr=[];
         for(var jian in obj.data){
             let str=`${jian}=${obj.data[jian]}`;
             arr.push(str);
         }
         var ps=arr.join('&');
         data.url+=ps;
     }else{
         var formdata=new FormData();
         for(let jian in obj.data){
             formdata.append(jian,obj.data[jian]);
         }
     }
 var xhr=new XMLHttpRequest();
     xhr.onreadystatechange=function(){
         if(xhr.readyState==4){
             if(xhr.status==200){
                 console.log(xhr.responseText)
                 console.log(JSON.parse(xhr.responseText))
             }
         }
     }
     xhr.timeout=3000;
     xhr.timeout=function(){
         console.log('����ʱ')��
     }
     xhr.open(obj.type,obj.url,true);
     obj.type.toLowerCase()=='get'?xhr.send(null:xhr.send(formdata);
 }
 ```
   ***
  ### 8��̸̸cookie��sessionStorage��localStorage��������ϵ
 * ***cookie***  
   * cookie����ʼ����ͬԴhttp������Я������������ͷ�����֮�����ش���
   * ��С��cookie�������ݺ�С������4KB��
   * ���ã�http���󶼻�Я��cookie��ֻ�ʺ�Я��С�����磺�Ự��ʶ
   * ����ʱ�䣺�������õ�cookie����ʱ��֮ǰ
 * ***sessionStorage��localStorage*** 
     * ����һ����ڱ��ر���
     * ��С�����߶��ܴ�ɴ�5M����
     * ����ʱ�䣺
        * ```sessionStorage```���ڵ�ǰ�����ҳ��ر�֮ǰ��Ч
        * ```localStorage```ʼ����Ч����ʹ�����ҳ��/���ڹر�Ҳ��һֱ����
     * ���ã������־����ݵı���
 ***
### 9��̸̸JavaScript�е�ԭ�����ͼ̳�
 ``` �����漰�˺ܶ�,�Ҹ���Ҳ���˺ܶ�ʼ�,����ֻ����˵��```
 * JavaScript��ͨ��ԭ����ʵ�ַ����ļ̳и���,����ļ������ظ��Ĵ����д��Ҳ�ô�����ӵ�����淶
 * ԭ����ʵ�ּ̳У���ʵ��������̳и������Ժͷ�����
 * ʵ�ּ̳еĹؼ�֮������
 ```javascript
   Son.prototype = new Father();
   var sonObj_2 = new Son();
 ```
 * ����ܺ����ͨ��new Son()���ɵ�ʵ������
``` 
sonObj_2�е�protoָ��Son.prototype
  ��Son.prototype��ָ��Father��ʵ������
  Father��ʵ�������protoָ��Father.prototype
  ���Sonʵ�������Ķ���ͨ��ԭ�����Ĳ���
  �����й��캯��Father���ϵ����Ժͷ�����
 ```
 ### 10������һ���ַ���������ַ����г���Ƶ����ߵ��ַ�
 ```javascript
 function seleMax(){
    var str=document.getElementById('text').value;
    var arr=str.split('');
    var json=[];
    for(let i=0; i<arr.length;i++){
        json[arr[i]]?json[arr[i]]+=1:json[arr[i]]=1;
    }
    var char='';
    var num=0;
    for(var hxp in json){
        json[hxp]>num?(num=json[hxp],char=hxp):null
    }
    console.log(json);
    console.log(`����Ƶ����ߵ��ַ�Ϊ${char},��������${num}��`);
}
 ```
 ![������Խ��](https://user-gold-cdn.xitu.io/2019/9/24/16d6131b8a1af712?w=520&h=324&f=png&s=20685)
 ##### ��������һ�������ŵı�����ܼ򵥣���Ȼ��˵�����ܶ��������Һ������Ѽ�һЩ���������ģ��������������Щ������Ϊһ�����ĵ�С�˼�������ϣ����λָ����