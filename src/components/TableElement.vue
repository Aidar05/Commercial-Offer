<!-- <template>
  <div class="table-element" v-for="tableElement in tableOne">
    <div class="column-name">
      <span>{{ tableElement.columnName }}</span>
    </div>
    
    <ul class="column-content">
      <li v-for="(elements, index) in tableElement.points" :key="index">
        {{ elements }}
      </li>
    </ul>
  </div>
</template>

<script>
export default{
  name: "TableElement",
  props: {
    columnName: String,
    columnContent: Array
  }
}
</script> -->