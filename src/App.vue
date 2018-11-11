<template>
  <div id="app">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
    <nav class="navbar navbar-dark navbar-expand-lg navbar-light" style="background-color: #1995E0;">
      <a class="navbar-brand" href="#">#あたしと新山詩織 プロジェクト</a>
      <button type="button" class="navbar-toggler" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item active">
            <a class="nav-link" href=""> <span class="sr-only">(current)</span>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#message">プロジェクトについて</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#tweet">ツイート</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#form">Webフォーム</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#letter">お手紙</a>
          </li>
        </ul>
      </div>
    </nav>
    
    <div id="backgroud">
      <!-- <img src="./assets/logo.png"> -->
      <div id="message">
        <strong><h1 id="about" style="color: #fff;"> {{ msg }}</h1></strong>
      </div>
      <div id="message">
        <h3>10月20日。突然の活動休止発表。</h3>
        <h3>今、応援しているファンができることはなにか。</h3><br>
      </div>
      <a class="twitter-timeline" data-width="900" data-height="500" href="https://twitter.com/atashito_shiori?ref_src=twsrc%5Etfw">Tweets by atashito_shiori</a>
      
      <div id="item">
        <h2 id="tweet" style="color: #fff;">新山詩織さんへの想いをツイートで共有しよう</h2>
      </div>
      <div class="btn btn-primary badge-pill" style="background-color: #1995E0;">
        <a href="https://twitter.com/intent/tweet?button_hashtag=あたしと新山詩織&ref_src=twsrc%5Etfw" data-show-count="false" style="color: white;">#あたしと新山詩織をツイートする</a><br>
      </div>
      <dir id="twtimeline">
        <a class="twitter-timeline form" data-lang="ja" data-width="500" data-height="900" href="https://twitter.com/atashito_shiori/likes?ref_src=twsrc%5Etfw">#あたしと新山詩織のツイート</a>
      </dir>    
      <div id="item">
        <h2 id="form" style="color: #fff;">Webフォームから想いを伝えてみよう</h2>
      </div>
      <a href="http://niiyama-shiori.com/message/index.html" class="btn btn-primary badge-pill" style="background-color: #1995E0;">メッセージを送る</a>
      <!-- <iframe class="100%" style="margin: 5px;
        transform-origin: 0 0;" 
        src="http://niiyama-shiori.com/message/index.html" 
        width="600" height="1200">
      </iframe> -->
      <div id="item">
        <h2 id="letter" style="color: #fff;">お手紙で想いを伝えてみよう</h2>
      </div>
      <div id="adress">
        <p>〒106-0032<br>
            東京都港区六本木５－２－２　トーマスビル<br>
          「新山詩織ファンレター」係<br>
        </p>
      </div>
      <footer class="footer footer-dark mt-auto py-3" style="background-color: #1995E0;">
        <div class="container">
          <a href="https://twitter.com/atashito_shiori" class="footer-font">お問い合わせはTwitterのDMまで</a>
        </div>
      </footer>
    </div>
  </div>
</template>

<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
<script>
export default {
  name: 'app',
  data () {
    return {
      msg: '#あたしと新山詩織 プロジェクト'
    }
  }
}
</script>

<style lang="scss">
// .collapse {
//   padding: 5%;
// }

#twButton{
  padding: 2%;
  font-size: 10%;
}

#message {
  padding: 5%;
  font-size: 10%;
}

#item {
  padding: 5%;
}

#adress {
  padding-bottom: 10%;
  display: block;
  text-align: center;
}

#adress p {
  text-align: left;
  display: inline-block;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#twtimeline{
  padding: 5%;
}

#backgroud{
  background-image: linear-gradient(-90deg, #1A55AD, #3DD2F0);
}

h1 {
  font-size: 100%;
  line-height: 200%;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

.list {
	position: relative;
	padding: 0;
	list-style-type: none;
  text-align: center;
}

.list ul {
  display: inline-block;
  text-align: left;
}

.list li {
	padding: 0.5em 0.5em 0.6em 0.5em;
	margin-bottom: 5px;
	line-height: 1.5;
	vertical-align: middle;
	background: #1995E0;
	border-radius: 20px 0px 0px 20px;
	color: #ffffff;
}

.list li::before {
	display:inline-block;
	vertical-align: middle;
	content:'';
	margin-right: 8px;
	width:1em;
	height: 1em;
	background: #fff;
	border-radius: 50%;
}
.footer-font{
  color: white;
}
</style>
