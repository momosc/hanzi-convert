# PHP 中文繁简体字转换
汉字中文繁简体转换，繁体转简体，简体转繁体，最全字库，共15356个

## 关于字库
之前使用过几个繁简体转换程序，发现其内置的字库都是日常生活常用字，对于一些古诗之类的有比较多繁体字的字符串，很多繁体字无法转换，故网络收集整理了这份相对比较全的字库，共收录了15356个繁体字，能够比较好的满足有较多生僻繁体字转换的需求。


## 使用方法

```
use sqhlib\Hanzi\HanziConvert;

//繁体转简体
$str = '平時已秉班揚筆，暇處不妨甘石經。吾里忻傳日邊信，君言頻中斗杓星。會稽夫子餘詩禮，巴蜀君平舊典型。歷歷周天三百度，更參璿玉到虞廷。';
echo HanziConvert::convert($str);

//简体转繁体
$str = '平时已秉班扬笔，暇处不妨甘石经。吾里忻传日边信，君言频中斗杓星。会稽夫子余诗礼，巴蜀君平旧典型。歷歷周天三百度，更参璇玉到虞廷。';
echo HanziConvert::convert($str,1);

```

## 注意事项
由于在中文中，一个简体字有的有多个繁体字写法，因此不能保证从繁体转成简体后再转成繁体和之前字形一样。

