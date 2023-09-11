<template>
  <header class="header">
    <h1 class="title">My NuxtBoard</h1>
  </header>


  <article class="link-wrapper">
    <ClientOnly>
      <NuxtLink class="links" to="/">
        <h3 class="job-title">Personal Finance Writer & Editor</h3>
        <div class="job-details">
          <section class="job-location">
            <img src="~/assets/location.svg" alt="">
            <h5>Nigeria</h5>
          </section>
          <h5 class="job-price-range">
            $80,000 - $90,000
          </h5>
          <h5 class="job-date">
            21-08-2023
          </h5>
        </div>
      </NuxtLink>
    </ClientOnly>
  </article>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  font-family: 'Inter', sans-serif;
}

.header {
  background-color: #016A70;
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.title {
  color: #FFD;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  font-family: Inter;
  font-size: 20px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
}

.link-wrapper {
  display: flex;
  flex-direction: column;
  margin: 12px auto;
  width: 90%;
  gap: 6px;
}

.links {
  border: 2px solid #016A70;
  border-radius: 4px;
  color: inherit;
  text-decoration: none;
  color: #016A70;
  padding: 10px 0;

}

.job-title {
  margin-left: 14px;
}

.job-details {
  display: flex;
  justify-content: space-around;
  align-items: baseline;
  margin-top: 20px;
}

.job-location {
  display: flex;
  align-items: baseline;
}

.job-location img {
  width: 25%;
  transform: translateY(4px);
}

@media only screen and (min-width: 768px) {
  .title {
    font-size: 32px;
  }

  .link-wrapper {
    width: 50%;
  }

}

@media only screen and (min-width: 1024px) {
  .link-wrapper {
    width: 40%;
  }
}

@media only screen and (min-width: 1366px) {
  .link-wrapper {
    width: 30%;
  }
}
</style>