作者：raphealguo
ExtCSS介绍：http://rapheal.sinaapp.com/2013/02/26/extcss1-0/

2013/02/25 ======================================================
ExtCss-1.0：
1.支持原生CSS语法，有可能不支持（*color _color这类hack语法）
2.支持变量、函数
3.支持嵌套语法
4.支持新增的include require语法

2013/02/27 ======================================================
ExtCss-1.0.1：
1.修复重大的一个bug：#id { a:hover{}; } 与 #id { a:hover; }的二义性！
2.修复函数内无法调用另一个函数的bug
3.兼容LESS通过选择器名字来引用规则
4.修复不能以*_开头的CSS hack的bug

2013/02/28 ======================================================
ExtCss1.0.2：
1.修复解析的bug:IE对于filter存在的一些特殊函数，例如，filter: progid:DXImageTransform.Microsoft.gradient( GradientType = 0,startColorstr = '#82000000',endColorstr = '#82000000');
2.修复IE8的hack的bug：xxx:xxx\9;
3.修复@media等一些特殊的hack，例如，@media screen and (-webkit-min-device-pixel-ratio:0) 
4.修复一些特殊的选择器，如，::-webkit-scrollbar 有双冒号的选择器。
5.添加缩写特性，修改config/abbr.conf文件，可以自己定义一些缩写，例如，w=width
6.增加CSS文件输出模式：正常模式（normal模式）、压缩成一行(min模式)、每个规则集单独一行（line模式）
