<template>
<div class="">
    <div class="d-flex justify-content-center my-5">
        <div class="col-md-4">
          <form
            action=""
            class="shipping p-5"
            id="formShipping"
            style="border: 3px solid pink"
          >
            <h1 style="text-align: center">Shipping Form</h1>
            <div class="row">
              <div class="mb-3 col-md-6">
                <label for="first name">First Name</label>
                <input
                  class="form-control"
                  type="text"
                  placeholder="Enter your first name"
                  id="firstName"
                  required
                />
              </div>
              <div class="mb-3 col-md-6">
                <label for="phone number">Phone Number</label>
                <input
                  class="form-control"
                  type="number"
                  placeholder="Enter Phone number"
                  id="phoneNumber"
                />
              </div>
              <div class="mb-3 col-md-6">
                <label for="last name">Last Name</label>
                <input
                  class="form-control"
                  type="text"
                  placeholder="Enter your last name"
                  id="lastName"
                  required
                />
              </div>
              <div class="mb-3 col-md-6">
                <label for="city">City</label>
                <input
                  class="form-control"
                  type="text"
                  placeholder="Enter city"
                  id="city"
                />
              </div>
              <div class="mb-3 col-md-6">
                <label for="first name">Email Address</label>
                <input
                  class="form-control"
                  type="email"
                  placeholder="Enter email"
                  id="email"
                />
              </div>
              <div class="mb-3 col-md-6">
                <label for="postal code">Postal Code</label>
                <input
                  class="form-control"
                  type="text"
                  placeholder="Enter postal code"
                  id="postalCode"
                />
              </div>
              <label for="">Address</label>
              <div class="input-group">
                <textarea
                  class="form-control"
                  name=""
                  id="address"
                  placeholder="Enter address"
                  required
                ></textarea>
              </div>
              <div class="p-3 col-md-6">
                <button
                  type="submit"
                  class="btn"
                  style="background-color: pink"
                  id="btnSubmitShipping"
                >
                  Submit
                </button>
              </div>
            </div>
          </form>
        </div>
      </div>
</div>
      <!-- <div class="alert alert-success d-none" role="alert" id="alert">
        <h4 class="alert-heading" id="title"></h4>
        <p id="Isi"></p>
        <a href="index.html">
          <button type="submit" class="btn btn-primary">Back</button>
        </a>
      </div> -->
</template>

<script>

import Shipping from '@/pages/Shipping.vue';
export default {
name: 'formView',
component:{
    Shipping
}
}
</script>

<style>

</style>