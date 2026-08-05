# The Quadthmetic Meandian ヽ(・∀・)ﾉ

> "Stats tip: If you aren't sure whether to use the AM, GM, HM, or Median, just run all four recursively until math collapses completely out of confusion."

This is a single-file, zero-dependency web calculator inspired by [xkcd 2435: Geothmetic Meandian](https://xkcd.com/2435/). 

While Randall Munroe's comic joked about recursively computing the Arithmetic Mean, Geometric Mean, and Median, this tool introduces the Harmonic Mean to create a complete 4-mean mathematical squeeze, running the algorithm in real-time until the values converge to a single number at 10 significant figures. OwO

## Features ( ◡‿◡ )

* zero build pipeline means it is 100% vanilla HTML, CSS, and JS with no NPM, Webpack, or React needed so just open the file
* the xkcd aesthetic uses hand-drawn styling via Caveat and Comic Neue fonts complete with asymmetrical borders and sketchy interactive charts using [Chartist.js](https://gionkunz.github.io/chartist-js/)
* robust parser lets you throw anything at it like 10 apples, 40 bananas, 90.5 and the regex engine strips out the text and extracts the math
* csv export allows you to download a complete generation-by-generation log of the numbers collapsing
* deep linking works by clicking Share Dataset URL to generate a Base64-encoded URL that automatically loads your specific dataset when opened
* explainxkcd integration adds an on-page wiki-style breakdown of the mathematics and the comic transcript UwU

## Usage ( ´ ▽ ` )ﾉ

You can try it live here [Insert your GitHub Pages URL here]

### Local Setup

Because it is a single file, you don't even need a server to run it locally >w<
1. clone the repository or download index.html
2. double-click index.html to open it in any modern web browser
3. enter your data and watch the squeeze

## The Mathematics Why does it converge? (・`ω´・)

The system computes four primary measures of central tendency for a given set of positive numbers

1. arithmetic mean is the standard average
2. geometric mean is the $n$-th root of the product of all numbers
3. harmonic mean is the reciprocal of the average of the reciprocals
4. median is the exact middle value

The process is mathematically guaranteed to converge because of the strict inequality of the Pythagorean Means, which dictates that for any non-identical set of positive numbers

$HM < GM < AM$

On every single loop, the maximum boundary is pulled down, and the minimum boundary is pulled up. The Median acts as a chaotic anchor that forces the system into a true iterative sequence preventing the AM, GM, and HM from algebraically cancelling each other out instantly. The numbers act like a mathematical vise, squeezing tighter on every generation until the difference between them shrinks to absolute zero. ( ˘ ³˘)

## Built With (｡♥‿♥｡)

* vanilla JavaScript and HTML5
* [Chartist.js](https://gionkunz.github.io/chartist-js/) for SVG line charting
* Google Fonts using Comic Neue and Caveat