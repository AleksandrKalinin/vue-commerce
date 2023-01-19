<template>
  <header class="header"></header>
  <main class="container">
    <aside class="sidebar"></aside>
    <section class="content">
      <div class="content-header">
        <h2 class="content-header__category">Cameras</h2>
        <div class="content-header__items">
          <nav class="content-header__menu content-menu">
            <span class="content-menu__link content-menu__link_active">По цене</span>
            <span class="content-menu__link">Название</span>
            <span class="content-menu__link">Популярность</span>
          </nav>
          <div class="content__display content-display">
            Показывать по:
            <select class="content-display__selected">10</select>
          </div>          
        </div>
      </div>
      <div class="catalog">
        <div class="catalog-item"></div>
      </div>
      <nav class="content-navigation">
        <span href="" class="content-navigation__item content-navigation__item_active">1</span>
        <span href="" class="content-navigation__item">2</span>
        <span href="" class="content-navigation__item">3</span>
        <span href="" class="content-navigation__item">4</span>
      </nav>
    </section>
  </main>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {

  }
}
</script>

<style lang="sass">

*
  box-sizing: border-box
  margin: 0
  padding: 0
  font-family: 'Open Sans', sans-serif

body
  width: 100%  

.header
  width: 100%
  height: 100px
  background: #ffffff 
  box-shadow: 0 4px 2px -2px #cccccc

.container
  padding: 20px
  border: 1px solid #cccccc
  height: 1000px  
  display: flex
  justify-content: space-between

.sidebar
  height: 100%
  width: 250px
  border: 1px solid #cccccc

.content
  border: 1px solid #cccccc
  height: 100%
  width: calc(100% - 250px - 20px)  

.content-header
  width: 100%
  padding: 20px
  .content-header__items
    display: flex
    justify-content: space-between  
  h2
    font-size: 40px
    margin-bottom: 16px
  .content-header__menu
    display: flex
  .content-menu__link
    margin-right: 16px
    cursor: pointer  

.content-navigation
  padding: 20px
  border: 1px solid #cccccc
  display: flex
  justify-content: center

.content-navigation__item
  padding: 8px 13px
  font-size: 18px
  font-weight: 700
  color: #000000
  cursor: pointer  

.content-navigation__item_active
  background: #53B220
  color: #ffffff

</style>
