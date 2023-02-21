---
title: "Programmation lettrée et _Notebook_"
author: "Module d'initiation à R - Ecole d'été du CIST 2023 - Ouidah, Bénin"
output:
  ioslides_presentation:
    logo: img/rmarkdown.png
    keep_md: yes
  beamer_presentation: default
pagetitle: Atelier pratique avec Rmarkdown
subtitle: __Atelier pratique avec Rmarkdown__
---



<style type="text/css">
.title-slide {
  background-image: url('assets/sharon-mccutcheon-576867-unsplash.jpg');
  background-size: cover;
  background-position: center;
  background-blend-mode: lighten;
}
</style>


## Exemple simple : rmd en pdf 


```{=html}
<div class="columns-2">
<embed src="simple.pdf" type="application/pdf" width="100%" height="500px"/>
<div>
<iframe srcdoc="&lt;!DOCTYPE html&gt;&#10;&lt;html xmlns=&quot;http://www.w3.org/1999/xhtml&quot; lang=&quot;fr&quot; xml:lang=&quot;fr&quot;&gt;&#10;&lt;head&gt;&#10;  &lt;meta charset=&quot;utf-8&quot; /&gt;&#10;  &lt;meta name=&quot;generator&quot; content=&quot;pandoc&quot; /&gt;&#10;  &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0, user-scalable=yes&quot; /&gt;&#10;  &lt;title&gt;Fichier source (.rmd) :&lt;/title&gt;&#10;  &lt;style&gt;&#10;    html {&#10;      line-height: 1.5;&#10;      font-family: Georgia, serif;&#10;      font-size: 20px;&#10;      color: #1a1a1a;&#10;      background-color: #fdfdfd;&#10;    }&#10;    body {&#10;      margin: 0 auto;&#10;      max-width: 36em;&#10;      padding-left: 50px;&#10;      padding-right: 50px;&#10;      padding-top: 50px;&#10;      padding-bottom: 50px;&#10;      hyphens: auto;&#10;      overflow-wrap: break-word;&#10;      text-rendering: optimizeLegibility;&#10;      font-kerning: normal;&#10;    }&#10;    @media (max-width: 600px) {&#10;      body {&#10;        font-size: 0.9em;&#10;        padding: 1em;&#10;      }&#10;      h1 {&#10;        font-size: 1.8em;&#10;      }&#10;    }&#10;    @media print {&#10;      body {&#10;        background-color: transparent;&#10;        color: black;&#10;        font-size: 12pt;&#10;      }&#10;      p, h2, h3 {&#10;        orphans: 3;&#10;        widows: 3;&#10;      }&#10;      h2, h3, h4 {&#10;        page-break-after: avoid;&#10;      }&#10;    }&#10;    p {&#10;      margin: 1em 0;&#10;    }&#10;    a {&#10;      color: #1a1a1a;&#10;    }&#10;    a:visited {&#10;      color: #1a1a1a;&#10;    }&#10;    img {&#10;      max-width: 100%;&#10;    }&#10;    h1, h2, h3, h4, h5, h6 {&#10;      margin-top: 1.4em;&#10;    }&#10;    h5, h6 {&#10;      font-size: 1em;&#10;      font-style: italic;&#10;    }&#10;    h6 {&#10;      font-weight: normal;&#10;    }&#10;    ol, ul {&#10;      padding-left: 1.7em;&#10;      margin-top: 1em;&#10;    }&#10;    li &gt; ol, li &gt; ul {&#10;      margin-top: 0;&#10;    }&#10;    blockquote {&#10;      margin: 1em 0 1em 1.7em;&#10;      padding-left: 1em;&#10;      border-left: 2px solid #e6e6e6;&#10;      color: #606060;&#10;    }&#10;    code {&#10;      font-family: Menlo, Monaco, &#39;Lucida Console&#39;, Consolas, monospace;&#10;      font-size: 85%;&#10;      margin: 0;&#10;    }&#10;    pre {&#10;      margin: 1em 0;&#10;      overflow: auto;&#10;    }&#10;    pre code {&#10;      padding: 0;&#10;      overflow: visible;&#10;      overflow-wrap: normal;&#10;    }&#10;    .sourceCode {&#10;     background-color: transparent;&#10;     overflow: visible;&#10;    }&#10;    hr {&#10;      background-color: #1a1a1a;&#10;      border: none;&#10;      height: 1px;&#10;      margin: 1em 0;&#10;    }&#10;    table {&#10;      margin: 1em 0;&#10;      border-collapse: collapse;&#10;      width: 100%;&#10;      overflow-x: auto;&#10;      display: block;&#10;      font-variant-numeric: lining-nums tabular-nums;&#10;    }&#10;    table caption {&#10;      margin-bottom: 0.75em;&#10;    }&#10;    tbody {&#10;      margin-top: 0.5em;&#10;      border-top: 1px solid #1a1a1a;&#10;      border-bottom: 1px solid #1a1a1a;&#10;    }&#10;    th {&#10;      border-top: 1px solid #1a1a1a;&#10;      padding: 0.25em 0.5em 0.25em 0.5em;&#10;    }&#10;    td {&#10;      padding: 0.125em 0.5em 0.25em 0.5em;&#10;    }&#10;    header {&#10;      margin-bottom: 4em;&#10;      text-align: center;&#10;    }&#10;    #TOC li {&#10;      list-style: none;&#10;    }&#10;    #TOC ul {&#10;      padding-left: 1.3em;&#10;    }&#10;    #TOC &gt; ul {&#10;      padding-left: 0;&#10;    }&#10;    #TOC a:not(:hover) {&#10;      text-decoration: none;&#10;    }&#10;    code{white-space: pre-wrap;}&#10;    span.smallcaps{font-variant: small-caps;}&#10;    div.columns{display: flex; gap: min(4vw, 1.5em);}&#10;    div.column{flex: auto; overflow-x: auto;}&#10;    div.hanging-indent{margin-left: 1.5em; text-indent: -1.5em;}&#10;    ul.task-list{list-style: none;}&#10;    ul.task-list li input[type=&quot;checkbox&quot;] {&#10;      width: 0.8em;&#10;      margin: 0 0.8em 0.2em -1.6em;&#10;      vertical-align: middle;&#10;    }&#10;    pre &gt; code.sourceCode { white-space: pre; position: relative; }&#10;    pre &gt; code.sourceCode &gt; span { display: inline-block; line-height: 1.25; }&#10;    pre &gt; code.sourceCode &gt; span:empty { height: 1.2em; }&#10;    .sourceCode { overflow: visible; }&#10;    code.sourceCode &gt; span { color: inherit; text-decoration: inherit; }&#10;    div.sourceCode { margin: 1em 0; }&#10;    pre.sourceCode { margin: 0; }&#10;    @media screen {&#10;    div.sourceCode { overflow: auto; }&#10;    }&#10;    @media print {&#10;    pre &gt; code.sourceCode { white-space: pre-wrap; }&#10;    pre &gt; code.sourceCode &gt; span { text-indent: -5em; padding-left: 5em; }&#10;    }&#10;    pre.numberSource code&#10;      { counter-reset: source-line 0; }&#10;    pre.numberSource code &gt; span&#10;      { position: relative; left: -4em; counter-increment: source-line; }&#10;    pre.numberSource code &gt; span &gt; a:first-child::before&#10;      { content: counter(source-line);&#10;        position: relative; left: -1em; text-align: right; vertical-align: baseline;&#10;        border: none; display: inline-block;&#10;        -webkit-touch-callout: none; -webkit-user-select: none;&#10;        -khtml-user-select: none; -moz-user-select: none;&#10;        -ms-user-select: none; user-select: none;&#10;        padding: 0 4px; width: 4em;&#10;        color: #aaaaaa;&#10;      }&#10;    pre.numberSource { margin-left: 3em; border-left: 1px solid #aaaaaa;  padding-left: 4px; }&#10;    div.sourceCode&#10;      {   }&#10;    @media screen {&#10;    pre &gt; code.sourceCode &gt; span &gt; a:first-child::before { text-decoration: underline; }&#10;    }&#10;    code span.al { color: #ff0000; font-weight: bold; } /* Alert */&#10;    code span.an { color: #60a0b0; font-weight: bold; font-style: italic; } /* Annotation */&#10;    code span.at { color: #7d9029; } /* Attribute */&#10;    code span.bn { color: #40a070; } /* BaseN */&#10;    code span.bu { color: #008000; } /* BuiltIn */&#10;    code span.cf { color: #007020; font-weight: bold; } /* ControlFlow */&#10;    code span.ch { color: #4070a0; } /* Char */&#10;    code span.cn { color: #880000; } /* Constant */&#10;    code span.co { color: #60a0b0; font-style: italic; } /* Comment */&#10;    code span.cv { color: #60a0b0; font-weight: bold; font-style: italic; } /* CommentVar */&#10;    code span.do { color: #ba2121; font-style: italic; } /* Documentation */&#10;    code span.dt { color: #902000; } /* DataType */&#10;    code span.dv { color: #40a070; } /* DecVal */&#10;    code span.er { color: #ff0000; font-weight: bold; } /* Error */&#10;    code span.ex { } /* Extension */&#10;    code span.fl { color: #40a070; } /* Float */&#10;    code span.fu { color: #06287e; } /* Function */&#10;    code span.im { color: #008000; font-weight: bold; } /* Import */&#10;    code span.in { color: #60a0b0; font-weight: bold; font-style: italic; } /* Information */&#10;    code span.kw { color: #007020; font-weight: bold; } /* Keyword */&#10;    code span.op { color: #666666; } /* Operator */&#10;    code span.ot { color: #007020; } /* Other */&#10;    code span.pp { color: #bc7a00; } /* Preprocessor */&#10;    code span.sc { color: #4070a0; } /* SpecialChar */&#10;    code span.ss { color: #bb6688; } /* SpecialString */&#10;    code span.st { color: #4070a0; } /* String */&#10;    code span.va { color: #19177c; } /* Variable */&#10;    code span.vs { color: #4070a0; } /* VerbatimString */&#10;    code span.wa { color: #60a0b0; font-weight: bold; font-style: italic; } /* Warning */&#10;    .display.math{display: block; text-align: center; margin: 0.5rem auto;}&#10;  &lt;/style&gt;&#10;  &lt;!--[if lt IE 9]&gt;&#10;    &lt;script src=&quot;//cdnjs.cloudflare.com/ajax/libs/html5shiv/3.7.3/html5shiv-printshiv.min.js&quot;&gt;&lt;/script&gt;&#10;  &lt;![endif]--&gt;&#10;&lt;/head&gt;&#10;&lt;body&gt;&#10;&lt;header id=&quot;title-block-header&quot;&gt;&#10;&lt;h1 class=&quot;title&quot;&gt;Fichier source (.rmd) :&lt;/h1&gt;&#10;&lt;/header&gt;&#10;&lt;div class=&quot;sourceCode&quot; id=&quot;cb1&quot;&gt;&lt;pre&#10;class=&quot;sourceCode markdown&quot;&gt;&lt;code class=&quot;sourceCode markdown&quot;&gt;&lt;span id=&quot;cb1-1&quot;&gt;&lt;a href=&quot;#cb1-1&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;co&quot;&gt;---&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-2&quot;&gt;&lt;a href=&quot;#cb1-2&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;an&quot;&gt;title:&lt;/span&gt;&lt;span class=&quot;co&quot;&gt; &amp;quot;Mon module de cours&amp;quot;&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-3&quot;&gt;&lt;a href=&quot;#cb1-3&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;an&quot;&gt;author:&lt;/span&gt;&lt;span class=&quot;co&quot;&gt; &amp;quot;Marc Done&amp;quot;&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-4&quot;&gt;&lt;a href=&quot;#cb1-4&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;an&quot;&gt;date:&lt;/span&gt;&lt;span class=&quot;co&quot;&gt; &amp;quot;29/03/2023&amp;quot;&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-5&quot;&gt;&lt;a href=&quot;#cb1-5&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;an&quot;&gt;output:&lt;/span&gt;&lt;span class=&quot;co&quot;&gt; &lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-6&quot;&gt;&lt;a href=&quot;#cb1-6&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;co&quot;&gt;  pdf_document:&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-7&quot;&gt;&lt;a href=&quot;#cb1-7&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;co&quot;&gt;    df_print: kable&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-8&quot;&gt;&lt;a href=&quot;#cb1-8&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;co&quot;&gt;---&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-9&quot;&gt;&lt;a href=&quot;#cb1-9&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-10&quot;&gt;&lt;a href=&quot;#cb1-10&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-11&quot;&gt;&lt;a href=&quot;#cb1-11&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;fu&quot;&gt;## Introduction&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-12&quot;&gt;&lt;a href=&quot;#cb1-12&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-13&quot;&gt;&lt;a href=&quot;#cb1-13&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;Quelques mots sur les **objectifs de ce cours** et les données utilisées.&lt;/span&gt;&#10;&lt;span id=&quot;cb1-14&quot;&gt;&lt;a href=&quot;#cb1-14&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-15&quot;&gt;&lt;a href=&quot;#cb1-15&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;fu&quot;&gt;## Du texte et un graphique&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-16&quot;&gt;&lt;a href=&quot;#cb1-16&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-17&quot;&gt;&lt;a href=&quot;#cb1-17&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas euismod, dolor at faucibus finibus, lacus nunc gravida mauris, ac porttitor felis turpis a purus. Mauris aliquam risus ut erat accumsan, id gravida purus dignissim. Donec tortor est, fringilla sit amet magna at, mattis pulvinar erat. Aenean tellus ante, rutrum non purus eu, commodo vehicula leo. Mauris congue urna nec tristique eleifend. Sed tincidunt vel justo id pellentesque. Proin sagittis fermentum tellus, eu viverra neque eleifend at. Suspendisse potenti.&lt;/span&gt;&#10;&lt;span id=&quot;cb1-18&quot;&gt;&lt;a href=&quot;#cb1-18&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-19&quot;&gt;&lt;a href=&quot;#cb1-19&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;Source du graphique : http://r-statistics.co/Top50-Ggplot2-Visualizations-MasterList-R-Code.html&lt;/span&gt;&#10;&lt;span id=&quot;cb1-20&quot;&gt;&lt;a href=&quot;#cb1-20&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-21&quot;&gt;&lt;a href=&quot;#cb1-21&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;```{r graphique, eval = TRUE, echo = TRUE, message = FALSE, fig.height=4}&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-22&quot;&gt;&lt;a href=&quot;#cb1-22&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;library(ggplot2)&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-23&quot;&gt;&lt;a href=&quot;#cb1-23&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;library(quantmod)&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-24&quot;&gt;&lt;a href=&quot;#cb1-24&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;data(&amp;quot;economics&amp;quot;, package = &amp;quot;ggplot2&amp;quot;)&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-25&quot;&gt;&lt;a href=&quot;#cb1-25&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-26&quot;&gt;&lt;a href=&quot;#cb1-26&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;# Compute % Returns&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-27&quot;&gt;&lt;a href=&quot;#cb1-27&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;economics$returns_perc &amp;lt;- c(0, diff(economics$psavert)/economics$psavert[-length(economics$psavert)])&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-28&quot;&gt;&lt;a href=&quot;#cb1-28&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-29&quot;&gt;&lt;a href=&quot;#cb1-29&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;# Create break points and labels for axis ticks&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-30&quot;&gt;&lt;a href=&quot;#cb1-30&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;brks &amp;lt;- economics$date[seq(1, length(economics$date), 12)]&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-31&quot;&gt;&lt;a href=&quot;#cb1-31&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;lbls &amp;lt;- lubridate::year(economics$date[seq(1, length(economics$date), 12)])&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-32&quot;&gt;&lt;a href=&quot;#cb1-32&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-33&quot;&gt;&lt;a href=&quot;#cb1-33&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;# Plot&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-34&quot;&gt;&lt;a href=&quot;#cb1-34&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;ggplot(economics[1:100, ], aes(date, returns_perc)) + &lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-35&quot;&gt;&lt;a href=&quot;#cb1-35&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;  geom_area() + &lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-36&quot;&gt;&lt;a href=&quot;#cb1-36&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;  scale_x_date(breaks=brks, labels=lbls) + &lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-37&quot;&gt;&lt;a href=&quot;#cb1-37&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;  theme(axis.text.x = element_text(angle=90)) + &lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-38&quot;&gt;&lt;a href=&quot;#cb1-38&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;  labs(title=&amp;quot;Area Chart&amp;quot;, &lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-39&quot;&gt;&lt;a href=&quot;#cb1-39&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;       subtitle = &amp;quot;Perc Returns for Personal Savings&amp;quot;, &lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-40&quot;&gt;&lt;a href=&quot;#cb1-40&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;       y=&amp;quot;% Returns for Personal savings&amp;quot;, &lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-41&quot;&gt;&lt;a href=&quot;#cb1-41&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;       caption=&amp;quot;Source: economics&amp;quot;)&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-42&quot;&gt;&lt;a href=&quot;#cb1-42&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;```&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-43&quot;&gt;&lt;a href=&quot;#cb1-43&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-44&quot;&gt;&lt;a href=&quot;#cb1-44&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;fu&quot;&gt;## Un tableau avec quelques données&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-45&quot;&gt;&lt;a href=&quot;#cb1-45&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-46&quot;&gt;&lt;a href=&quot;#cb1-46&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;Voici un petit tableau :&lt;/span&gt;&#10;&lt;span id=&quot;cb1-47&quot;&gt;&lt;a href=&quot;#cb1-47&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-48&quot;&gt;&lt;a href=&quot;#cb1-48&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;```{r tableau}&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-49&quot;&gt;&lt;a href=&quot;#cb1-49&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;head(economics, n = 3L)&lt;/span&gt;&lt;/span&gt;&#10;&lt;span id=&quot;cb1-50&quot;&gt;&lt;a href=&quot;#cb1-50&quot; aria-hidden=&quot;true&quot; tabindex=&quot;-1&quot;&gt;&lt;/a&gt;&lt;span class=&quot;in&quot;&gt;```&lt;/span&gt;&lt;/span&gt;&lt;/code&gt;&lt;/pre&gt;&lt;/div&gt;&#10;&lt;/body&gt;&#10;&lt;/html&gt;" style="height:500px!important;"></iframe>
</div>
</div>
```

# Rmarkdown avec Rstudio

## Prise en main facile avec RStudio

Menu `File > New File > R Markdown...`

<img src="img/create_rmd.png" width="60%" style="display: block; margin: auto;" />


## Enregistrer le fichier .rmd crée

<img src="img/untitled2.png" width="100%" style="display: block; margin: auto;" />

## Compiler (*knit*) un Rmarkdown

<img src="img/knit2.png" width="100%" style="display: block; margin: auto;" />


## Fichier généré (exemple HTML) 

<iframe src="mon_premier_rmarkdown.html"></iframe>


# Comment cela fonctionne ?

##  🧶 Tricot d'un Rmarkdown ?

<img src="img/schema_rmd.png" width="100%" style="display: block; margin: auto;" />

<font size="4">Pandoc est généralement pré-installé sur les systèmes d'exploitation MACOS et Windows.</font>    
<font size="4">Si vous n'avez pas $\LaTeX$ d'installé, utilisez le package [`tinytex`](https://cran.r-project.org/package=tinytex) pour la compilation en pdf.</font>



## Les 3 composants d'un rmd

<img src="img/rmardown.PNG" width="100%" style="display: block; margin: auto;" />

## Les 3 composants d'un rmd

- **En-tête `YAML`** : indications de variables pour la compilation du document : métadonnées (titre, auteur, date...), type de document souhaité (format et template), options de mise en page (TOC, Bibliographie, CSS...).    
<font size="4">Documentation &rarr; [***R Markdown: The Definitive Guide***](https://bookdown.org/yihui/rmarkdown/html-document.html).</font>  

- **Texte balisé en `Markdown`** : texte en langage naturel mis forme grâce à la syntaxe markdown.    
<font size="4">Documentation &rarr; [***Learn X in Y minutes***](https://learnxinyminutes.com/docs/markdown/)</font>  

- **_Chunks_** : code qui sera affiché (ou pas) et dont le résultat sera inséré (ou pas) dans le document final. Plusieurs options permettent de gérer l'éxécution,  l'affichage du code et de résultats.   
<font size="4">Documentation &rarr; [***Chunk options and package options***](https://yihui.org/knitr/options/)</font>  


## A. En-tête du document (`YAML`)

```yaml
---
title: Programmation lettrée et Notebook
author: Marc Done
date: 2023-02-21
output: 
  ioslides_presentation:
    transition: slower
    incremental: true
    widescreen: true
    logo: img/rmarkdown.png
---
```

<font size="4">**De nombreuses variables sont paramétrables**. Certaines sont spécifiques à des formats de sortie ou à des templates. Mais, dans tous les cas :</font>

[`<svg aria-hidden="true" role="img" viewBox="0 0 576 512" style="height:1em;width:1.12em;vertical-align:-0.125em;margin-left:auto;margin-right:auto;font-size:inherit;fill:currentColor;overflow:visible;position:relative;"><path d="M569.517 440.013C587.975 472.007 564.806 512 527.94 512H48.054c-36.937 0-59.999-40.055-41.577-71.987L246.423 23.985c18.467-32.009 64.72-31.951 83.154 0l239.94 416.028zM288 354c-25.405 0-46 20.595-46 46s20.595 46 46 46 46-20.595 46-46-20.595-46-46-46zm-43.673-165.346l7.418 136c.347 6.364 5.609 11.346 11.982 11.346h48.546c6.373 0 11.635-4.982 11.982-11.346l7.418-136c.375-6.874-5.098-12.654-11.982-12.654h-63.383c-6.884 0-12.356 5.78-11.981 12.654z"/></svg>`{=html} **L'indentation des variables doit être parfaite !**]{}



## Multiplier les formats de sortie ?

La variable `output` vous offre la possibilité de produire plusieurs formats à partir du même fichier Rmd : 

```yaml
---
title: Programmation lettrée et Notebook
author: Marc Done
date: 2023-02-21
output: 
  html_document: default
  pdf_document: default
---
```

*Kniter* votre fichier en ligne de commande de la façon suivante :

```r
rmarkdown::render("mon_premier_rmarkdown.Rmd", output_format = "all")
```

## Les *templates* disponibles

<font size="5"> **De nombreux packages fournissent des modèles de mise en page prêts à l'emploi** :</font> 

<font size="4">`bookdown`, `distill`, `flexdashboard`, `hrbrthemes`, `komadown`, `komaletter`, `learnr`, `linl`, `memor`, `pagedown`, `papaja`, `pinp`, `prettydoc`, `radix`, `revealjs`, `rmarkdown`, `rmdformats`, `rmdshower`, `rticles`, `rzine`, `tufte`, `unilur`, `vitae`, `xaringan`...</font> 

<font size="5">Ils permettent de produire des documents de toute forme, comme :</font> 

<font size="4">
- des documents (pages) HTML,    
- des documents paginés (articles, livres, thèses) en pdf avec $\LaTeX$, docx, odt...,    
- des présentations/diaporama en format HTML, pdf ou pptx,    
- des tableaux de bord interactif,   
- des cours et sujets d'examens (interactif ou non),   
- et même des sites internet statiques !   
</font>


## Ex : `rmdformats` - modèle `readthedown`

```yaml
---
title: "Template readthedown proposé par le package rmdformats"
date: "2023-02-21"
output:
  rmdformats::readthedown:
    highlight: kate
---
```

</br>

L'interface Rstudio permet de générer un rmd paramétré dans un modèle de mise en page souhaité. Pour cela, installer le package qui fournit le template que vous souhaitez utiliser. Ex :

```r
install.packages("rmdformats")
```


## Exemple `rmdformats`

Une fois installé, les templates proposés par le package installés sont disponibles en clic-buton dans Rstudio :

<img src="img/rmdformats.png" width="60%" style="display: block; margin: auto;" />



## Ajouter ses variables... modulables !

Pour produire des rapports sur différentes périodes, zones géographiques... A partir du même fichier R Markdown ! 

```yaml
---
title: Rapport statistique IDH
output: html_document
params:
  annee: 2023
  region: Europe
---
```

</br>

*Kniter* votre fichier en ligne de commande de la façon suivante :

```r
rmarkdown::render("monfichier.Rmd", params = list(annee = 2013, region = Asie))
```

## Ajouter ses variables... modulables !

Cette fonctionnalité est aussi disponible en clic-bouton via l'interface Rstudio :

::: {.columns-2}

\

<img src="img/knit_buton2.png" width="30%" style="display: block; margin: auto;" />


<img src="img/params.png" width="60%" style="display: block; margin: auto;" />


<img src="img/params2.png" width="100%" style="display: block; margin: auto;" />

:::



## B. Zone de texte - balisage `markdown`



<img src="img/markdown_guide.png" width="100%" style="display: block; margin: auto;" />

[https://www.markdownguide.org/]{.linkcenter}

<style type="text/css">
.linkcenter {
  font-size: 60%;
}
</style>


## C. Bloc de code - *chunks*

Deux façons d'insérer du code dans son document :

1. **Code chunk**  

    ````r
    ```{r, eval=TRUE, echo=FALSE}
    
    head(mtcars)
    
    ```
    ````
    
    
2. **Inline code**, pour inclure du code dans une zone de texte

    ````markdown
    La moyenne est de `r mean(mtcars$cyl)`.
    ````

## Les [options disponibles](https://yihui.name/knitr/options/)


<img src="img/chunk_params.jpg" width="65%" style="display: block; margin: auto;" />


## *chunk* plurilingues


```r
names(knitr::knit_engines$get())
```

```
##  [1] "awk"       "bash"      "coffee"    "gawk"      "groovy"    "haskell"  
##  [7] "lein"      "mysql"     "node"      "octave"    "perl"      "php"      
## [13] "psql"      "Rscript"   "ruby"      "sas"       "scala"     "sed"      
## [19] "sh"        "stata"     "zsh"       "asis"      "asy"       "block"    
## [25] "block2"    "bslib"     "c"         "cat"       "cc"        "comment"  
## [31] "css"       "ditaa"     "dot"       "embed"     "eviews"    "exec"     
## [37] "fortran"   "fortran95" "go"        "highlight" "js"        "julia"    
## [43] "python"    "R"         "Rcpp"      "sass"      "scss"      "sql"      
## [49] "stan"      "targets"   "tikz"      "verbatim"  "glue"      "glue_sql" 
## [55] "gluesql"
```


## Ex : `python` et le package `reticulate` {.smaller}



1. Initialisation de la configuration

    ````r
    ```{r, include = FALSE, eval = TRUE}
    library(reticulate)
    use_python("usr/local/bin/python")
    use_virtualenv("r-reticulate")
    py_install(c("pandas", "numpy"))
    ```
    ````

1. Script python

    ````py
    ```{python, eval = TRUE}
    a = 15 + 45
    print(a)
    ```
    ````

    
    ```
    ## 60
    ```


## Exemple : `SQL` avec scripts externes



**Etape 1 : connexion à la base de données**  
````r
```{r , eval = TRUE}
conn <- DBI::dbConnect(RSQLite::SQLite(), path = ":memory:")
```
````

\

**Pour se déconnecter (en fin de document) :**  
````r
```{r , eval = TRUE}
DBI::dbDisconnect(conn)
```
````

---

**Etape 2 : Lecture et éxécution d'un fichier sql** 



````markdown
```{sql, connection=conn, code=readLines('sql/list_tables.sql')}

```
````


```sql
SELECT name FROM sqlite_master WHERE type='table';
```


<div class="knitsql-table">


Table: 1 records

|name   |
|:------|
|mtcars |

</div>








## Ex : `node.js` avec un script externe {.smaller}

Vous voulez présenter du code `node.js`.  
Vos scripts sont dans des fichiers `.js`.

Vous pouvez écrire :

````markdown
```{node, code=readLines('node/example.js')}
```
````


```javascript
const hi = (name) => {
  console.log("Hello " + name + "!");
};

hi("Bob");
```


# Un peu de documentation ?


## Cheatsheet Rmarkdown

[[R Markdown Cheat Sheet](https://posit.co/wp-content/uploads/2022/10/rmarkdown-1.pdf) par [RStudio](https://www.rstudio.com/), licence [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)]{.license}

<iframe src="https://posit.co/wp-content/uploads/2022/10/rmarkdown-1.pdf"></iframe>

<style type="text/css">
.license {
  font-size: 70%;
  position: absolute;
  top: 100px;
}
</style>


## Bibliographie


**Les références :**

- [Xie, Y., J.J. Allaire et G. Grolemund [_R Markdown: The Definitive Guide_](https://bookdown.org/yihui/rmarkdown/)]{.reference}   
- [Xie Yihui, [_`knitr` Elegant, flexible, and fast dynamic report generation with R_](https://yihui.name/knitr/)]{.reference}   
- [Xie, Y., C. Dervieux et E. Riederer [_R Markdown Cookbook_](https://bookdown.org/yihui/rmarkdown-cookbook/)]{.reference}   
- [Xie Yihui, [_bookdown: Authoring Books and Technical Documents with R Markdown_](https://bookdown.org/yihui/bookdown/)]{.reference}   

\

**En français :**

- [Julien Barnier, [_Introduction à R et au tidyverse - Diffuser et publier avec rmarkdown_](https://juba.github.io/tidyverse/13-rmarkdown.html)]{.reference}
- [Lino Galiana et al. (INSEE), [_Utilitaire - Produire des documents avec R Markdown_](https://www.book.utilitr.org/03_fiches_thematiques/fiche_rmarkdown)]{.reference}


<style type="text/css">
.reference {
  font-size: 76%;
}
</style>


## Crédits

Cette présentation est fortement inspirée d'un excellent support de communication existant, dont le code source est [disponible sur GitHub](https://github.com/RLesur/meetup-r-nantes-rmd).

- [Romain Lesur, [_Créez vos documents avec Rmarkdown_](https://rlesur.github.io/meetup-r-nantes-rmd/#1), Janvier 2019, Nantes]{.reference}


\

Il s'agit d'un document Rmarkdown au format ***ioslides***. Il a donc été très simple de repartir du code source original pour produire ce diaporama !



# À vous de jouer !



<!-- ## Le fonctionnement de R Markdown -->

<!-- Le package `rmarkdown` assure la bonne exécution des étapes suivantes : -->

<!-- - fichier `.Rmd`  fichier `.md` = `knitr`   -->
<!--   Exécution des chunks et insertion du résultat -->

<!-- - fichier `.md`  fichier `.html` ou `.tex`, `.docx`, `.odt`... = **Pandoc** -->

<!-- Pour les pdf avec $\LaTeX$, étape supplémentaire : -->

<!-- - fichier `.tex`  fichier `.pdf` = $\LaTeX$  -->

