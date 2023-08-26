# HTML

## SGML 慣用語法

### 標籤 Tags

ex.&lt;p&gt; &lt;p/&gt;

### 屬性 Attributes

width、height、src 就是 Attributes

```HTML
// HTML
<img width="600" height="300" src="./images/故宮圖片 2.jpeg"alt="故宮圖片 2"/>
```

## 內容:HTML5 基本結構

&lt;script&gt; **程式碼**放在這裡面

```HTML
// HTML
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8"/>
<title>Ch1_4_2.html</title>
</head>
<body onload = "javascript:alert('大家好')">
    <script>
       document.write("第一支JAVA程式!" + "<br>");
    </script>
</body>
</html>
```

# Java Script

## 引用外部 JS 檔案

```HTML
// HTML
<script src="Ch1_5_3.js"></script>
```

## 註解

一行註解//

多行註解

```HTML
// HTML
/*

*/
```

## 變數/資料型態/運算子/資料型態轉換

### 變數

#### 命名

- 變數名稱區分大小寫
- 不能使用保留字 ex.for、var
- 變數名稱開頭只能使用 英文 跟 \_  
  <font color=red>**數字** 跟 **.** 不可當變數名稱</font>

#### 宣告

- 多個變數用 , 分隔
- 可以宣告完後，直接賦值

#### 變數是否存在

存在跑 A，不存在跑 B

```Java Script
// Java Script
<script>
// 變數宣告
var strName = "陳會安";
// 檢查變數是否存在
if (window.strName)
   document.write("strName存在:" + window.strName + "<br/>");
else
   document.write("strName不存在:" + window.strName + "<br/>");
// 一個不存在的變數
if (window.intBalance)
   document.write("intBalance存在:" + window.intBalance + "<br/>");
else
   document.write("intBalance不存在:" + window.intBalance + "<br/>");
</script>
```

### 資料型態

#### 數值

- 整數值  
  包含 0、正整數、負整數  
  可用十進位、八進位(0 開頭，每個位數值是 0\~7)、十六進位(0x 開頭，每個位數值是 0\~9、A\~F)

- 浮點數值

#### 字串

- 用\' 或 \"

#### 布林值

True 或 False

#### Null

表示 空 或 不存在 的特殊值，故意設為沒有值  
<font color=red>明確設置為\"沒有值\"的情況</font>

```Java Script
// Java Script
var myVar = null;
```

#### Undefined

- 有存在，尚未定義變數值
- 變數不存在

```Java Script
// Java Script
var myVar;
var myVar = undefined;
```

#### escape 逸出字元

在字元資料型態中顯示無法使用鍵盤輸入的特殊字元

| escape |         說明          |
| :----: | :-------------------: |
|  \\b   |       Backspace       |
|  \\f   |     FF、Formfeed      |
|  \\n   | LF、Linefeed 換行符號 |
|  \\r   |     CR、Enter 鍵      |
|  \\t   |        Tab 鍵         |
|  \\\'  |        \' 符號        |
|  \\\"  |       \\\" 符號       |
|  \\\\  |       \\\\ 符號       |

### 運算子

#### 說明

先乘除後加減

#### 順序

|    運算子    |               說明               | 性質 |
| :----------: | :------------------------------: | :--: |
|     ( )      |               括號               |
|  !、++、--   |    邏輯運算子 Not、遞增、遞減    |
|      -       |               負號               |
|   \*、/、%   |         乘法、除法、餘數         |
|     +、-     |            加法、減法            |
| <<、>>、>>>  | 位元運算子左移、右移、無符號右移 |
| >、>=、<、<= |             \' 符號              |
|    ==、!=    |            \\\" 符號             |
|      &       |            \\\\ 符號             |
|      ^       |            \\\\ 符號             |
|      \|      |            \\\\ 符號             |
|      &&      |            \\\\ 符號             |
|     \|\|     |            \\\\ 符號             |
|      ?:      |            \\\\ 符號             |
|    =、op=    |            \\\\ 符號             |

#### 種類

#### 比較

#### 邏輯

#### 位元運算子

#### 指定運算子

### 資料型態轉換

#### 轉換函數

```Java Script
// Java Script
parselnt( )
```
