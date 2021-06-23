# 日常工作中经常用到的live-templates
## 参考文档
官方文档在[Jetbrains Live Templates](https://www.jetbrains.com/help/idea/using-live-templates.html)

## 通用
### serialVersionUID
Abbreviation: svd

Description: serialVersionUID

Template text:
```
private static final long serialVersionUID = 1L;
```
Applicable in: Java>declaration



## 类属性
### private String
Abbreviation: pvs

Description: private String

Template text:
```
/**
 *
 */
private String $END$;
```
Applicable in: Java>declaration

### private BigDecimal
Abbreviation: pvb

Description: private BigDecimal

Template text:
```
/**
 *
 */
private BigDecimal $END$;
```
Applicable in: Java>declaration

### private Integer
Abbreviation: pvi

Description: private Integer

Template text:
```
/**
 *
 */
private Integer $END$;
```
Applicable in: Java>declaration

### private Long
Abbreviation: pvl

Description: private Long

Template text:
```
/**
 *
 */
private Long $END$;
```
Applicable in: Java>declaration

### Autowired属性
Abbreviation: apv

Description: Autowired private

Template text:
```
@Autowired
private $END$;
```
Applicable in: Java>declaration

## 局部变量
### new ArrayList
Abbreviation: list

Description: new ArrayList

Template text:
```
List<$END$> list = new ArrayList<>();
```
Applicable in: Java>statement

### new HashMap
Abbreviation: mp

Description: new HashMap

Template text:
```
Map<$END$> map = new HashMap<>();
```
Applicable in: Java>statement

### new HashSet
Abbreviation: st

Description: new HashSet

Template text:
```
Set<$END$> set = new HashSet<>();
```
Applicable in: Java>statement

## 逻辑判断
### 对象判断
Abbreviation: eqs

Description: Objects.equals

Template text:
```
if (Objects.equals($SELECTION$, $END$)) {
    
}
```
Applicable in: Java>statement

注: 选中相应变量后通过 ctrl + alt + j 快捷键触发

### 集合判空
Abbreviation: ce

Description: CollectionUtils.isEmpty

Template text:
```
if (CollectionUtils.isEmpty($SELECTION$)) {

}
```
Applicable in: Java>statement

注: 选中相应变量后通过 ctrl + alt + j 快捷键触发

### 字符串判空
Abbreviation: nb

Description: StringUtils.isNotBlank

Template text:
```
if (StringUtils.isNotBlank($SELECTION$)) {
            
}
```
Applicable in: Java>statement

注: 选中相应变量后通过 ctrl + alt + j 快捷键触发

## 日志记录
### 声明
Abbreviation: lg

Description: private static final Logger

Template text:
```
private static final Logger logger = LoggerFactory.getLogger($CLASS_NAME$.class);
```
Applicable in: Java>declaration

### info
Abbreviation: info

Description: logger.info

Template text:
```
logger.info("", $END$);
```
Applicable in: Java>statement


### error
Abbreviation: error

Description: logger.error

Template text:
```
logger.error("", $END$);
```
Applicable in: Java>statement

### warn
Abbreviation: warn

Description: logger.warn

Template text:
```
logger.warn("", $END$);
```
Applicable in: Java>statement

### 其它
### 抛出运行时异常
Abbreviation: rte

Description: throw new RuntimeException

Template text:
```
throw new RuntimeException("$END$");
```
Applicable in: Java>statement

### 字符串格式化
Abbreviation: sfmt

Description: String.format

Template text:
```
String.format("", $END$);
```
Applicable in: Java>statement
