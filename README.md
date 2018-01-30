# htmlhintrc
htmlhintrc

# Usage
## Step 1. Install htmlhintrc
```bash
npm i -D htmlhintrc
```

## Step 2. Copy `.htmlhintrc` to your project root
```bash
# cd your project root
cp node_modules/htmlhintrc/.htmlhintrc .htmlhintrc
```

## Rules
```js
{
  // 标签名小写
  "tagname-lowercase": true,
  // 属姓名小写
  "attr-lowercase": true,
  // 属性值使用双引号
  "attr-value-double-quotes": true,
  // 属性值可以为空
  "attr-value-not-empty": false,
  // 不能有重复属性值
  "attr-no-duplication": true,
  // 不需要声明
  "doctype-first": false,
  // 需要关闭所有非空元素<p><p>
  "tag-pair": true,
  // 需要关闭所有空元素<br/>
  "tag-self-close": true,
  // 需要转义特殊字符"&" "<" ">" ...
  "spec-char-escape": true,
  // ID不能重复
  "id-unique": true,
  // src值不能为空
  "src-not-empty": true,
  // 不需要每个html文件都拥有title元素
  "title-require": false,
  // 如果存在alt属性，则需要添加alt属性值
  "alt-require": true,
  // 不需要每个html文件都声明doctype
  "doctype-html5": false,
  // id, class的值以中划线分隔
  "id-class-value": "dash",
  // 不允许添加<style type="text/css"></style>标签
  "style-disabled": true,
  // 不允许添加行内css值<div style="color:red"></div>
  "inline-style-disabled": true,
  // 允许行内js脚本
  "inline-script-disabled": false,
  // 使用2个space代替tab
  "space-tab-mixed-disabled": "space2",
  // 允许id和class出现ad值，注含有ad的id或者class会被adblock软件block
  "id-class-ad-disabled": false,
  // 允许href属性值使用相对和绝对路径
  "href-abs-or-rel": false,
  // 不允许属性值使用不安全的字符
  "attr-unsafe-chars": true,
  // 不允许在head标签中使用script标签
  "head-script-disabled": true
}
```
