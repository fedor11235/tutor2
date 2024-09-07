<template>
  <div class="main">
    <div class="main__header">
      <UDivider >
        <UAvatar
          :src="avatar"
          alt="Avatar"
          size="3xl"
        />
      </UDivider>
    </div>
    <div class="main__body">
        <UCard class="card-info">
          <template #header>
            <span class="font-semibold">Образование</span>
          </template>
          Марийский государственный университет - 01.03.02 Прикладная математика и информатика
        </UCard>
        <UCard class="card-info">
          <template #header>
            <span class="font-semibold">Опыт работы</span>
          </template>
          Icons8 - младший инженер-программист. <br/>
          SidusHeroes - инженер-программист. <br/>
          ИОМ Анкетолог - тим лид
        </UCard>
        <UCard class="card-info">
          <template #header>
            <span class="font-semibold">Проекты</span>
          </template>
          Коммерческие проекты:<br/>
          https://icons8.ru/bgremover - сайт фронт <br/>
          https://sidusheroes.com - сайт фронт <br/>
          https://sidusheroes.com/nidum - игра веб фронт<br/>
          https://xenna.sidusheroes.com - игра декстоп<br/>
          https://sidusheroes.com/asterally- игровой телеграм бот<br/>
          https://anketolog.ru  - сайт фронт <br/>
          ИОМ Анкетолог - тим лид <br/><br/>
          Мли проекты:<br/>
          https://t.me/SlonRobot - телеграм бот<br/>
          https://t.me/SlonRobot - телеграм бот<br/>
          https://t.me/TarologExpertBot - телеграм бот<br/>
        </UCard>
        <UCard class="card-info">
          <template #header>
            <span class="font-semibold">Как проходит обучение</span>
          </template>
          Мои курсы подойдут всем от начинающих до продвинутых.<br/>
          Отталкиваемся от ваших хотелок и вашего уровня. Обсуждаем на первом занятии.<br/>
          Работаем на языках JS, TS, Python.<br/>
          Пишими телеграм ботов, фронт, бэк.<br/>
          Инструменты и язык выбираем от того чем будем заниматься.<br/>
          Скорее всгео будем работать с такими инструментами как Vue и Nuxt и их экосистема, Nest.js, Three.js, Dgango, Flask, Aiogram, FastAPI. SQLLite3, PostgreSQL, git<br/>
          Раберем немного теорию: Декларативный/иперативный подход, ООП/фнкциональщина, Паттерны в программировании, REST, SOLID, CRUD.<br/>
          Я считаю что программирование это прикладная наука, поэтому ы будем каждый термин разбирать в коде, с первого дня поставим себе цель написать ту программу которую вы хотите,
          в первый же урок мы гапишем работчю миним рпрограмму которую будем в дальнейшем улучшать и приводить к готовому виду.
        </UCard>
    </div>
    <div class="main__footer">
      <UDivider label="Записаться на курс" class="mb-10" />
        <UCard class="card-info">
          Для записи на курс и для получения более подробной информации заполните <a class="link" href="https://docs.google.com/forms/d/e/1FAIpQLSc9KgugQjrS0S76Vkxn19G0TIcWvFqoBhwm1hQjppGT_MLRsQ/viewform?usp=sf_link" target="_blank" >анкету</a>
          или же напишите мне в <a class="link" href="https://t.me/fedor11235b" target="_blank" >телеграм</a>
        </UCard>
    </div>

  </div>
</template>

<script setup>
import avatar from "@/assets/img/avatar.jpg"

</script>

<style lang="scss">
.main {
  height: max(100vh, auto);
  &__header {
    background-color: aliceblue;
    padding: 80px 40px;
  }
  &__body {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 32px;
    padding: 40px 40px;
    background: linear-gradient(90deg, white, aliceblue 100%);
    @media (max-width: 900px) {
      grid-template-columns: 1fr;
    }
  }
  &__footer {
    background-color: aliceblue;
    padding: 80px 40px;
  }
}

.card-info {
  width: 100%;
  background: linear-gradient(90deg, aliceblue, white 100%);
}
.link {
  color: blue;
  text-decoration: underline;
}
</style>