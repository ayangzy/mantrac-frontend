<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-md-4 m-auto mt-5">
          <h1 class="text-center">Sign In</h1>
          <form id="contactForm" data-sb-form-api-token="API_TOKEN">
            <!-- Email address input-->
            <div class="form-floating mb-3">
              <input
                class="form-control"
                id="email"
                type="email"
                placeholder="name@example.com"
                data-sb-validations="required,email"
              />
              <label for="email">Email address</label>
              <div class="invalid-feedback" data-sb-feedback="email:required">
                An email is required.
              </div>
              <div class="invalid-feedback" data-sb-feedback="email:email">Email is not valid.</div>
            </div>

            <div class="form-floating mb-3">
              <input
                class="form-control"
                id="password"
                type=""
                placeholder="Password"
                data-sb-validations="required"
              />
              <label for="password">Password</label>
              <div class="invalid-feedback" data-sb-feedback="password:required">
                A password field is required
              </div>
            </div>

            <div class="d-grid">
              <button class="btn btn-primary btn-xl" id="submitButton" type="submit">Login</button>
            </div>

            <p class="mt-3">Not registered? <router-link to="register">Register</router-link></p>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>