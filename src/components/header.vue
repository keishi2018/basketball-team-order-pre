<template>
    <header>
            <div class="header-top">
                <div class="header-top-icon-left"><img alt="" src="@/assets/info-i.svg" ></div>
                <p>冬期休暇のお知らせ</p><img src="@/assets/y-under.svg" alt="">
            </div>
            <div class="header-under">
                <p class="hm-menu"><a href=""><img src="@/assets/hm.png" alt=""></a></p>
                <h1 class="main-logo"><a href=""><img src="@/assets/header-logo.png" alt="logo"></a></h1>
                <nav class="hd-sarch">
                        <ul>
                            <li><a href=""><img src="@/assets/magnify.svg" alt=""></a></li>
                            <li><a href=""><img src="@/assets/cart.svg" alt=""></a></li>
                        </ul>
                </nav>
            </div>
    </header>
</template>

<style>

header{
	background-color: white;
	position: fixed;
	width: 100%;
	filter: drop-shadow(0px 0px 5px rgba(0,0,0,0.5));
}

header .header-top{
	display: flex;
	justify-content: flex-start;
	align-items: center;
	height: 35px;
	background-color: black;
}

header .header-top p{
	font-size: 12px;
	color: #AD9978;
	margin-bottom: 0;
	padding-top: 3px;
	padding-left: 10px;
}

.header-top-icon-left img{
	height: 14px;
	padding-left: 10px;
}

.header-top-icon-right img{
	height: 8px;
	padding-left: 10px;
}

.header-under{
	background-color: white;
	display: flex;
	justify-content: space-between;
	align-items: center;
	width: 95%;
	margin: 0 auto;
}

header .main-logo{	
	width: 160px;
	padding-top: 18px;
	padding-bottom: 18px;
	margin-bottom: 0px;
}

header .main-logo h1{	

}

header .hm-menu{
	max-width: 20px;
}

header .hd-sarch ul{
	display: flex;
	justify-content: space-around;
	margin-bottom: 0;
	padding: 0;
}

header .hd-sarch ul li {
	list-style:none;
}

header .hd-sarch ul li a{
	padding-left: 12px;
}

header .hd-sarch img{
	height: 29px;
}
</style>