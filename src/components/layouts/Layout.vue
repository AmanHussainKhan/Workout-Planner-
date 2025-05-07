<script setup></script>

<template>
  <header>
    <h1 class="text-gradient">Workout Planner</h1>
  </header>
  <main>
    <slot />
  </main>
  <footer>
    <small>Created by</small>
    <a href="https:www.amanhussainkhan.com" target="_blank">
      <img
        alt="pfp"
        src="https://media.licdn.com/dms/image/v2/D4D03AQE08j4_xZsDkA/profile-displayphoto-shrink_800_800/profile-displayphoto-shrink_800_800/0/1727105577688?e=1752105600&v=beta&t=uf_fdsA46x4W1HcCPd4YOPcnAVHSjfUMvzhzhBME5Qc"
      />
      <p>Aman Hussain Khan</p>
      <i class="fa-brands fa-github"></i>
    </a>
  </footer>
</template>

<style scoped>
header,
footer,
main {
  padding: 1rem;
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
}

main {
  flex: 1;
}

footer {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  align-items: center;
  padding: 2rem 0;
  padding-bottom: 3rem;
}

footer a {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.3rem;
  padding-right: 0.5rem;
  background: var(--background-muted);
  border-radius: 4rem;
  border: 1px solid transparent;
  transition-duration: 200ms;
  text-decoration: none;
}

footer a:hover {
  border-color: var(--color-link);
}

footer a img {
  max-width: 30px;
  aspect-ratio: 1 / 1;
  border-radius: 100%;
}
</style>
