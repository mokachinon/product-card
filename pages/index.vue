<template>
  <div>
    <div class="body">
      <div class="container">
        <img src="~static/images/image-product-desktop.jpg" alt="img-product" class="card-img" />
        <div class="card-content">
          <p class="text">P E R F U M E</p>
          <h1 class="title">Gabrielle Essence Eau De Parfum</h1>
          <p class="text">A floral, solar and voluptuous interpretation composed by Olivier Polge,
            Perfumer-Creator for the House of CHANEL.</p>
          <div class="pricing">
            <h1 class="title">$149.99</h1>
            <p class="text disc">$169.99</p>
          </div>
          <button class="btn-cart">
            <img src="~static/images/icon-cart.svg" alt="icon" />
            <p class="btn">Add to Cart</p>
          </button>
        </div>
      </div>
    </div>
    <attribution />
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Fraunces&family=Montserrat&display=swap');

.body {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 50px;
}

.container {
  box-shadow: 0px 151px 60px rgba(0, 0, 0, 0.01), 0px 85px 51px rgba(0, 0, 0, 0.05), 0px 38px 38px rgba(0, 0, 0, 0.09), 0px 9px 21px rgba(0, 0, 0, 0.1), 0px 0px 0px rgba(0, 0, 0, 0.1);
  background-color: var(--white);
  width: 600px;
  height: 100%;
  border-radius: 10px;
  box-sizing: border-box;
  display: flex;
}

.card-img {
  width: 300px;
  height: 450px;
  border-radius: 10px 0px 0px 10px;
}

.card-content {
  display: grid;
  align-content: space-evenly;
  align-items: center;
  padding: 32px;
}

.pricing {
  display: flex;
  align-items: center;
  gap: 10px;
}

.title {
  font-weight: var(--fwBold);
  font-family: var(--ffFraunces);
}

p,
span {
  font-size: var(--forParagraph);
}

.text {
  color: var(--pureGrey)
}

.disc {
  text-decoration: line-through;
}

.btn-cart {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 236px;
  height: 48px;
  border: none;
  border-radius: 10px;
  background: var(--darkCyan);
  font-weight: var(--fwBold);
  color: var(--white);
  gap: 10px;
}


.btn-cart:hover {
  background: var(--veryDarkBlue);
  cursor: pointer;
  transition: 0.3s;
}


@media screen and (max-width: 375px) {
  .body {
    box-sizing: border-box;

  }

  .container {
    flex-direction: column;
    width: 343px;
    height: 611px;
  }

  .card-img {
    width: 343px;
    height: 240px;
    object-fit: cover;
    border-radius: 10px 10px 0px 0px;
  }

  .card-content {
    gap: 20px;
  }

  .pricing {
    display: flex;
    align-items: flex-end;
  }

  .btn-cart {
    width: 100%;
  }


}
</style>


