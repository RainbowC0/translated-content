---
title: SVG 核心属性
slug: Web/SVG/Attribute/Core
tags:
  - 属性
  - Intermediate
  - 参考
  - SVG
translation-of: Web/SVG/Attribute/Core
---
SVG 核心属性是所有可以指定在任何 SVG 元素上的通用属性。

- [`id`](#attr-id)
- [`lang`](#attr-lang)
- [`tabindex`](#attr-tabindex)
- [`xml:base`](#attr-xml:base)
- [`xml:lang`](#attr-xml:lang)
- [`xml:space`](#attr-xml:space)

## 属性

- {{SVGAttr('id')}}
  - : 定义在整个文档中必须唯一的唯一标识符 (ID)。 其目的是在链接（使用片段标识符）、脚本或样式（使用 CSS）时识别元素。
    *值*：一切合法字符串；*可变性*：**否**
- {{SVGAttr('lang')}}
  - : 参与定义元素的语言、编写不可编辑元素的语言或编写可编辑元素的语言。标签包含一个单一的条目值，其格式定义在 {{RFC(5646, "标识语言的标签（也称为 BCP 47）")}}。

    > **注意：**SVG 2 引入了新的 `lang` 属性。 如果同时使用 `lang` 和 `xml:lang` 属性，则 `xml:lang` 优先于 `lang`。
    *值*：一切合法 ID；*可变性*：**否**
- {{SVGAttr('tabindex')}}
  - : tabindex SVG 属性允许您控制元素是否可聚焦并定义元素的相对顺序以进行顺序焦点导航。
    *值类型*：[\<integer>](/zh-CN/docs/Web/SVG/Content_type#整型数); *可动性*：**否**
- {{SVGAttr('xml:base')}}
  - : 指定除文档的基本 IRI 之外的基本 IRI。
    *值类型*：[\<IRI>](/zh-CN/docs/Web/SVG/Content_type#iri); *可动性*：**否**
- {{SVGAttr('xml:lang')}}
  - : 它是所有 XML 语言中允许标记元素所包含的自然人类语言的通用属性。它的用法与 HTML 的 [lang](/zh-CN/docs/Web/HTML/Global_attributes/lang) 几乎相同，但是在符合XML 1.0文档的情况下，它不允许使用空值（`xml:lang=""`）来指示未知语言。而是使用`xml:lang="und"`。

    > **注意：**SVG 2 引入了新的 `lang` 属性。 如果同时使用 `lang` 和 `xml:lang` 属性，则 `xml:lang` 优先于 `lang`。
    *值*：一切合法 ID; *可动性*：**否**
- {{SVGAttr('xml:space')}} {{deprecated_inline}}
  - : SVG 支持标准 XML 属性 `xml:space`,以指定给定 {{ SVGElement("text") }} 元素的字符数据中空格字符的处理。

    > **注意：**你应该使用 {{cssxref('white-space')}} 属性，而不是 `xml:space` 属性。
    *值*：**`default`** | `preserve`; *可动性*：**否**

## 浏览器兼容性

{{Compat}}
