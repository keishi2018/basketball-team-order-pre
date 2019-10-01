<template>
<footer>
	<div class="footer-inner">
			<div class="top-back">
				<div class="top-back-inner">
				<a href=""><img src="@/assets/y-top.svg" alt=""></a>
			</div>
		</div>

		<div class="sns-icon">
			<div class="sns-icon-inner">
				<a href=""><img src="@/assets/instagram.svg" alt=""></a>
				<a href=""><img src="@/assets/facebook.svg" alt=""></a>
				<a href=""><img src="@/assets/twitter.svg" alt=""></a>
			</div>
		</div>

		<div class="footer-menu">
			<div class="footer-menu-inner">
				<div id="footer-about"><p>ABOUT AKTR</p></div>
				<div id="footer-shop"><p>取扱店舗</p></div>
				<div id="footer-news"><p>NEWS</p></div>
				<div id="footer-my"><p>MYページ</p></div>
			</div>
		</div>

		<div class="footer-info">
			<div class="footer-info-inner">
				<p>会員登録</p>
				<p>利用ガイド</p>
				<p>Q&A</p>
				<p>特定商取引法に基づく表記</p>
				<p>支払い方法</p>
				<p>プライバシーポリシー</p>
				<p>利用規約</p>
				<p>お問い合わせ</p>
			</div>
		</div>

		<div class="copyright">
			copyright (c) AKTR all rights reserved.
		</div>
	</div>
</footer>
</template>


<style>
footer{
	background-color: black;
}

.top-back-inner{

}

.top-back{
	display: flex;
	justify-content: center;
	padding: 23px 0px;
}

.sns-icon{
	border-top: 1px solid #808080;
}

.sns-icon-inner{
	display: flex;
	justify-content: space-around;
	align-items: center;
	width: 200px;
	margin: 0 auto;
	padding: 25px 0px;
}

.sns-icon img{
	height: 20px;
}

.footer-menu{
	border-top: 1px solid #808080;
}
.footer-menu-inner{
	display: flex;
	justify-content: center;
	align-items: center;
	color: white;
	font-size: 12px;
}

.footer-menu-inner p{
	margin-bottom: 0;
}

#footer-about,#footer-shop,#footer-news,#footer-my{
	text-align: center;
	height: 75px;
	width: 320px;
	display: flex;
	justify-content: center;
	align-items: center;
}

#footer-shop{
	border-left: 1px solid #808080;
	border-right: 1px solid #808080;
}

#footer-news{
	border-right: 1px solid #808080;
}

.footer-info{
	border-top: 1px solid #808080;
}

.footer-info-inner{
	display: flex;
	justify-content: space-around;
	align-items: center;
	color: white;
	font-size: 12px;
	width: 800px;
	margin: 0 auto;
	padding: 30px 0px;
}

.footer-info-inner p{
	margin-bottom: 0;
}

.copyright{
	text-align: center;
	color: white;
	font-size: 12px;
	padding-bottom: 30px;
}


</style>