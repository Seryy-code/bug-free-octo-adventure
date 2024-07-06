<template>
  <h3>
    1 Создание компонента кнопки: Создайте компонент кнопки в Vue.js, который
    меняет свой текст при клике.
  </h3>
  <ButtonComponent />
  <h3>
    2 Отображение списка: Используя директиву v-for, выведите список элементов
    массива на странице.
  </h3>
  <ListComponent />
  <h3>
    3 Форма ввода с двусторонним связыванием: Создайте форму с полем ввода и
    отобразите введённый текст ниже поля ввода с использованием директивы
    v-model.
  </h3>
  <FormComponent />
  <h3>
    4 Вычисляемое свойство: Создайте компонент Vue, в котором будет вычисляемое
    свойство, зависящее от значения других данных компонента.
  </h3>
  <MathComponent />
  <h3>
    5 Обработка событий: Добавьте обработчик события на кнопку, который изменяет
    данные компонента Vue при клике.
  </h3>
  <ContainerFigureComponent />
</template>

<script>
import ButtonComponent from "./components/ButtonComponent.vue";
import ListComponent from "./components/ListComponent.vue";
import FormComponent from "./components/FormComponent.vue";
import MathComponent from "./components/MathComponent.vue";
import ContainerFigureComponent from "./emits/ContainerFigureComponent.vue";

export default {
  name: "App",
  components: {
    ButtonComponent,
    ListComponent,
    FormComponent,
    MathComponent,
    ContainerFigureComponent,
  },
};
</script>

<style>
#app {
  width: 70%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 60px;
  margin: auto;
}
button {
  padding: 10px 30px;
  cursor: pointer;
}
</style>
