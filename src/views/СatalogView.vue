<template>
	<div class="about">
		<h1> Каталог товаров</h1>
	</div>
	<div class="content-catalog">
		<div v-for="p in pictures" :key="p.id" class="catalog-block">
			<div class="name">{{ p.title }}</div>
			<div class="image-block">
				<img :src="`/image/${p.image}`">
			</div>
			<div class="buttons">
				<span class="button">BN{{p.price}}</span>
				<span class="button">${{p.price*3}}</span>
				<span class="button">RUB{{p.price*2}}</span>
			</div>
			<!-- <p> {{p.price}}</p>
			<p>$ {{p.price*3}}</p>
			<p>RUB {{p.price*2}}</p> -->
		</div>
		<!-- <div class="catalog-block">
			<div class="name"> Баба Яга </div>
			<div class="image-block">
				<img src="/image/Баба Яга.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Перун </div>
			<div class="image-block">
				<img src="/image/Перун.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Русалки </div>
			<div class="image-block">
				<img src="/image/русалки.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Мавка </div>
			<div class="image-block">
				<img src="/image/Мавка.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Кикимора </div>
			<div class="image-block">
				<img src="/image/кикимора болотная.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Полудница </div>
			<div class="image-block">
				<img src="/image/Полудница.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Полуночница</div>
			<div class="image-block">
				<img src="/image/Полуночница.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name">Lorem Ipsum</div>
			<div class="text-block">
				<div class="button-block-fly"><button>Button</button></div>
				<div class="text">
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut dignissim lobortis nibh nec
					porttitor. Sed finibus leo nec hendrerit faucibus. Aliquam eleifend efficitur orci non
					ornare.
					Etiam commodo arcu eu lacinia fringilla. Cras tincidunt sed leo eu iaculis. Fusce ac
					lorem
					sit
					amet odio finibus eleifend dignissim eget felis. Suspendisse potenti.

					Proin ac feugiat sem. Class aptent taciti sociosqu ad litora torquent per conubia
					nostra,
					per
					inceptos himenaeos. Proin mattis maximus ultrices. Etiam in faucibus tellus. Praesent
					mattis
					sapien tortor, ac mollis libero tempor ut. Donec rutrum sem eu placerat convallis.
					Aenean
					commodo eleifend posuere.

					Mauris malesuada vehicula rhoncus. Suspendisse aliquet massa et massa semper feugiat.
					Vestibulum
					nec dolor risus. Etiam et nisi ut justo tincidunt cursus. Nullam luctus aliquam ligula,
					nec
					tincidunt arcu ullamcorper eget. Aliquam ac arcu erat. Nam ac nulla purus. In bibendum
					efficitur
					turpis id elementum. Nunc cursus bibendum nulla, eu tristique eros placerat non.
					Suspendisse
					rhoncus condimentum tempor. Pellentesque vitae nunc vel ipsum interdum lacinia et a
					velit.
					Mauris neque purus, sodales ut mollis vel, pulvinar vel massa. Pellentesque tempor id ex
					a
					gravida.

					Quisque ornare, lorem ut pretium gravida, ligula lacus cursus lacus, id sodales nulla
					tortor
					vel
					nisi. Integer tortor libero, eleifend et malesuada ac, vestibulum et erat. Sed a urna
					maximus,
					egestas mi sed, ultrices mi. Proin sed tortor et massa convallis rhoncus sed quis arcu.
					Morbi
					congue blandit elit posuere posuere. Sed euismod egestas nisi at tincidunt. Phasellus ut
					eros
					eget diam interdum tristique a eu mauris.

					Quisque fringilla tempor urna, sed viverra massa condimentum quis. Donec ut feugiat
					nulla.
					Fusce
					ac neque ut tellus vestibulum sollicitudin. Phasellus quis dictum dolor, a ornare
					turpis.
					Mauris
					at diam et metus lobortis condimentum. Class aptent taciti sociosqu ad litora torquent
					per
					conubia nostra, per inceptos himenaeos. Aliquam lobortis odio eu leo congue, ac sagittis
					dolor
					lacinia. In a leo tortor. Proin porta neque sit amet cursus eleifend. In in dolor arcu.
				</div>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Лесной дух</div>
			<div class="image-block">
				<img src="/image/Дух.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Мировое дерево </div>
			<div class="image-block">
				<img src="/image/drevo.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>
		</div>
		<div class="catalog-block">
			<div class="name"> Леший </div>
			<div class="image-block">
				<img src="/image/Леший.jpg">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>

		</div>
		<div class="catalog-block">
			<div class="name"> Дерево </div>
			<div class="image-block">
				<img src="/image/drevo.png">
			</div>
			<div class="buttons">
				<span class="button">button1</span>
				<span class="button">button2</span>
				<span class="button">button3</span>
			</div>

		</div> -->
	</div>
</template>

<script setup>
import sourceData from '@/BlockCatalog.json'
const pictures = sourceData.Catalog;
// const pictures = [
// {id: 1, image: "Велес.jpg", title: "Велес"},
// {id: 2, image: "Баба Яга.jpg", title: "Баба Яга"},
// {id: 3, image: "Перун.jpg", title: "Перун"},
// {id: 4, image: "русалки.jpg", title: "Русалки"},
// {id: 5, image: "Мавка.jpg", title: "Мавка"},
// {id: 6, image: "кикимора болотная.jpg", title: "Кикимора"},

// {id: 7, image: "Полудница.jpg", title: "Полудница"},
// {id: 8, image: "Полуночница.jpg", title: "Полуночница"},
// {id: 9, image: "Дух.jpg", title: "Лесной дух"},
// {id: 10, image: "drevo.jpg", title: "Мировое дерево"},
// {id: 11, image: "Леший.jpg", title: "Леший"},
// {id: 12, image: "drevo.png", title: "Дерево"},
// ];
</script>