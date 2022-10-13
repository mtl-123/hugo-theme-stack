+++
author = "梅桃林"
title = "Emoji支持"
date = "2022-10-13"
description = "Hugo中的表情符号使用指南"
categories = [
    "emoji表情包"
]
tags = [
    "emoji",
]
image = "the-creative-exchange-d2zvqp3fpro-unsplash.jpg"
+++

在Hugo项目中可以通过多种方式启用表情符号。
<!--more-->
The [`emojify`](https://gohugo.io/functions/emojify/) function can be called directly in templates or [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes). 

若要全局启用表情符号，请设置 `enableEmoji` to `true` in your site's [configuration](https://gohugo.io/getting-started/configuration/) 然后你可以直接在内容文件中输入表情符号的简写代码;如。

<p><span class="nowrap"><span class="emojify">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙊</span> <code>:speak_no_evil:</code></span></p>
<br>

这 [表情符号备忘单](http://www.emoji-cheat-sheet.com/) 是表情符号速记代码的有用参考。

***

**N.B.** 上面的步骤在Hugo中启用了Unicode标准的表情符号字符和序列，但是这些符号的呈现取决于浏览器和平台。要样式的表情符号，你可以使用第三方的表情符号字体或字体堆栈;如。

{{< highlight html >}}
.emoji {
  font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol, Android Emoji, EmojiSymbols;
}
{{< /highlight >}}

{{< css.inline >}}
<style>
.emojify {
	font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol, Android Emoji, EmojiSymbols;
	font-size: 2rem;
	vertical-align: middle;
}
@media screen and (max-width:650px) {
  .nowrap {
    display: block;
    margin: 25px 0;
  }
}
</style>
{{< /css.inline >}}
