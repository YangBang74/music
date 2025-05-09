<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <header class="header">
    <div class="container">
      <div class="header__wrap">
        <div class="header__left">
          <RouterLink to="/" class="header__logo">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 73.099 74.074"
              width="50"
              height="50"
            >
              <g
                transform="matrix(1.166686, 0, 0, 1.166686, -10.507028, -9.630989)"
                fill="var(--logo-color)"
              >
                <g xmlns="http://www.w3.org/2000/svg">
                  <path
                    d="M69.999,40c0.001-16.567-13.432-30-30-29.999C24.984,9.999,12.545,21.031,10.345,35.432C10.117,36.92,10,38.446,10,40   c0,16.569,13.431,30,30,30C56.566,70,69.999,56.568,69.999,40z M11.958,47.395c2.577,4.538,7.447,7.604,13.041,7.604   c8.284,0.001,15-6.717,15-15c0-8.284,6.716-15,15-15c5.595-0.001,10.463,3.067,13.041,7.606c0.624,2.361,0.959,4.839,0.959,7.394   c0.001,15.99-13.01,29-29,29C26.563,69,15.236,59.814,11.958,47.395z"
                  />
                </g>
              </g>
            </svg>
          </RouterLink>
          <div class="header__menu">
            <RouterLink to="/" class="header__menu-link active">Home</RouterLink>
            <RouterLink to="/" class="header__menu-link">Feed</RouterLink>
            <RouterLink to="/" class="header__menu-link">Library</RouterLink>
          </div>
        </div>
        <form class="header__search">
          <input type="text" placeholder="Search" class="header__search-input" />
          <button type="button" class="header__search-submit">
            <svg
              viewBox="0 0 24 24"
              width="24"
              height="24"
              xmlns="http://www.w3.org/2000/svg"
              aria-hidden="true"
            >
              <path
                d="M10 2.25a7.75 7.75 0 1 0 4.924 13.735l5.546 5.545 1.06-1.06-5.545-5.546A7.75 7.75 0 0 0 10 2.25ZM3.75 10a6.25 6.25 0 1 1 12.5 0 6.25 6.25 0 0 1-12.5 0Z"
                fill="currentColor"
              ></path>
            </svg>
          </button>
        </form>
        <div class="header__actions">
          <div class="header__user">
            <svg
              viewBox="0 0 24 24"
              width="30"
              height="30"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
              <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
              <g id="SVGRepo_iconCarrier">
                <circle cx="12" cy="9" r="3" stroke="currentColor" stroke-width="1.5"></circle>
                <circle cx="12" cy="12" r="10" stroke="currentColor" stroke-width="1.5"></circle>
                <path
                  d="M17.9691 20C17.81 17.1085 16.9247 15 11.9999 15C7.07521 15 6.18991 17.1085 6.03076 20"
                  stroke="currentColor"
                  stroke-width="1.5"
                  stroke-linecap="round"
                ></path>
              </g>
            </svg>
            <svg
              viewBox="0 0 24 24"
              height="20"
              width="20"
              xmlns="http://www.w3.org/2000/svg"
              class="header__user-arrow"
            >
              <path
                d="M20.5303 9.53033L12 18.0607L3.46967 9.53033L4.53033 8.46967L12 15.9393L19.4697 8.46967L20.5303 9.53033Z"
                fill="currentColor"
              ></path>
            </svg>
          </div>
          <button class="header__more">
            <svg
              viewBox="0 0 16 16"
              height="30"
              width="30"
              xmlns="http://www.w3.org/2000/svg"
              aria-hidden="true"
            >
              <path
                d="M4 8c0-.832-.67-1.5-1.511-1.5C1.67 6.5 1 7.168 1 8s.67 1.5 1.489 1.5C3.33 9.5 4 8.832 4 8zm5.5 0c0-.832-.67-1.5-1.504-1.5C7.17 6.5 6.5 7.168 6.5 8s.67 1.5 1.496 1.5C8.831 9.5 9.5 8.832 9.5 8zM15 8c0-.832-.664-1.5-1.493-1.5C12.664 6.5 12 7.168 12 8s.664 1.5 1.507 1.5C14.336 9.5 15 8.832 15 8z"
                fill="currentColor"
              ></path>
            </svg>
          </button>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.header {
  position: fixed;
  width: 100%;
  height: 46px;
}

.header__wrap {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header__left {
  display: flex;
  align-items: center;
  gap: 10px;
}

.header__logo {
  width: 100%;
  max-width: 80px;
}

.header__menu {
  display: flex;
  font-weight: 600;
  justify-content: space-between;
  width: 100%;
  max-width: 300px;
}

.header__menu-link {
  padding: 12px 8px;
}

.header__menu-link.active {
  border-bottom: 3px solid #000;
}

.header__actions {
  display: flex;
  align-items: center;
}

.header__search {
  position: relative;
}

.header__search-input {
  width: 100%;
  padding: 10px 20px;
  border-radius: 5px;
  background-color: var(--input-background);
}

.header__search-submit {
  position: absolute;
  align-self: center;
  right: 20px;
  top: 50%;
  transform: translateY(-45%);
}
</style>
