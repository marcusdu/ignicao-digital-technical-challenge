<template>
  <nav class="apps">
    <p class="apps__title">Apps</p>
    <ul class="apps__list">
      <li class="apps__item">
        <img src="@/assets/images/mail.svg" alt="Email" />
        <p class="apps__item-text">Email</p>
      </li>
      <li class="apps__item">
        <img src="@/assets/images/message-square.svg" alt="Conversar" />
        <p class="apps__item-text">Conversar</p>
      </li>
      <li class="apps__item">
        <img src="@/assets/images/check-square.svg" alt="Todo" />
        <p class="apps__item-text">Todo</p>
      </li>
      <li class="apps__item">
        <img src="@/assets/images/calendar.svg" alt="Calendário" />
        <p class="apps__item-text">Calendário</p>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'AppsSidebar'
}
</script>

<style lang="scss" scoped>
@import '@/assets/sass/abstracts/_variables.scss';

.apps {
  margin: 5rem 0 0 3rem;

  &__list {
    @media screen and (max-width: 800px) {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }
  }

  &__title {
    margin-bottom: 0.625rem;
    text-transform: uppercase;
    color: $appsSidebarTitle;

    @media screen and (max-width: 800px) {
      text-align: center;
    }
  }

  &__item {
    display: flex;
    margin: 2rem 0;
    cursor: pointer;

    &:hover {
      opacity: 0.5;
    }
  }

  &__item-text {
    margin-left: 0.625rem;

    @media screen and (max-width: 800px) {
      margin: 0 2rem;
    }
  }
}
</style>
