# JS 流程控制 process control

## 基礎

- 循序結構
- 選擇結構 selection
- 重複結構 iteration

## 條件控制 if

### if 條件式一種是否執行的單選題

```Java Script
// Java Script
// 變數宣告
var strGender = "男";
// 條件敘述
if (strGender == "男"){
   document.write("男性網友您好! ");
   document.write("歡迎使用JavaScript<br/>");
}
```

### if / else 二選一條件敘述

```Java Script
// Java Script
// 變數宣告
var strGender;
strGender = "女";
// 條件敘述
if (strGender == "男"){
   document.write("男性網友您好! ");
}
else{
   document.write("女性網友您好! ");
}
document.write("歡迎使用JavaScript<br/>");
```

### if / else 多選一條件敘述

```Java Script
// Java Script
// 變數宣告
var strPayment = "visa";
// 多選一條件敘述
if (strPayment == "cash")
   document.write("使用現金付款!<br/>");
else
   if (strPayment == "visa")
       document.write("使用VISA信用卡付款!<br/>");
   else
       if (strPayment == "master")
           document.write("使用Master信用卡付款!<br/>");
       else
           document.write("未明的付款方式!<br/>");
```

### switch 多選一條件敘述

每個條件判斷完要加入 **break**

```Java Script
// Java Script
// 變數宣告
var strPayment = "master";
// 條件敘述
switch (strPayment){
    case "cash":
        document.write("使用現金付款!<br/>");
        break;
    case "visa":
        document.write("使用VISA信用卡付款!<br/>");
        break;
    case "master":
        document.write("使用Master信用卡付款!<br/>");
        break;
    default:
        document.write("未明的付款方式!<br/>");
}
```

### 條件運算子?:

? 代替 if ， : 代替 else

```Java Script
// Java Script
// 變數宣告
var strHours = "";
dtHour = 18;
strHours = (dtHour >= 12) ? " PM" : " AM";
dtHour = (dtHour >= 12) ? dtHour-12 : dtHour;
document.write("目前時間為: " + dtHour + strHours + "!<br/>");
```

## 迴圈  

### for 迴圈  

```Java Script
// Java Script
// 變數宣告
var i; 
var intSum = 0;
// 迴圈敘述
for (i = 1; i <= 5; i++){
    document.write("整數: " + i + "<br/>");
    intSum += i;
}
document.write("<hr/>總和: " + intSum + "<br/>");
```

### for / in 迴圈  

顯示物件的所有屬性  

```Java Script
// Java Script
// 變數宣告
var prop;
var objAddress = new Object();
objAddress.name = "陳會安";
objAddress.age = "40";
objAddress.phone = "02-22222222";
objAddress.email = "hueyan@ms2.hinet.net";
// 迴圈敘述
for (prop in objAddress){
    document.write("屬性: " + prop + "=" + objAddress[prop] + "<br/>");
}
```

### while 迴圈  

條件為true才能進入迴圈，false 離開迴圈  

```Java Script
// Java Script
// 變數宣告
var i = 1;
var intSum = 0;
// 迴圈敘述
while (i <= 6){
    document.write("整數: " + i + "<br/>");
    intSum += i;
    i++;
}
document.write("<hr/>總和: " + intSum + "<br/>");
```

### do / while 迴圈  

do 會先做第一次，之後才有while判斷是否執行  

```Java Script
// Java Script
// 變數宣告
var i = 1;
var intSum = 0;
// 迴圈敘述
do{
    document.write("整數: " + i + "<br/>");
    intSum += i;
    i++;
} while (i <= 6);
document.write("<hr/>總和: " + intSum + "<br/>");
```

### 跳出迴圈 break  

```Java Script
// Java Script
if (number == null || number == target)
    break;
```

### 繼續 continue  

```Java Script
// Java Script
if (number > target) {
    alert(number + "太大!");
    times++;
    continue;
}
```

### 巢狀迴圈  

```Java Script
// Java Script
document.write("<table border='1'>");
// 變數宣告
var i, j;
// 表格的標題列
document.write("<tr><td></td>");
for (i=1;i<=9;i++)
    document.write("<td><b>" + i + "</b></td>");
document.write("</tr>");
// 巢狀迴圈
for (i=1;i<=9;i++) {
    document.write("<tr>");
    document.write("<td><b>" + i + "</b></td>");
    j = 1;
    while (j <= 9) { // 內層迴圈
       document.write("<td>");
       document.write(i + "*" + j + "=" + i*j);
       document.write("</td>");
       j++;
    }
    document.write("</tr>");
}
document.write("</table>");
```


```Java Script
// Java Script

```
