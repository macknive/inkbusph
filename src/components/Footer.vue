<template>
  <div class="formbold-main-wrapper appointment">
    <div class="formbold-form-wrapper">
      <h2 style="color: black; text-align: center; margin-bottom: 50px">
        Book an Appointment
      </h2>
      <form action="">
        <div class="formbold-mb-5">
          <label for="name" class="formbold-form-label"> Name </label>
          <input
            type="text"
            name="name"
            id="name"
            placeholder="Full Name"
            class="formbold-form-input"
          />
        </div>
        <div class="formbold-mb-5">
          <label for="phone" class="formbold-form-label"> Phone Number </label>
          <input
            type="text"
            name="phone"
            id="phone"
            placeholder="Enter your phone number"
            class="formbold-form-input"
          />
        </div>
        <div class="formbold-mb-5">
          <label for="email" class="formbold-form-label"> Email Address </label>
          <input
            type="email"
            name="email"
            id="email"
            placeholder="Enter your email"
            class="formbold-form-input"
          />
        </div>
        <div class="flex flex-wrap formbold--mx-3">
          <div class="w-full sm:w-half formbold-px-3">
            <div class="formbold-mb-5 w-full">
              <label for="date" class="formbold-form-label"> Date </label>
              <input
                type="date"
                name="date"
                id="date"
                class="formbold-form-input"
              />
            </div>
          </div>
          <div class="w-full sm:w-half formbold-px-3">
            <div class="formbold-mb-5">
              <label for="time" class="formbold-form-label"> Time </label>
              <input
                type="time"
                name="time"
                id="time"
                class="formbold-form-input"
              />
            </div>
          </div>
        </div>

        <div>
          <button class="formbold-btn">Book Appointment</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
html {
  box-sizing: border-box;
}
*,
*:before,
*:after {
  box-sizing: inherit;
}
input {
  width: 100% !important;
}
.formbold-main-wrapper {
  background-color: white;
  position: relative;
}

.formbold-mb-5 {
  margin-bottom: 20px;
}
.formbold-pt-3 {
  padding-top: 12px;
}
.formbold-main-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 48px;
  @media screen and (max-width: 450px) {
    padding: 24px;
  }
}

.formbold-form-wrapper {
  margin: 0 auto;
  width: 100%;
  background: white;
  // @media screen and (max-width: 450px) {
  //   max-width: 80%;
  // }
}
.formbold-form-label {
  display: block;
  font-weight: 500;
  font-size: 16px;
  color: #07074d;
  margin-bottom: 12px;
}
.formbold-form-label-2 {
  font-weight: 600;
  font-size: 20px;
  margin-bottom: 20px;
}

.formbold-form-input {
  width: 100%;
  padding: 12px 24px;
  border-radius: 6px;
  border: 1px solid #e0e0e0;
  background: white;
  font-weight: 500;
  font-size: 16px;
  color: #6b7280;
  outline: none;
  resize: none;
}
.formbold-form-input:focus {
  border-color: #6a64f1;
  box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.05);
}

.formbold-btn {
  text-align: center;
  font-size: 16px;
  border-radius: 6px;
  padding: 14px 32px;
  border: none;
  font-weight: 600;
  background-color: black;
  color: white;
  width: 100%;
  cursor: pointer;
}
.formbold-btn:hover {
  box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.05);
}

.formbold--mx-3 {
  margin-left: -12px;
  margin-right: -12px;
}
.formbold-px-3 {
  padding-left: 12px;
  padding-right: 12px;
}
.flex {
  display: flex;
}
.flex-wrap {
  flex-wrap: wrap;
}
.w-full {
  width: 100%;
}
@media (min-width: 540px) {
  .sm\:w-half {
    width: 50%;
  }
}
</style>
