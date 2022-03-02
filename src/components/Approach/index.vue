<template>
  <div class="approach">
    <div class="container">
      <div class="approach__content">
        <div class="header">Approach</div>
        <div class="approach__items">
          <ApproachItem v-for="item in approachList" :key="item.id" :ApproachListItem="item"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ApproachItem from "@/components/Approach/ApproachItem";

export default {
  name: "index",
  data(){
    return {
      approachList: [
        {id: 1, text: 'Tools for uploading a templates for future automatic generation of contracts with tourists',
        img: require('./../../../images/approach-1.png')},
        {id: 2, text: 'A page for creating a tourist request with financial info and current statuses of their trips',
        img: require('./../../../images/approach-2.png')},
        {id: 3, text: 'Management of agents and their commissions (CRUD)',
        img: require('./../../../images/approach-3.png')},
        {id: 4, text: 'Financing and invoicing management',
        img: require('./../../../images/approach-4.png')},
        {id: 5, text: 'Pop-up notifications for all agents regarding tourists trip, birthdays, air flights, ets',
        img: require('./../../../images/approach-5.png')},
        {id: 6, text: 'Creating a database of tourists and tools to manage them',
        img: require('./../../../images/approach-6.png')},
      ]
    }
  },
  components: {
    ApproachItem
  }
}
</script>

<style lang="scss" scoped>
.approach {
  margin-top: 118px;
  &__content {
    max-width: 912px;
    margin: 0 auto;
  }
  &__items {
    margin-top: 80px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
}

@media(max-width: 576px){
  .header {
    font-size: 56px;
  }
  .approach {
    margin-top: 167px;
    &__items {
      justify-content: center;
    }
  }
}
</style>