<template>
  <main class="d-flex w-100">
    <div class="container d-flex flex-column">
      <div class="row vh-100">
        <div class="col-sm-10 col-md-8 col-lg-6 col-xl-5 mx-auto d-table h-100">
          <div class="d-table-cell align-middle">
            <div class="text-center mt-4">
              <h1 class="h2">Welcome back!</h1>
              <p class="lead">Sign in to your account to continue</p>
            </div>

            <div class="card">
              <div class="card-body">
                <div class="m-sm-3">
                  <form>
                    <div class="mb-3">
                      <label class="form-label">Email</label>
                      <input
                        class="form-control form-control-lg"
                        type="email"
                        name="email"
                        placeholder="Enter your email"
                      />
                    </div>
                    <div class="mb-3">
                      <label class="form-label">Password</label>
                      <input
                        class="form-control form-control-lg"
                        type="password"
                        name="password"
                        placeholder="Enter your password"
                      />
                    </div>
                    <div>
                      <div class="form-check align-items-center">
                        <input
                          id="customControlInline"
                          type="checkbox"
                          class="form-check-input"
                          value="remember-me"
                          name="remember-me"
                          checked
                        />
                        <label class="form-check-label text-small" for="customControlInline"
                          >Remember me</label
                        >
                      </div>
                    </div>
                    <div class="d-grid gap-2 mt-3">
                      <router-link to="/" class="btn btn-lg btn-primary">Sign in</router-link>
                    </div>
                  </form>
                </div>
              </div>
            </div>
            <div class="text-center mb-3">
              Don't have an account? <router-link to="/auth/register">Sign up</router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.divider:after,
.divider:before {
  content: '';
  flex: 1;
  height: 1px;
  background: #eee;
}

.h-custom {
  height: calc(100% - 73px);
}

@media (max-width: 450px) {
  .h-custom {
    height: 100%;
  }
}
</style>
