<script>
  let items = [
    {
      img: "assets/01.png",
	  title: "Bewe base",
	  price:"20",
      desc:
        "Software base de BEWE. Todo lo necesario para gestionar tu negocio aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa .",
    },
    {
      img: "assets/02.png",
	  title: "Bewe Pass",
	  price:"40",
      desc:
        "Software base de BEWE. Todo lo necesario para gestionar tu negocio.",
    },
    {
      img: "assets/03.png",
	  title: "Bewe Class",
	  price:"20",	  
      desc:
        "Software base de BEWE. Incluye una agenda y todo lo necesario para gestionar tu negocio.",
    },
    {
      img: "assets/04.png",
	  title: "Bewe Pay +",
	  price:"20",	  
      desc:
        "Software base de BEWE. Incluye una agenda y todo lo necesario para gestionar tu negocio.",
    },
    {
      img: "assets/04.png",
	  title: "Periodo de pago",
	  price:"20",	  
      desc:
        "Elige la periodicidad de pago que prefieras. A más meses, mayor será el descuento.",
    },
  ];
</script>

<main>
  <section class="pricing-container">
    {#each items as { img, title, desc, price }}
      <div class="item">
        <div class="item__info">
          <div class="item__info__image">
            <img src={img} alt="" />
          </div>
          <div class="item__info__text">
			<p class="text__title">{title}</p>
			<p class="text__desc">{desc}</p>
          </div>       
        </div>
        <div class="item__select">
			<select name="" placeholder="Empleado" id="">
				<option value="1">1</option>
				<option value="2">2</option>
			</select>
		</div>
        <div class="item__price"> 
			<p class="item__price_title"></p>
			$ {price}/mes
		</div>
      </div>
	{/each}
	<div class="summary bg-primary">
		<div class="summary__total">Total</div>
		<div class="summary__date">
			<span class="color-red line-thru">$ 40/mes</span>
			<span>$20 /mes</span>
		</div>
	</div>
	<div class="cta">
		<button class="cta__btn">Comprar</button>
	</div>
  </section>
</main>

<style>
</style>
