<template>
  <footer>
    <div class="judul my-5">
      <img src="../assets/img/logo.png" alt="" />
    </div>
    <div class="d-flex justify-content-between">
      <div class="footer">
        <h2>Overview</h2>
        <a href="">Shipping</a>
        <a href="">Refund</a>
        <a href="">Promotion</a>
      </div>
      <div class="footer">
        <h2>Company</h2>
        <a href="">About</a>
        <a href="">Career</a>
        <a href="">Contact Us</a>
      </div>
      <div class="footer">
        <h2>Explore</h2>
        <a href="">Terms & Condition</a>
        <a href="">Privacy Policy</a>
        <a href="">For Developer</a>
      </div>
      <div class="footer">
        <h2>Special Letter</h2>
        <form class="d-flex" id="btnSubmit">
          <input
            type="email"
            class="form-control"
            id="inputNama"
            placeholder="Your email address"
            aria-label="Recipient's username"
            aria-describedby="button-addon2"
            required
          />
          <button class="btn btn-outline-danger" type="submit">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-send-fill"
              viewBox="0 0 16 16"
            >
              <path
                d="M15.964.686a.5.5 0 0 0-.65-.65L.767 5.855H.766l-.452.18a.5.5 0 0 0-.082.887l.41.26.001.002 4.995 3.178 3.178 4.995.002.002.26.41a.5.5 0 0 0 .886-.083l6-15Zm-1.833 1.89L6.637 10.07l-.215-.338a.5.5 0 0 0-.154-.154l-.338-.215 7.494-7.494 1.178-.471-.47 1.178Z"
              />
            </svg>
          </button>
        </form>
      </div>
    </div>
  </footer>
        
      
</template>

<script>
export default {

}
</script>

<style>

</style>