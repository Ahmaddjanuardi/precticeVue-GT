<template>
    
        <div class="container my-5">
        <div class="row">
          <div class="col-2 d-flex flex-column justify-content-between">
            <img
              src="../assets/img/side-1.png"
              alt="side-1"
              style="width: 50%"
            />
            <img
              src="../assets/img/side-2.png"
              alt="side-2"
              style="width: 50%"
            />
            <img
              src="../assets/img/side-3.png"
              alt="side-3"
              style="width: 50%"
            />
            <img
              src="../assets/img/side-2.png"
              alt="side-3"
              style="width: 50%"
            />
            <img
              src="../assets/img/side-1.png"
              alt="side-3"
              style="width: 50%"
            />
          </div>
          <div class="col-6">
            <img
              :src="require('@/assets/img/' + imageLink + '.png')"
              alt=""
              id="imgParent"
            />
          </div>
          <div class="col-4 d-flex flex-column justify-content-start">
            <div class="judul">
              <h3>Chair Thatty</h3>
              <p>IDR 12.000.000</p>
              <router-link to="/shipping">
                <a
                  class="btn btn-light"
                  href="./form_shipping.html"
                  role="button"
                >
                  <img src="../assets/img/cart3.svg" alt="" />
                  Add to Cart</a
                >
              </router-link>
              <hr />
            </div>
            <div class="title">
              <h4>About the product:</h4>
              <p>
                Tailored to a level of perfection synonymous with that of a
                Savile Row suit and with understated quality in the detail,
                Jetty has been influenced by timeless 1950s style.
              </p>
              <p>
                Providing a subtle nod to the past, Jetty also provides a
                perfect solution for the way we work today. A comprehensive
                product family, Jetty features a veriety of elegant chairs and
                sofas.
              </p>
            </div>
          </div>
        </div>
      </div>
    
</template>

<script>
export default{

    name: 'ComponentView',
    props: ['imageLink']
}
</script>

<style>
#imgParent{
  height: 609px;
    width: 560px;
}
</style>