# 2022-05-17practice


<html>

<head>
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<link rel="stylesheet" type="text/css" href="./css/header.css">
	<link rel="stylesheet" type="text/css" href="./css/figure.css">
	<link rel="stylesheet" type="text/css" href="./css/metadata-block.css">
	<link rel="stylesheet" type="text/css" href="./css/toolbox-block.css">
	<link rel="stylesheet" type="text/css" href="./css/infobox.css">

	<!-- 清除瀏覽器預設的風格 -->
	<link rel="stylesheet" type="text/css" href="https://meyerweb.com/eric/tools/css/reset/reset200802.css">

	<!-- 載入思源黑體 -->
	<link
		href="https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@400;700&family=Roboto:wght@400;700&display=swap"
		rel="stylesheet">

	<!--載入bootstrap的css css要在head裡面-->
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet"
		integrity="sha384-0evHe/X+R7YkIZDRvuzKMRqM+OrBnVFBL6DOitfPri4tjfHxaWutUpFmBp4vmVor" crossorigin="anonymous">

	<style>
		* {
			box-sizing: border-box;
		}

		body {
			font-family: 'Roboto', 'Noto Sans TC', sans-serif;
			background-color: #fff;
			margin: 0;
		}

		a {
			font-size: 16px;
			line-height: 38px;
			text-decoration-line: none;
			border-bottom: 1px solid #A67A44;
			padding-bottom: 2px;
			color: #A67A44;
		}

		.mobile-block {
			max-width: 375px;
			width: 100%;
			background-color: #F1F1F1;
		}

		.w-300 {
			width: calc(300/375*100%);
		}

		.title {
			font-weight: bold;
			font-size: 34px;
			line-height: 50px;
			width: calc(326/375*100%);
			margin-bottom: 30px;
		}

		.sub-title {
			font-weight: bold;
			font-size: 16px;
			line-height: 24px;
			color: #000000;
			margin-bottom: 30px;
			margin-top: 10px;
			width: calc(326/375*100%);
		}

		.block-horizontal-center {
			margin-right: auto;
			margin-left: auto;
		}

		.para-text {
			font-size: 18px;
			line-height: 38px;
			color: #404040;
			margin-bottom: 40px;
			margin-top: 40px;
		}

		/* 為Bootstrap Carousel 增加風格 限制bootstrap 的slideshow的高度，讓圖片高度一致*/

		.carousel img {
			height: 250px;
			object-fit: cover;
			/*使圖片塞進框中，多餘的瀏覽器會裁切*/

		}

		/*調整示意圓點的位置*/
		.carousel-indicators {
			margin-bottom: -20px;
		}

		/*有[data-bs-target]標籤的，
		會是整個程式中權重最重的；
		所以在此需要這樣打以覆蓋掉原本的[data-bs-target]裡面的數值，
		不然蓋不掉*/

		.carousel-indicators [data-bs-target] {
			width: 10px;
			height: 10px;
			border-radius: 50%;
			border: 1px solid black;

		}

		.carousel-indicators [data-bs-target].active {
			background-color: black;
		}

		/*做出下來後的內容*/
		.annotation{
			background-color: white;
			padding-top:15ps;
			padding-bottom:20px;
		}

		.annotation-body{
			width:300px;
			margin-left:auto;
			margin-right:auto;
			font-size:20px;
			line-height:40px;
		}


		[data-bs-toggle="collapse"][aria-expanded="false"]{
			transform:rotate(0deg);
			transition-property:transform;
			transition-duration:0.3s;
			transition-timing-function: ease-in-out;
		}


		[data-bs-toggle="collapse"][aria-expanded="true"]{
			transform:rotate(90deg);
			transition-property:transform;
			transition-duration:0.3s;
			transition-timing-function: ease-in-out;
		}

		#ham-block{
			height:100%;
			width:200px;
			background-color: aliceblue;

		}
	</style>
</head>

<body>
	<!-- mobile version start -->


	<div class="mobile-block">
		<!-- header -->
		<div id="header">
			<div class="logo">
				<img src="./assets/icons/twreporter-logo.svg" width="100%">
			</div>

			<div class="ham"
			data-bs-toggle="collapse" 
			href="#ham-block" 
			aria-expanded="false" 
			aria-controls="ham-block"
			>

				<div></div>
				<div></div>
				<div></div>
			</div>
		</div>

		<!-- subtitle -->
		<h2 class="sub-title block-horizontal-center">Reporter Saturday Features</h2>

		<!-- title -->
		<h1 class="title block-horizontal-center">【山思而行】登山中的死亡，對生命的凝視</h1>

		<!-- hero image-->
		<figure class="mobile">
			<img src="./assets/images/image-1.jpg">
			<figcaption class="mobile-hero">
				登上山峰之途，就是在死亡的陰影之下，動用自身全部的感官與技藝，設法避開那些遭致危機的陷阱。圖為2016年2月，一支國際登山隊正跨越珠穆朗瑪峰基地營附近的冰川。（Photo by Jerry Zhang on
				Unsplash）
			</figcaption>
		</figure>

		<!-- metadata-->
		<div class="metadata-block w-300 block-horizontal-center" style="margin-top: 50px;">
			<div class="top-separation"></div>
			<div class="category" style="margin-bottom: 15px;">環境．教育</div>
			<div class="top-separation"></div>
			<div class="pubdate" style="margin-bottom: 15px;">刊出日期 2020/2/28</div>
			<div class="author-block" style="margin-bottom: 45px;">文字 ／
				<a class="author-text" href="https://www.twreporter.org/authors/5d8b2d8035544318001f9255"
					target="_blank">張元植</a>
			</div>
			<div class="tag-bt">#體育</div>
			<div class="tag-bt">#山思而行</div>
			<div class="bottom-separation"></div>
		</div>

		<!-- tool box -->
		<div class="w-300 toolbox-block block-horizontal-center" style="margin-top: 25px;">
			<img src="./assets/icons/add-bookmark.svg" width="30px">
			<img src="./assets/icons/tool-text.svg" width="30px">
			<img src="./assets/icons/tool-print.svg" width="30px">
			<img src="./assets/icons/share-fb.svg" width="30px">
			<img src="./assets/icons/share-twitter.svg" width="30px">
			<img src="./assets/icons/share-line.svg" width="30px">
		</div>

		<!-- content -->
		<p class="w-300 block-horizontal-center para-text">
			講到登山，普遍的印象可能是壯闊的山景，雲海朝霞萬丈金芒；也可能是山上人與人之間的情誼，過地形時伸手扶一把，或濕冷雨天一碗熱呼呼的泡麵。我們在山中感受生命各種美好，汲取養分。就算是逆境，痛苦會過去，美會留下，回到人間後依舊能量滿滿再度出發。
		</p>
		<p class="w-300 block-horizontal-center para-text">
			做為人，不知為何，我們傾向記憶美好，卻遺忘過程的苦痛。但我卻想，這是否讓我們理解、記憶一件事情性質的方式，也隨之產生偏誤？
		</p>

		<p class="w-300 block-horizontal-center para-text">我想說的是，登山是件會死人的運動。

			<img data-bs-toggle="collapse" 
			href="#collapseExample" 
			aria-expanded="false" 
			aria-controls="collapseExample"  	 
			src="./assets/icons/abbreviations.svg">
			<!-- 
			這串是要做出點擊後可以下滑內容的按鈕
			從data-bs-toggle開始一串都是bootstrap的JS需要啟動collapse功能所需要的
			最下方的是img src是按扭的圖片
			可以注意到aria-controls後面接的是一個id叫做collapseExample，而在此指的是下方物件的id-->
		
		</p>

		<div class="collapse annotation" id="collapseExample">
			<div class="annotation-body">
				某程度上，登上山巔之途，就是在死亡的陰影之下，動用自身全部的感官與技藝，設法避開那些遭致危機的陷阱。這樣的經驗本身，就是一種回報，高處的風景與抵達最高點的滿足，則是額外的嘉獎。
			</div>
		</div>

		<p class="w-300 block-horizontal-center para-text">
			那是個風和日麗的早晨，我跟阿果從標高5,600公尺的馬卡魯峰前進基地營帳篷中醒來。我倆前一天剛攀升至7,150公尺處進行適應攀登並下山，往後一週將是一系列壞天氣週期的到來，所以我們正準備迎接休息日的放鬆作息。
		</p>
		<!-- slidshow / carousel-->

		<div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="false" data-bs-touch="false"
			data-bs-interval="false">
			<div class="carousel-indicators">
				<button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"
					aria-current="true" aria-label="Slide 1"></button>
				<button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
					aria-label="Slide 2"></button>
				<button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"
					aria-label="Slide 3"></button>
			</div>
			<div class="carousel-inner">
				<div class="carousel-item active">
					<img src="./assets/images/image-3.jpg" class="d-block w-100" alt="img3">
				</div>
				<div class="carousel-item">
					<img src="./assets/images/image-5.jpg" class="d-block w-100" alt="img5">
				</div>
				<div class="carousel-item">
					<img src="./assets/images/image-4.jpg" class="d-block w-100" alt="img4">
				</div>
			</div>
			<button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators"
				data-bs-slide="prev">
				<span class="carousel-control-prev-icon" aria-hidden="true"></span>
				<span class="visually-hidden">Previous</span>
			</button>
			<button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators"
				data-bs-slide="next">
				<span class="carousel-control-next-icon" aria-hidden="true"></span>
				<span class="visually-hidden">Next</span>
			</button>
		</div>

		<!-- slidshow / carousel 結束 -->

		<p class="w-300 block-horizontal-center para-text">
			慢慢踱進餐廳帳，吃完千篇一律的鬆餅加煎蛋，正想放個音樂泡杯咖啡，這時外面有人叫我。是Lakpa。</p>
		<p class="w-300 block-horizontal-center para-text">Lakpa是隔壁營區的商業團"Pioneer
			Adventure"的老闆，今年除了我跟阿果，馬卡魯峰這裡還有同樣來自台灣的登山者<a href="">三條魚</a>，她就在這個隊伍中。
		</p>
		<figure class="mobile" style="margin-top:50px; margin-bottom: 50px;">
			<img src="./assets/images/image-2.jpg">
			<figcaption class="mobile">2017年3月，一隊登山者朝向尼泊爾羅布崎的登山營地前進。（Photo by Marco Bonomo on Unsplash）
			</figcaption>
		</figure>
		<div class="infobox-block w-300 block-horizontal-center">
			<h3 class="infobox-title">作者簡介／張元植</h3>
			<p class="infobox-content">
				生命與山交纏18載，如今已切分不開。從台灣百岳健行，到中級山探勘；高海拔遠征登山，到冰岩技術攀登。涉獵廣泛但都不精，只願打開更多與山對話的可能性，更自由的在山中遊走。</p>
			<p class="infobox-content">每當自問為何登山、山是什麼？總覺面貌多重不清。有時是異域、是試煉自身的標尺；又或是鄉愁、生活的場域。</p>
			<p class="infobox-content">
				13歲接觸登山，至今行過百岳60餘，21歲完成中央山脈大縱走。15歲初涉海外，登頂北美最高峰丹奈利；18歲攀登阿空加瓜，為台灣最年輕的南美最高峰登頂者；25歲登上人生第一座8千公尺——布羅德峰；30歲嘗試攀登K2，未竟。至今累積近20座海外攀登經歷，海拔遍及4千至8千公尺。
			</p>
		</div>
	</div>
	<!-- mobile version end -->

	<!--載入bootstrap的JavaScipt JS在body裡面-->
	<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/js/bootstrap.bundle.min.js"
		integrity="sha384-pprn3073KE6tl6bjs2QrFaJGz5/SUsLqktiwsUTF55Jfv3qYSDhgCecCxMW52nD2"
		crossorigin="anonymous"></script>

</body>

</html>
