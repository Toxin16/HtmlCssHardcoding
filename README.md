# HTML, CSS Coding
page : https://toxin16.github.io/HtmlCssHardcoding/

![_C__kmove_Kangsunghun_index html (1)](https://user-images.githubusercontent.com/109052012/191651502-1442ccb8-cacf-4f90-8649-eebb2b5d7e7e.png)

```html
<!DOCTYPE html>
<html lang="jp">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="css/style.css">
    <title>강성훈의 이력서</title>
</head>

<body>
    <a href = "index1.html">일본어 페이지</a>
    <div class="wrapper"></div>
    <h1>강성훈의 이력서</h1>

    <section id="my_info">
        <h2>My info</h2>
        <img src="images/ksh.png" alt="강성훈의 사진"/>
        <table>
            <tbody>
                <tr id = "myname">
                    <th>이름</th>
                    <td>강성훈</td>
                </tr>
                <tr>
                    <th>직업</th>
                    <td>취업준비생</td>
                </tr>
                <tr>
                    <th>나이</th>
                    <td>26</td>
                </tr>
                <tr>
                    <th>거주지</th>
                    <td>부산</td>
                </tr>
            </tbody>
        </table>
    </section>
    
    <section id="about">
        <h2>About</h2>
        <p>스펀지처럼 모든 것을 흡수해서 자신의 기술로 만들 수 있도록 하겠습니다. </p>
    </section>

    <section id="contact">
        <h2>Contact</h2>
        <ul>
            <li>
                <a href="tel:01000000000">010-0000-0000</a>
            </li>
            <li>
                <a href="https://www.instagram.com/kang99373" target="_blank">인스타그램</a>
            </li>
            <li>
                <a href="https://github.com/Toxin16" target="_blank">깃허브</a>
            </li>
        </ul>
    </section>

    <section id="skill">
        <h2>skills</h2>
        <ol>
            <li>HTML</li>
            <li>CSS</li>
            <li>SASS</li>
            <li>Javascript</li>
            <li>php</li>
            <li>JAVA</li>
        </ol>
    </section>

    <section id="project">
        <h2>PROJECTS</h2>
            <ol>
                <li>
                    <h3>내면 수련</h3>
<!--                    <video src=""></video> 
                    <p>Integer imperdiet accumsan dui eget imperdiet. Nulla cursus sed metus posuere fringilla.</p>
-->
                    <a href="https://www.youtube.com/watch?v=4-YVVziGXc0" target="_blank">법륜스님의 희망세상 만들기 (언짢은 말을 들으면 떨쳐내기가 힘들어요)</a>
                </li>
            </ol>
    </section>

</body>
</html>
```



```CSS
**@charset "UTF-8";
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR&display=swap');

body {
    background-color: #f5f5f5;
    color: #2f2f2f;
    font-family: 'Noto Sans KR', sans-serif;
    font-size: 16px;
}

section {
    background-color: white;
    border-radius: 10px;
    padding: 40px;
    margin-bottom: 10px;
}

.wrapper {
    width: 85%;
    margin: 20px auto;
}

h1 {
    display: none;  /*h1 보이지 않게 처리*/
}

h2, h3 {
    font-family: sans-serif;
}

h2 {
    margin: 0 0 20px 0;
    text-transform: uppercase;
    font-size: 18px;
}

#my_info h2 {
    display: none;
}

#my_info img {
    width: 100px;
    height: auto;
    border-radius: 50px;
    margin-right: 40px;
}

table {
    display: inline-block;
    border-collapse: collapse;
    border-spacing: 0;
    vertical-align: top;
}

th {
    text-align: left;
    padding-right: 20px;
}

th, td {
    font-size: 12px;
}

#myname th {
    display: none;
}

#myname td {
    display: block;
    font-size: 18px;
    font-weight: bold;
    margin-bottom: 10px;
}

a {
    color:inherit;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
    color: gold;
}

ul {
    list-style: none;
    padding: 0;
}

ul li {
    margin-bottom: 4px;
}

ul li::before {
    display: inline-block;
    width: 20px;
    height: 20px;
    vertical-align: middle;
    margin-right: 10px;
}

ul li:nth-child(1)::before {
    content: url('../images/ico_mobile.png');
}
ul li:nth-child(2)::before {
    content: url('../images/ico_insta.png');
}
ul li:nth-child(3)::before {
    content: url('../images/ico_github.png');
}

#skill ol {
    list-style: none;
    padding: 0;
}

#skill li {
    display: inline-block;
    background-color: gold;
    padding: 4px 10px;
    border-radius: 32px;
    margin: 0 8px 8px 0;
}

#skill li::before {
    content: "#";
}

#project ol {
    list-style: none;
    padding: 0;
}

#project li {
    border-bottom: 1px solid #ddd;
    padding-bottom: 20px;
}

#project li:last-child {
    border-bottom: none;
}

#project video {
    width: 100px;
}

#project a {
    color: gold;
    display: inline-block;
    border-radius: 4px;
    padding: 2px 8px 2px 0;
}

#project a:hover {
    background-color: #2f2f2f;
    text-decoration: none;
    padding: 2px 8px;
    transition: padding 0.2s;
}
