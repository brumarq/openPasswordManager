<template>
  <main class="form-signin text-center" style="margin-top: 10%">
    <form class="loginForm" name="login" @submit.prevent="login">
      <h1 class="h3 mb-3 fw-normal">Sign Up</h1>
      <div class="col-12">
        <div class="row">
          <div class="col-6 form-floating">
            <input
              type="email"
              name="email"
              class="form-control"
              id="email"
              v-model="email"
              placeholder="name@example.com"
            />
            <label for="floatingInput" class="floatingInput"
              >First Name</label
            >
          </div>
          <div class="col-6 form-floating">
            <input
              type="email"
              name="email"
              class="form-control"
              id="email"
              v-model="email"
              placeholder="name@example.com"
            />
            <label for="floatingInput" class="floatingInput"
              >Last Name</label
            >
          </div>
        </div>
        <div class="row">
          <div class="col-12 form-floating">
            <input
              type="email"
              name="email"
              class="form-control"
              v-model="password"
              id="email"
              placeholder="Email"
            />
            <label for="floatingInput" class="floatingInput">Email</label>
          </div>
        </div>
        <div class="row">
          <div class="col-12 form-floating">
            <input
              type="password"
              name="password"
              class="form-control"
              v-model="password"
              id="password"
              placeholder="Password"
            />
            <label for="floatingInput" class="floatingInput">Password</label>
          </div>
        </div>
        <div class="row mb-1">
          <div class="col-12 form-floating">
            <small id="errorMessage" class="p-4 text-danger"> </small>
          </div>
        </div>
        <div class="row">
          <div class="col-12 form-floating">
            <button class="w-100 btn btn-lg btn-primary btnLogin" type="submit">
              Sign Up
            </button>
          </div>
        </div>
      </div>
    </form>
    <small class="pt-3">
      Have an account already? <a href="/login" id="signupLink"> Log in</a>
    </small>
  </main>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
html,
body {
  height: 100%;
}

body {
  display: flex;
  align-items: center;
  padding-top: 40px;
  padding-bottom: 40px;
  background-color: #ffffff;
}

.form-signin {
  width: 100%;
  max-width: 630px;
  padding: 15px;
  margin: auto;
}

.form-signin .checkbox, .form-signup .checkbox {
  font-weight: 400;
}

.form-signin .form-floating:focus-within, .form-signup .form-floating:focus-within {
  z-index: 2;
}

.floatingInput {
  padding-left: 25px;
}
</style>
