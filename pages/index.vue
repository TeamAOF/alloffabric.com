<template>
  <div class="container">
    <header class="header">
      <img
        class="logo header__logo"
        src="~/assets/images/aof-logo.svg"
        alt="AOF logo"
      />
      <nav>
        <NuxtLink class="link header__link" to="/#download">
          Download
        </NuxtLink>
        <NuxtLink class="link header__link" to="/#support-us">
          Support us
        </NuxtLink>
        <a
          class="link header__link"
          href="https://discord.gg/6rkdm48"
          target="_blank"
          rel="noopener noreferrer"
        >
          Discord
        </a>
        <a
          class="link header__link"
          href="https://github.com/TeamAOF"
          target="_blank"
          rel="noopener noreferrer"
        >
          GitHub
        </a>
      </nav>
    </header>
    <main class="main">
      <img
        class="bolt main__bolt"
        src="~/assets/images/bolt.svg"
        alt="Decorative bolt"
      />
      <div class="main__content">
        <div class="main__buzz">
          <div class="main__buzzaction">
            <img
              class="main__buzzpic"
              src="~assets/images/aof3-logo.png"
              alt="AOF3 Logo"
            />
            <NuxtLink class="button main__buzzlink" to="/#download">
              <IconDownload class="button__icon main__buzzlink-icon" />
              <span class="button__text">Download</span>
            </NuxtLink>
          </div>
          <div class="main__buzzwords">
            <h2 class="main__buzzwords-heading">All of Fabric 3</h2>
            <p class="main__buzzwords-subheading">
              Fabric modpack you will love to play
              <IconHeart class="inline-icon main__buzzwords-heart" />
            </p>
          </div>
        </div>
        <!-- <div class="card main__download">
          <div class="card__wrapper">
            <h1 class="card__header">Download</h1>
            <a
              class="link"
              href="https://curseforge.com/minecraft/modpacks/all-of-fabric-3"
              target="_blank"
              rel="noopener noreferrer"
            >
              All of Fabric 3
            </a>
          </div>
        </div> -->
      </div>
        <a href="https://www.yourkit.com">
   <img src="yklogo" alt="Powered by yourkit">
</a>
    </main>
  </div>

</template>

<script>
import IconDownload from '~/assets/icons/download.svg?inline'
import IconHeart from '~/assets/icons/heart.svg?inline'

export default {
  components: {
    IconDownload,
    IconHeart,
  },
}
</script>

<style lang="scss" scoped>
.container {
  margin: 0 auto;
  max-width: 80rem;
}

.header {
  align-items: center;
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  max-width: 50rem;
  padding: 1rem 0;
}

.header__logo {
  height: 5rem;
}

.header__link {
  font-size: 1.5rem;
  font-weight: bold;
  letter-spacing: 0.05rem;
  margin-left: 2rem;
}

.main {
  min-height: max-content;
}

.main__bolt {
  margin: 0 auto;
  max-width: 80rem;
  position: absolute;
  z-index: -1;
}

.main__buzz {
  margin: 0 auto;
  max-width: 35rem;
  padding-top: 10rem;
}

.main__buzzaction {
  align-items: center;
  display: flex;
  justify-content: space-between;
  margin: 0 3rem -2rem 3rem;
}

.main__buzzpic {
  display: block;
  height: 10rem;
  width: 10rem;
}

.main__buzzlink {
  background-color: #232323;
  color: #fff;
  font-size: 2rem;
  font-weight: bold;
  padding: 1rem 2rem;
}

.main__buzzlink-icon {
  height: 2rem;
}

.main__buzzwords {
  background-color: #232323;
  color: #fff;
  display: block;
  font-size: 2rem;
  padding: 2rem 3rem 2rem 3rem;
}

.main__buzzwords-heading {
  margin: 1rem 0;
  padding: 0;
}

.main__buzzwords-subheading {
  margin: 0;
  padding: 0;
}

.main__buzzwords-heart {
  height: 2rem;
  margin: 0;
  padding: 0;
  width: 2rem;
}

.main__download {
  max-width: fit-content;
}

.logo {
  display: block;
}

.card {
  background: #ff3054;
  clip-path: polygon(95% 0, 100% 100%, 5% 100%, 0 0);
  display: block;
  padding: 1rem;
}

.card__wrapper {
  background: #232323;
  clip-path: polygon(95% 0, 100% 100%, 5% 100%, 0 0);
  padding: 1rem 3rem;
}

.card__header {
  font-size: 2rem;
  font-weight: bold;
  letter-spacing: 0.1rem;
  text-transform: uppercase;
}
</style>
