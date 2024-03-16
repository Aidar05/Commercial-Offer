<template>
  <div class="document-body">
      <h2>Коммерческое предложение по созданию веб-сайта.</h2>
      
      <p>
        Мы предлагаем разработку эффективного продающего сайта по отлаженной
        рабочей схеме. Это позволяет получить действительно мощный бизнес-ресурс,
        приносящий прибыль вашей компании. 
      </p>
  
      <h2>ЭТАПЫ И ВИДЫ РАБОТ</h2>

      <div class="table">
        <div class="table-header">
          <h4>Этап 1. Оценка проекта</h4>
        </div>
        
        <div class="table-content">
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
        </div>
      </div>
    </div>
</template>

<script>
export default{
  name: "KP",
  data() {
    return {
      tableOne: [
        {
        "columnName": "ИСПОЛНИТЕЛЬ",
        "points": ["Запрашивает все исходные данные, пожелания для оценки трудоемкости и стоимости проекта",
        "Изучает конкурентов, и если есть - то старый сайт заказчика", 
        "Формирует базовое описание проекта и оценивает стоимость"] 
        }, 
        {
        "columnName": "ЗАКАЗЧИК",
        "points": ["Предоставляет необходимую информацию и отвечает на вопросы",
        " Согласует стоимость и требования к сайту"] 
        }, 
        {
        "columnName": "РЕЗУЛЬТАТЫ",
        "points": [" У обоих сторон есть общее видение проекта, понимание целей и задач будущего сайта",
        " Определена стоимость и сроки разработки"] 
        }, 
      ]
    }
  }
}
</script>