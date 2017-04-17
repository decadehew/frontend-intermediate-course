# 從新手到中手：前端工程加強班

## Homework 1
### 作業名稱:
  *基本 HTML/CSS 練習：以 Twitch 為例*

## 自我練習
1. 請問 CSS 的屬性position有哪幾種值？
  * absolute, fixed, relative, static, inherit

2. 承上，請問那幾種值有哪些區別？請講出適合應用的地方。
  * absolute会脱离normal flow，而且可以设定位置使它偏移
  * relative是相对，保留normal flow，和static一样。
  * 但是用这个absolute和relative要特别注意，最好方式先再container设定relative，然后在content设定absolute偏移，这样它就会在相对容器内偏移。
  * fixed和absolute有点类似，一旦固定位置，它不会移动，大多数都用在导航(navigate)列表中。

3. display的三個值inline, block, inline-block有什麼異同？可以試著舉出幾個例子嗎？
  * 假设div设定成inline不会有段落。而如果block elements会有段落。inline-block像inline但它有保留block功能。
  * 一般想把列表排成一排的话，例如导航navigate可以使用inline或inline-block

4. 有哪些 HTML 元素是 inline, 哪些是 block？
  * [inline: span，a, img...] | [block: div, p, h1...].

5. 當我設定一個元素的width為300px，並且padding設成10px之後，這個元素的寬度應該會是多少？
  * 320px, padding左右10px [padding-left + width + padding-right = 320px]
  * 如果使用box-sizing: border-box; 会强制把border，padding w或h(计算)加进去 会变成300px；
  * 使用box-sizing的好处，可以避免宽度爆炸

6. 這次實作的畫面當頻道名稱字太多的時候，會超出一格的大小或者會直接被卡掉，有沒有辦法讓字太多的時候在尾巴顯示...？例如原本名稱叫做：「1234567」，顯示的時候變成：「12345...」？
  * 会把文字width设定，如果要显示[1234567]，会使用width来设定可以容下的宽度，使用%作为单位。(或许我误解问题意思)
