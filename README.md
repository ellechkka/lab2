<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<title>интернет магазин</title>
		
		<link rel="preconnect" href="https://fonts.googleapis.com">
		<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
		<link href="https://fonts.googleapis.com/css2?family=Comfortaa:wght@300&family=Nunito:wght@200&display=swap" rel="stylesheet">
		
		<style>
			* {
				margin: 0;
				box-sizing: border-box;
				font-family: Nunito;
				

				/* background-color: #fffce1; */
			}
			li {
				list-style-type: none;
			}
			
			
			header {
				background-color: #fffce1;
				width: 100%; 
				display: inline-block;
			}
			.header-logo {
				display: block;
				float: left;
				padding: 5px;
			}

			.bar {
				margin: 0;
			}
			
            .bar ul {
				display: flex;
				flex-flow: row nowrap;
				align-items: center;
				align-content: space-between;
				justify-content: space-between;
				margin-right: 30px;
			}
			.bar li {
				display: inline; 
				float: right;
			}
			#searchform {
				display: inline;
			    float: left;
			    margin-left: 40px;
			}
			#searchform input {
				background-color: #fffce1;
			    width: 250px;
			    float: left;
			    border: none;
			    padding-left: 12px;
			    height: 40px;
			    overflow: hidden;
			    outline: none;
			    color: #462b12;
			}
			#searchform button {
				background: transparent;
				height: 40px;
				border: none;
				right: 5px;
				color: #fffce1;
				cursor: pointer;
				font-size: 18px;
				margin-right: 30px;
			}
			
			
			nav {
				margin: 0;
				background-color: #fffce1;
			}
			nav li {
				align-items: center;
				width: 100%;
			}
			nav ul {
				display: flex;
				flex-flow: row nowrap;
				align-items: center;
				align-content: space-between;
				justify-content: space-between;
			}
			nav a {
				color: #42675b;
				text-decoration: none;
			}
			nav a:visited {
				color: #42675b;
				text-decoration: none;
			}
			nav a:active {
				color: #42675b;
				text-decoration: underline;
			}
			
			
			main {
				background-color: #fffce1;
				padding: 20px;
			}
			h1 {
				margin-left: 20px;
				font-size: 36px;
			}
			.filter {
				float: left;
				width: 20%;
				margin-top: 18px;
			}
			.filter il {
				text-decoration: none;
				color: #fffce1;
			}
			.filter a {
				color: black;
				text-decoration: none;
			}
			.filter a:visited {
				color: black;
				text-decoration: none;
			}
			.filter a:active {
				color: #dba774;
				text-decoration: underline;
			}
			.items {
				float: left;
				width: 80%;
			}
			.items p {
				text-align: center;
				padding: 5px;
				color: black;
			}
			h6 {
				font-family: Nunito;
				font-size: 20px;
				text-align: center;
				margin: 7px;
				color: black;
			}
			.items button {
				position: relative;
				left: 50%;
				transform: translate(-50%, 0);
				background-color: #c3d9bb;
			}
			
			.product-wrapper {
				display: block;
				width: 100%;
				float: left;
				transition: width .2s;
			}
			@media only screen and (min-width: 620px) {
				* {
					font-size:16px;
				}
				.product-wrapper {
					width: 50%;
				}
			}
			@media only screen and (min-width: 1000px) {
				* {
					font-size: 20px;
				}
				.product-wrapper {
					width: 33.333%;
				}
			}

			
			.product {
				display: block;
				position: relative;
				background: #fffce1;
				margin: 0 20px 20px 0;
				text-decoration: none;
				z-index: 0;
				height: 460px;
			}
			.product-photo {
				position: relative;
				padding-bottom: 100%;
				overflow: hidden;
			}
			.product-photo img {
				position: absolute;
				top: 0;
				bottom: 0;
				left: 0;
				right: 0;
				max-width: 80%;
				max-height: 80%;
				margin: auto;
				transition: transform .4s ease-out;
				border: 1px solid #462b12;
				border-radius: 3px;
			}
			
			.row:after {
				content: "";
				display: table;
				clear: both;
				padding: 20px;
			}
			
			
			footer {
				background-color: #462b12;
				color: #fffce1;
			}
			footer li {
				color: #fffce1;
				margin: 20px;
			}
			footer ul {
				display: flex;
				flex-flow: row nowrap;
				align-items: center;
				align-content: space-between;
				justify-content: space-between;
			}
			footer a {
				color: #fffce1;
				text-decoration: none;
			}
			footer a:visited {
				color: #fffce1;
				text-decoration: none;
			}
			footer a:active {
				color: #fffce1;
				text-decoration: underline;
			}
			
		</style>
	</head>
	
	<body>
		<header>
			<div class="bar">
				<ul>
                    <li>
                        <div class="header-logo">
                            <img src="https://i.ibb.co/bW6L4zg/image.png" height="75px">
                        </div>
                    </li>
					<li>
						<form action="" method="get" id="searchform">
							<input type="text" placeholder="Искать на сайте">
							<button type="submit">
								<img src="https://cdn-icons-png.flaticon.com/512/622/622669.png" height="24px">
							</button>
						</form>
					</li>
					<li><a href=""><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="30px"></a></li>
					<li><a href=""><img src="https://cdn-icons-png.flaticon.com/512/1077/1077035.png" width="30px"></a></li>
					<li><a href=""><img src="https://cdn-icons-png.flaticon.com/512/1077/1077063.png" width="30px"></a></li>
				</ul>
			</div>
		</header>
		
		<nav>
			<hr>
			<ul>
				<li><a href="">Главная страница</a></li>
				<li><a href="">О магазине</a></li>
				<li><a href="">Каталог</a></li>
				<li><a href="">Контакты</a></li>
				<li><a href="">Вакансии</a></li>
			</ul>
			<hr>
		</nav>
		
		<main>
			<h1>Каталог</h1>
			<div class="row">
				<div class="filter">
					<ul>
						<li><a href="">Декор</a></li>
						<li><a href="">Диваны</a></li>
						<li><a href="">Ковры</a></li>
						<li><a href="">Освещение</a></li>
						<li><a href="">Столы</a></li>
						<li><a href="">Стулья</a></li>
						<li><a href="">Тумбочки</a></li>
						<li><a href="">Шкафы</a></li>
					</ul>
				</div>
				<div class="items">
					<ul class="products clearfix">
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/holmsund-3-mestnyy-divan-krovat-nordvalla-svetlo-zelenyy__0973704_pe812111_s5.jpg?f=xl">
								</div>
								<h6>Диван</h6>
								<p>3-местный диван-кровать</p>
								<p>39 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/landskrona-landskruna-2-mestnyy-divan-grann-bumstad-belyy-bereza__0320975_pe514793_s5.jpg?f=xxs">
								</div>
								<h6>Диван</h6>
								<p>2-местный диван из кожи</p>
								<p>49 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/knopparp-2-mestnyy-divan-knisa-svetlo-seryy__0713943_pe729858_s5.jpg?f=xxs">
								</div>
								<h6>Диван</h6>
								<p>2-местный диван</p>
								<p>8 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/landskrona-landskruna-2-mestnyy-divan-gunnared-svetlo-zelenyy-derevo__0602106_pe680175_s5.jpg?f=xxs">
								</div>
								<h6>Диван</h6>
								<p>2-местный диван</p>
								<p>35 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/strandmon-kreslo-s-podgolovnikom-shiftebu-bezhevyy__0641725_pe700622_s5.jpg?f=xxs">
								</div>
								<h6>Кресло</h6>
								<p>Кресло с подголовником</p>
								<p>13 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/landskrona-landskruna-kreslo-gunnared-temno-seryy-derevo__0602087_pe680155_s5.jpg?f=xxs">
								</div>
								<h6>Кресло</h6>
								<p>Кресло серое</p>
								<p>24 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/vonsbaek-vonsbek-kover-korotkiy-vors-zelenyy__0717879_pe731373_s5.jpg?f=xxs">
								</div>
								<h6>Ковер</h6>
								<p>Ковер, короткий ворс, 170x230 см</p>
								<p>5 499  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/loevbacken-lyovbakken-pridivannyy-stolik-klassicheskiy-korichnevyy__0173699_pe327848_s5.jpg?f=xxs">
								</div>
								<h6>Столик</h6>
								<p>Придиванный столик</p>
								<p>4 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/micke-mikke-pismennyy-stol-belyy__0736020_pe740347_s5.jpg?f=xxs">
								</div>
								<h6>Стол</h6>
								<p>Письменный стол, 42x50 см</p>
								<p>6 499  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/ingatorp-ingolf-ingolf-stol-i-4-stula-belyy-belyy__0954402_pe803271_s5.jpg?f=xxs">
								</div>
								<h6>Стол и 4 стула</h6>
								<p>Стол и 4 стула, 110/155 см</p>
								<p>37 195  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/nordviken-nordviken-nordviken-stol-i-6-stulev-morilka-antik-morilka-antik__0941068_pe795325_s5.jpg?f=xxs">
								</div>
								<h6>Стол и 6 стульев</h6>
								<p>Стол и 6 стульев, 152/223x95 см</p>
								<p>42 793  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/ingolf-stul-belyy__0728152_pe736113_s5.jpg?f=xxs">
								</div>
								<h6>Стул</h6>
								<p>Стул, белый</p>
								<p>3 799  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/fanbyn-fanbyun-stul-belyy-d-doma-ulicy__0545007_pe655282_s5.jpg?f=s">
								</div>
								<h6>Стул</h6>
								<p>Стул, белый</p>
								<p>4 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/trubbnate-tryubbnate-abazhur-dlya-podvesn-svetilnika-belyy__0946582_pe798151_s5.jpg?f=xxs">
								</div>
								<h6>Абажур</h6>
								<p>Абажур для подвесн светильника, 38 см</p>
								<p>799  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/brunsta-bryunsta-abazhur-dlya-podvesn-svetilnika-chernyy__0683764_pe720856_s5.jpg?f=xxs">
								</div>
								<h6>Абажур</h6>
								<p>Абажур для подвесн светильника, 20 см</p>
								<p>999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/skottorp-skaftet-skaftet-lampa-nastolnaya-seryy-nikelirovannyy__0859370_pe780897_s5.jpg?f=xxs">
								</div>
								<h6>Лампа</h6>
								<p>Лампа настольная</p>
								<p>1 099  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/nordkisa-nordkiza-tumba-prikrovatnaya-bambuk__0786399_pe762976_s5.jpg?f=xxs">
								</div>
								<h6>Тумбочка</h6>
								<p>Тумба прикроватная, 40x40 см</p>
								<p>5 499  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/nikkeby-nikkebi-komod-s-2-yashchikami-sero-zelenyy__0729042_pe738505_s5.jpg?f=xxs">
								</div>
								<h6>Тумбочка</h6>
								<p>Комод с 2 ящиками, 46x70 см</p>
								<p>4 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/sundvik-shkaf-platyanoy-belyy__0626568_pe692872_s5.jpg?f=xxs">
								</div>
								<h6>Шкаф</h6>
								<p>Шкаф платяной, 80x50x171 см</p>
								<p>14 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/rakkestad-garderob-3-dvernyy-cherno-korichnevyy__0823987_pe776018_s5.jpg?f=xxs">
								</div>
								<h6>Шкаф</h6>
								<p>Гардероб 3-дверный, 117x176 см</p>
								<p>8 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/pax-paks-grimo-grimo-garderob-kombinaciya-belyy-belyy__0780624_pe760134_s5.jpg?f=xxs">
								</div>
								<h6>Шкаф</h6>
								<p>Гардероб, комбинация, 100x60x236 см</p>
								<p>29 950  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/tordh-turd-stellazh-d-sada-korichnevaya-morilka__0763283_pe752524_s5.jpg?f=xxs">
								</div>
								<h6>Стеллаж</h6>
								<p>Стеллаж, 70x35x161 см</p>
								<p>5 000  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/dypsis-lutescens-dipsis-zheltovatyy-rastenie-v-gorshke-hrizalidokarpus-zheltovatyy__0653973_pe708202_s5.jpg?f=xxs">
								</div>
								<h6>Растение</h6>
								<p>Растение в горшке, Хризалидокарпус, 24 см</p>
								<p>2 999  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
						<li class="product-wrapper">
							<a href="" class="product">
								<div class="product-photo">
									<img src="https://www.ikea.com/ru/ru/images/products/vaeldoft-veldoft-aromaticheskaya-svecha-v-stakane-utrennyaya-rosa-svetlo-zelenyy__0797192_pe767287_s5.jpg?f=xxs">
								</div>
								<h6>Свечка</h6>
								<p>Ароматическая свеча в стакане, 8 см</p>
								<p>99  ₽</p>
								<button><img src="https://cdn-icons.flaticon.com/png/512/3002/premium/3002240.png?token=exp=1633797775~hmac=2b8ec015682a1c9c88e0d16a81451fe3" width="24px"> Добавить в корзину</button>
							</a>
						</li>
					</ul>
				
				</div>
			</div>
			
		</main>
		
		
		<footer>
			<ul>
				<li><a href="">Главная страница</a></li>
				<li><a href="">О магазине</a></li>
				<li><a href="">Контакты</a></li>
				<li><a href="">Вакансии</a></li>
			</ul>
			<img src="https://i.ibb.co/SdCsVhV/image.png" width="100%">	
		</footer>
	
	</body>
</html>
