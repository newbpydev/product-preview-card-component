<!-- * SCRIPT -->
<script lang="ts">
  // your script goes here
  import src from "/images/image-product-mobile.jpg";
</script>

<!-- * TEMPLATE -->
<article class="product-card">
  <div class="product-card__img" alt="product image" role="img" />

  <section class="product-card__details">
    <h2 class="product-card__subtitle">Perfume</h2>
    <h1 class="product-card__title">Gabrielle Essence Eau De Parfum</h1>
    <p class="product-card__description">
      A floral, solar and voluptuous interpretation composed by Olivier Polge,
      Perfumer-Creator for the House of CHANEL.
    </p>
    <div class="product-card__price">
      <span class="product-card__price-after-discount">$149.99</span>
      <span class="product-card__price-before-discount">$169.99</span>
    </div>
    <div class="product-card__cta">
      <button class="product-card__button">
        <img
          class="product-card__button-icon"
          src="/images/icon-cart.svg"
          alt="shopping cart"
        />

        <span class="product-card__button-text">Add to Cart</span>
      </button>
    </div>
  </section>
</article>
<!-- markup (zero or more items) goes here -->

<!-- * STYLE -->
<style>
  .product-card {
    max-width: 34.3rem;
    /* margin: 2.8rem auto; */
    border-radius: var(--border-radius);
    overflow: hidden;
  }

  .product-card__img {
    width: 100%;
    height: 24rem;
    background-image: url("../assets/images/image-product-mobile.jpg");
    background-size: cover;
    /* display: block; */
  }

  .product-card__details {
    padding: 2.4rem;
    background: var(--neut-white);
  }

  .product-card__subtitle {
    color: var(--neut-blue-dark-grayish);
    font-weight: 500;
    /* line-height: 1.5; */
    font-size: 1.2rem;
    letter-spacing: 0.5rem;
    text-transform: uppercase;
    margin-bottom: 1.2rem;
  }

  .product-card__title {
    font-family: "Fraunces";
    font-size: 3.2rem;
    font-weight: 700;
    /* line-height: 3.2rem; */
    line-height: 100%;
    margin-bottom: 1.6rem;
    color: var(--neut-blue-very-dark);
  }

  .product-card__description {
    font-weight: 500;
    font-size: 1.4rem;
    /* line-height: 1.5; */
    line-height: 164%;
    margin-bottom: 2.4rem;
  }

  .product-card__price {
    display: flex;
    align-items: center;
    margin-bottom: 2rem;
  }

  .product-card__price-after-discount {
    font-family: "Fraunces";
    font-size: 3.2rem;
    font-weight: 700;
    color: var(--pri-cyan);
    margin-right: 1.9rem;
  }

  .product-card__price-before-discount {
    font-size: 1.3rem;
    text-decoration: line-through;
  }

  .product-card__cta {
  }
  .product-card__button {
    width: 100%;
    height: 4.8rem;
    border: none;
    border-radius: 0.8rem;
    background: var(--pri-cyan);
    color: var(--neut-white);
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1.161rem;
    transition: all 0.3s ease;
  }

  .product-card__button:hover {
    background-color: var(--pri-aquamarine-hover);
  }

  .product-card__button-icon {
    width: 1.439rem;
  }
  .product-card__button-text {
    font-weight: 700;
  }

  @media (min-width: 90em) {
    .product-card {
      display: flex;
      justify-content: center;
      align-items: center;
      max-width: 60rem;
      max-height: 45rem;
    }

    .product-card__img {
      height: 45rem;
      width: 30rem;
      background-image: url("./images/image-product-desktop.jpg");
      background-position: center;

      background-size: cover;
      background-repeat: no-repeat;
      background-position: 50% 50%;
      /* object-fit: cover; */
    }

    .product-card__details {
      width: 30rem;
      padding: 3.2rem;
      /* margin-bottom: 2rem; */
    }

    .product-card__subtitle {
      margin-bottom: 2rem;
      /* line-height: 1.5; */
    }
    .product-card__title {
      margin-bottom: 2.4rem;
    }

    .product-card__description {
      margin-bottom: 2.9rem;
      line-height: 164%;
    }

    .product-card__price {
      margin-bottom: 3rem;
    }

    .product-card__price-before-discount {
      line-height: 177%;
    }
  }
</style>
