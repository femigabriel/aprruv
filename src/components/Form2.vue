<template>
  <div class="login-card">
    <header class="login-header">
      <h1 id="page-title">Create Account</h1>
    </header>
    <div class="form-row">
      <div class="form-container">
        <div class="form-group">
          <div class="form-label">
            <label for="business-name" class="control-label">
              Registered Business Name
            </label>
          </div>
          <div class="form-input">
            <input
              id="business-name"
              type="text"
              class="form-control"
              name="user.attributes.businessName"
              errormessage="Please enter business name"
              required=""
            />
          </div>
        </div>
      </div>

      <div class="form-group">
        <div class="form-label">
          <label for="business-address" class="control-label"
            >Business Address</label
          >
        </div>
        <div class="form-input">
          <input
            type="text"
            id="business-address"
            class="form-control"
            name="user.attributes.businessAddress"
            errormessage="Please enter business address"
            required=""
          />
        </div>
      </div>
    </div>

    <div class="form-group">
      <div class="form-label">
        <label for="business-description" class="control-label">
          What is your Business about?
        </label>
      </div>
      <div class="form-input">
        <textarea
          id="business-description"
          type="text"
          class="form-control"
          rows="4"
          name="user.attributes.businessDescription"
          errormessage="Please enter business description"
          required=""
        ></textarea>
      </div>
    </div>

    <div class="form-group">
      <div class="form-label">
        <label class="control-label"> What's your role at this company? </label>
      </div>
      <div class="form-radio" style="margin-top: 5px">
        <div class="custom-control custom-radio">
          <input
            id="rd-1"
            type="radio"
            name="user.attributes.companyRole"
            class="custom-control-input role-radio"
            value="Company administrator / Senior manager"
          />
          <label class="custom-control-label" for="rd-1"
            >Company administrator / Senior manager</label
          >
        </div>
        <div class="custom-control custom-radio">
          <input
            id="rd-2"
            type="radio"
            name="user.attributes.companyRole"
            class="custom-control-input role-radio"
            value="Employee / Contractor"
          />
          <label class="custom-control-label" for="rd-2"
            >Employee / Contractor</label
          >
        </div>
        <div class="custom-control custom-radio">
          <input
            id="rd-3"
            type="radio"
            name="user.attributes.companyRole"
            class="custom-control-input role-radio"
            value="Director / Owner"
          />
          <label class="custom-control-label" for="rd-3"
            >Director / Owner</label
          >
        </div>
        <div class="custom-control custom-radio">
          <input
            id="rd-4"
            type="radio"
            name="user.attributes.companyRole"
            class="custom-control-input role-radio"
            value="Software Developer / Engineer"
          />
          <label class="custom-control-label" for="rd-4"
            >Software Developer / Engineer</label
          >
        </div>
      </div>
    </div>
    <div class="form-container">
      <div class="form-group">
        <div class="form-label">
          <label class="control-label">
            What products are you interested in?
          </label>
        </div>
        <div class="form-checkbox">
          <div class="custom-control custom-checkbox custom-control-inline">
            <input
              id="ck-1"
              type="checkbox"
              class="custom-control-input products-input"
              value="Appruve Identity"
            />
            <label class="custom-control-label" for="ck-1"
              >Appruve Identity</label
            >
          </div>
          <div class="custom-control custom-checkbox custom-control-inline">
            <input
              id="ck-2"
              type="checkbox"
              class="custom-control-input products-input"
              value="Appruve Agency"
            />
            <label class="custom-control-label" for="ck-2"
              >Appruve Agency</label
            >
          </div>
          <div class="custom-control custom-checkbox custom-control-inline">
            <input
              id="ck-3"
              type="checkbox"
              class="custom-control-input products-input"
              value="Appruve Business"
            />
            <label class="custom-control-label" for="ck-3"
              >Appruve Business</label
            >
          </div>
          <div class="custom-control custom-checkbox custom-control-inline">
            <input
              id="ck-4"
              type="checkbox"
              class="custom-control-input products-input"
              value="Appruve Financial"
            />
            <label class="custom-control-label" for="ck-4"
              >Appruve Financial</label
            >
          </div>
        </div>
      </div>

      <div class="form-group">
        <div class="form-label">
          <label class="control-label">
            What's your role at this company?
          </label>
        </div>
        <div class="form-radio">
          <div class="custom-control custom-radio">
            <input
              id="rd-1"
              type="radio"
              name="user.attributes.companyRole"
              class="custom-control-input role-radio"
              value="Company administrator / Senior manager"
            />
            <label class="custom-control-label" for="rd-1"
              >Company administrator / Senior manager</label
            >
          </div>
          <div class="custom-control custom-radio">
            <input
              id="rd-2"
              type="radio"
              name="user.attributes.companyRole"
              class="custom-control-input role-radio"
              value="Employee / Contractor"
            />
            <label class="custom-control-label" for="rd-2"
              >Employee / Contractor</label
            >
          </div>
          <div class="custom-control custom-radio">
            <input
              id="rd-3"
              type="radio"
              name="user.attributes.companyRole"
              class="custom-control-input role-radio"
              value="Director / Owner"
            />
            <label class="custom-control-label" for="rd-3"
              >Director / Owner</label
            >
          </div>
          <div class="custom-control custom-radio">
            <input
              id="rd-4"
              type="radio"
              name="user.attributes.companyRole"
              class="custom-control-input role-radio"
              value="Software Developer / Engineer"
            />
            <label class="custom-control-label" for="rd-4"
              >Software Developer / Engineer</label
            >
          </div>
        </div>
      </div>

      <div class="form-group">
        <div id="form-options" class="form-label">
          <div class="">
            <span
              ><a
                href="/auth/realms/appruve/login-actions/authenticate?client_id=appruve-web&amp;tab_id=zyle5Q3csV0"
                >« Back to Login</a
              ></span
            >
            <div class="form-button">
              <div class="btn-group">
                <button
                  @click="previous"
                  class="btn btn-secondary disabled"
                  type="button"
                >
                  Previous</button
                ><button @click="next" class="btn btn-secondary" type="button">
                  Next
                </button>
              </div>
              <div class="btn-group" role="group">
                <button class="btn btn-finish disabled">
                  Start Verifying Identities
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Form2",
  data() {
    return {
      errors: [],
    };
  },

  methods: {
    previous() {
      this.$emit("previous");
    },
  },
};
</script>

<style>
.login-card {
  background: #fff;
  margin: 0 auto;
  padding: 0 20px;
  /* height: 650px; */
  border-top: 0;
  border-radius: 1rem;
  box-shadow: 0 16px 24px 0 rgb(0 0 0 / 8%);
  max-width: 750px;
}
.login-header {
  margin-bottom: 20px;
  display: flex;
  flex-direction: column;
}
#page-title {
  font-weight: 600;
  letter-spacing: 3px;
  line-height: 20px;
  color: #111;
  padding: 0.45rem 0.6rem;
  font-size: 1.5rem;
}
.login-header h1 {
  text-align: center;
}
.form-row {
  display: flex;
  flex-wrap: wrap;
  margin-right: -5px;
  margin-left: -5px;
}
textarea {
  display: block;
  box-sizing: border-box;
  width: 100%;
  height: 7rem;
  margin: 0 0 1rem;
  padding: 0.5rem;
  border: 1px solid #cacaca;
  border-radius: 2px;
  background-color: #fff;
  box-shadow: none;
  font-family: inherit;
  font-size: 1.2rem;
  font-weight: 400;
  line-height: 1.5;
  color: #4b4b4b;
  transition: box-shadow 0.5s, border-color 0.25s ease-in-out;
  padding-left: 1rem;
  padding-bottom: 0.04rem;
}
[type="text"] {
  box-sizing: border-box;
  width: 100%;
  margin: 0 0 1rem;
  padding: 0.5rem;
  border: 1px solid #cacaca;
  border-radius: 2px;
  background-color: #fff;
  box-shadow: none;
  font-family: inherit;
  font-size: 1.2rem;
  font-weight: 400;
  line-height: 1.5;
  color: #4b4b4b;
  transition: box-shadow 0.5s, border-color 0.25s ease-in-out;
  padding-left: 1rem;
  padding-bottom: 0.04rem;
}
label {
  font-weight: 600;
  display: inline-block;
  max-width: 100%;
}
.form-label {
  position: relative;
  min-height: 1px;
  margin: 10px 0px;
}
.btn-group {
  position: relative;
  display: inline-block;
  vertical-align: middle;
  margin-left: 5px;
  float: left;
}

.btn-group > .btn:first-child {
  margin-left: 0;
}

.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-top-right-radius: 0;
  border-bottom-right-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn.disabled {
  opacity: 0.65;
  background-color: #fafafa;
  background-image: none;
  border-color: #d1d1d1;
  color: #8b8d8f;
  box-shadow: none;
}
.btn {
  user-select: none;
  border: 1px solid transparent;
  padding: 0.375rem 0.75rem;
  font-size: 1rem;
  line-height: 1.5;
  border-radius: 0.25rem;
  transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out,
    border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
  display: inline-block;
  font-weight: 400;
  text-align: center;
  white-space: nowrap;
  vertical-align: middle;
  box-shadow: 0 2px 3px rgb(3 3 3 / 10%);
}

.btn-secondary {
  color: #fff;
  background-color: #6c757d;
  border-color: #6c757d;
}
</style>
