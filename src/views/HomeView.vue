<script>
import { RouterLink, RouterView } from 'vue-router'
export default {
  data() {
    return {
      dialog: false
    }
  },
  methods: {
    closeDialog() {
      this.dialog = false;
    },
    aboutUs() {
      this.closeDialog();
    }
  }
}
</script>

<template>
  <div id="start"></div>
  <v-container class="bg-image">
    <div>
      <h1 class="introduce">

      </h1>

      <a href="https://t.me/simplephysics_polyteh" target=»_blank>
      <v-btn
        transition="slide-x-transition"
        size="x-large"
        height='72'
        variant="elevated"
        append-icon="mdi-send"
        color="#1976D2"
        rounded="xl"
        >
        Перейти в Телеграм канал
      </v-btn>
      </a>
      <a href="https://t.me/simplephysicsbot" target=»_blank style="text-decoration: none;">
        <v-btn 
          transition="slide-x-transition"
          size="x-large"
          height='72'
          append-icon="mdi-robot"
          color="white"
          rounded="xl"
          variant="flat"
          block
          style="margin-right: 20px; margin-top: 20px;"
          >
          Перейти в телеграм бот
        </v-btn>
      </a>
      <a href="#path" style="text-decoration: none;">
        <v-btn 
          transition="slide-x-transition"
          size="x-large"
          height='72'
          variant="tonal"
          append-icon="mdi-account-multiple"
          color="white"
          rounded="xl"
          block
          style="margin-right: 20px; margin-top: 20px;"
          >
          О нас
        </v-btn>
      </a>
      <div id="path"></div>
    </div>

    <!-- <v-dialog
      v-model="dialog"
      width="auto"
    >
      <v-card style="padding: 20px; border-radius: 20px;" variant="flat" color="dark-indigo" class="Mascot-wrapper">
        <v-card-text class="mascot">
          <h2>Добро пожаловать в SIMPLE PHYSICS!</h2>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/Mascot.png"
          ></v-img>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <a href="#path" style="color: black; text-decoration: none;">
            <v-btn
            variant="elevated"
            color="green"
            @click="aboutUs"><a href="#path" style="color: black; text-decoration: none;">О нас</a>
            </v-btn>
          </a>
          <v-btn variant="elevated" color="gray" @click="closeDialog">Закрыть</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog> -->
    
  </v-container>
  <div class="introduce__content">
    <h1 style="margin-bottom: 40px;">
      SIMPLE PHYSICS
    </h1>
    <p style="margin-bottom: 15px;">
      Добро пожаловать! Перед вами проект Московского политехнического университета «Simple physics», 
      направленный на популяризацию физики среди широкой аудитории школьников и студентов. 
      Физика окружает нас повсюду и влияет на нашу повседневную жизнь. 
    </p>
    <p style="margin-bottom: 15px;">
      Мы уверены, что она намного интереснее, чем вы думаете, поэтому хотим показать вам это воочию. 
      Данная разработка включает в себя интерактивные уроки и видео, которые помогают учащимся лучше 
      понять и визуализировать сложные физические концепции. 
    </p>
    <p style="margin-bottom: 15px;">
      Проект «Simple physics» призван вдохновить людей на изучение науки, показать ее увлекательную 
      сторону и дать возможность каждому увидеть, как физика играет важную роль в нашем мире.
      C нами вы полюбите физику, а она сама откроется для вас совсем с другой стороны!
    </p>
  </div>
  <v-container style="color: #757474">
    <v-timeline>
      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Разработчик</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/me.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Лев</div>
          <p>
            1 Курс
          </p>
          <p>
            Факультет информационных технологий
          </p>
          <p>
            Информатика и вычислительная техника.
          </p>
          <p>
            Системная и программная инженерия (231-3213)
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Куратор</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 12.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Светлана</div>
          <p>
            Ассистент Центра проектной деятельности
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Контент-мейкер</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 5.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Анастасия</div>
          <p>
            1 Курс
          </p>
          <p>
            Машиностроительный Факультет
          </p>
          <p>
            Управление в технических системах(231-251)
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Дизайнер</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/5_1.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Василиса</div>
          <p>
            1 Курс
          </p>
          <p>
            Полиграфический институт  
          </p>
          <p>
            Технология полиграфического и упаковочного производства
          </p>
          <p>
            Дизайн и технологии производства визуального контента (231-722)
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Дизайнер</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/я.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Любовь</div>
          <p>
            1 Курс
          </p>
					<p>
            Группа 231-821
          </p>
          <p>
            Институт графики и искусства книги имени В.А. Фаворского
          </p>
          <p>
            54.03.01 Дизайн
            Графический дизайн мультимедиа
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Монтажер</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 6.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Родион</div>
          <p>
            1 Курс
          </p>
					<p>
            Группа 231-262
          </p>
          <p>
            Факультет машиностроения 
          </p>
          <p>
            Интеллектуальная электроника и промышленный интернет вещей
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Контент-мейкер</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/4.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Ирина</div>
          <p>
            1 Курс
          </p>
          <p>
            Полиграфический институт 
          </p>
          <p>
            Дизайн и проектирование мультимедиа и визуального контента 
          </p>
          <p>
            Технология полиграфического и упаковочного производства (231-721)
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Участник</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 2.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Мерген</div>
          <p>
            1 Курс
          </p>
          <p>
            Факультет химической технологии и биотехнологии
          </p>
          <p>
            Техносферная безопасность (231-511)
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Участник</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 1.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Артем</div>
          <p>
            1 Курс
          </p>
          <p>
            Машиностроительный Факультет
          </p>
          <p>
            Управление в технических системах (232-251)
          </p>
        </div>
      </v-timeline-item>

			<v-timeline-item>
        <template v-slot:opposite>
          <h2>Контент-мейкер</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 4.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Оскар</div>
          <p>
            1 Курс
          </p>
          <p>
            Группа 231-329
          </p>
          <p>
            факультета информационных технологий
          </p>
          <p>
            Системная и программная инженерия
          </p>
        </div>
      </v-timeline-item>

			<v-timeline-item>
        <template v-slot:opposite>
          <h2>Контент-мейкер</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 7.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Ксения</div>
          <p>
            1 Курс
          </p>
					<p>
            факультет Издательского дела
          </p>
          <p>
            специализация Книгоиздательское дело
          </p>
          <p>
            Группа 231-013
          </p>
        </div>
      </v-timeline-item>

			<v-timeline-item>
        <template v-slot:opposite>
          <h2>Контент-мейкер</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 3.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Оксана</div>
          <p>
            1 Курс
          </p>
					<p>
            Институт издательского дела и журналистики
          </p>
          <p>
            Журналистика
          </p>
          <p>
            Группа 231-022
          </p>
        </div>
      </v-timeline-item>

			<v-timeline-item>
        <template v-slot:opposite>
          <h2>Участник</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 8.png"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Иван</div>
          <p>
            1 Курс
          </p>
					<p>
            Факультет информационных технологий
          </p>
          <p>
            Информационные технологии управления бизнесом
          </p>
          <p>
            Группа 231-365
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          <h2>Участник</h2>
        </template>
        <div>
          <v-img
            :width="300"
            aspect-ratio="16/9"
            cover
            src="src/images/чел 9.jpg"
          ></v-img>
        </div>
        <div>
          <div class="text-h6">Айдын</div>
          <p>
            1 Курс
          </p>
					<p>
            Факультет информационных технологий
          </p>
          <p>
            информационная безопасность
          </p>
          <p>
            Группа 231-352
          </p>
        </div>
      </v-timeline-item>			
			
    </v-timeline>
  </v-container>

  <v-container>
      <a href="#start" style="color: rgb(50, 49, 49); text-decoration: none;">
        <v-btn color="rgb(50, 49, 49)" block>Наверх</v-btn>
      </a>
  </v-container>

</template>

<style scoped>
.bg-image {
    height: 100vh;
    min-width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    background: 
      linear-gradient(rgba(0,0, 0, 0.7), rgba(0, 0, 0, 0.8)), 
      url(https://catherineasquithgallery.com/uploads/posts/2023-01/1674274927_catherineasquithgallery-com-p-serii-fon-tekstura-abstraktsiya-foto-22.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-position: top; 
}

.mascot {
  display: flex;
  justify-content: center;
  align-items: center;
}


.introduce {
  text-align: center;
  opacity: 1;
  font-size: 50px;
}

.introduce__content {
  text-align: center;
  margin: 50px 65px;
  color:#828181;
}

.introduce__btn {
  display: block;
}
</style>
