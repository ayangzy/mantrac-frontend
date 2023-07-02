<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-md-4 m-auto mt-5">
          <h1 class="text-center">Sign up</h1>
          <form id="contactForm" data-sb-form-api-token="API_TOKEN">
            <!-- Name input-->
            <div class="form-floating mb-3">
              <input
                class="form-control"
                id="name"
                type="text"
                placeholder="Enter your name..."
                data-sb-validations="required"
              />
              <label for="name">Full name</label>
              <div class="invalid-feedback" data-sb-feedback="name:required">
                A name is required.
              </div>
            </div>
            <!-- Email address input-->
            <div class="form-floating mb-3">
              <input
                class="form-control"
                id="email"
                type="email"
                placeholder="name@example.com"
                data-sb-validations="required,email"
              />
              <label for="email">Business Email address</label>
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

            <div class="form-floating mb-3">
              <input
                class="form-control"
                id="confirm-password"
                type="tel"
                placeholder="confirm password"
                data-sb-validations="required"
              />
              <label for="password">Confirm Password</label>
              <div class="invalid-feedback" data-sb-feedback="confirm-passowrd:required">
                A Confirm password field is required
              </div>
            </div>

            <div class="d-grid">
              <button class="btn btn-primary btn-xl" id="submitButton" type="submit">Signup</button>
            </div>

            <p class="mt-3">Already registered? <router-link to="login">Login</router-link></p>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>