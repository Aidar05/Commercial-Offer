<template>
  <div class="table">
    <div class="table-header">
      <h4>{{ tableHeader }}</h4>
    </div>
    
    <div class="table-content">
      <div class="table-element" v-for="tableElement in tableContent">
        <div class="column-name">
          <span>{{ tableElement.columnName }}</span>
        </div>
        
        <ul class="column-content">
          <li v-for="(elements, index) in tableElement.points" :key="index">
            {{ elements }}
          </li>
        </ul>
      </div>
    </div>
  </div>

</template>

<script>
export default{
  name: "TableElement",
  props: {
    tableHeader: String,
    tableContent: Array
  }
}
</script>