<template>

<v-img
          contain
          height="300"
          src="@/assets/logo.svg"
        />
  
        <div class="text-body-2 font-weight-light mb-n1">Zapraszam do</div>
  
        <h1 class="text-h2 font-weight-bold">Coaching Warszawa {{ $route.path}}</h1>


        
      <div class="py-14" />
      <v-row class="d-flex align-center justify-center">
        <v-col cols="auto">
        
        
        
 <p class="text-justify font-weight-bold ">Patrz przed siebie… Idź swoją drogą</p>
 <p class="text-justify">To hasło chyba najlepiej oddaje moje podejście do życia i tego, jak chcę pracować z innymi oraz to, co chciałabym im przekazać. Nasza droga nie musi być prosta: pojawiają się na niej zakręty, czasami rozwidlenia, na których możemy wybrać niewłaściwy kierunek. Czasami jest wyboista, błotnista albo piaskowa. Wówczas trudniej jest iść. Może pomóc nam wówczas uważność na szczegóły dookoła nas: krople rosy na liściach paproci, koty leżąca na przydrożnej ścieżce pod drzewem, turkusowe żuki czy drzewa uginające się pod ciężarem owoców. A co można poczuć? Niepokój, związany z czarnymi chmurami zbierającymi się nad horyzontem, albo radość z pojawiających się pierwszych promieni słońca, które wychyla się po długich dniach szarości. 
Zmieniają się pory roku, pogoda…<br>
Drogowskazów czasem brakuje albo są nieczytelne<br>
A My cały czas idziemy… Wolniej, szybciej, czasami siadamy odpocząć</p>

 <p class="text-justify font-weight-bold">A gdzie jest Twoja droga? W mieście? W lesie? Co ją teraz otacza? Co ją teraz pokrywa? Co jest dookoła?</p>
 <p class="text-justify">Z przyjemnością i chęcią potowarzyszę Ci w tej niej tak długo, jak będzie to potrzebne; tak długo jak będziesz chciała.</p>

 <p class="text-justify">Świadomie zdecydowałam się na pracę tylko z kobietami, gdyż jest mi ona po prostu bliższa. </p>

        
        
        
        
        
        
        
        
        
        
        <p class="text-justify font-weight-bold ">Jestem HR-owcem z 15-letnim doświadczeniem pracy z ludźmi. Jakiś czas temu postanowiłam skupić się bardziej na obszarze life coachingu. Z wykształcenia jestem pedagogiem i psychologiem, a obszary rozwojowe, podnoszące samoświadomość były mi zawsze bliskie; zwłaszcza samorozwój kobiet oraz wspieranie ich w podążaniu własną drogą i odkrywanie siebie. Specjalizuję się w obszarach coachingu relacji, life coachingu, coachingu kariery i biznesowym. Pracuję w nastawieniu na cele Klienta, skupiam się na jego mocnych stronach, możliwościach i potrzebach.
        <br>
        <br>Ada Huber / Coaching Warszawa  
        </p></v-col>
      </v-row>
      <v-row class="d-flex align-center justify-center">

        <v-col cols="auto">
          <v-btn
            color="primary"
            href="https://calendar.google.com/calendar/u/0/appointments/schedules/AcZssZ32aVhzgi2zKeZ2lJHluHAWxElKMwGmG--fPqO1UGM6N-Gy7959yTHK69fQFsAZnKDukalWVmxl?gv=true"
            min-width="228"
            rel="noopener noreferrer"
            size="x-large"
            target="_blank"
            variant="flat"
          >
            <v-icon
              icon="mdi-calendar"
              size="large"
              start
            />

            Rozpocznij coaching *
          </v-btn>
          <p>*<i>Pierwsza sesja w CoachingWarszawa.com jest bezpłatna</i></p>
          <Article  
          v-for="post in posts"
          :key="post.id"
          :title="post.title"    
          :slug="post.slug"      
          />
        </v-col>

      </v-row>

</template>

<script setup>
import Article from './Article.vue'
import { ref } from 'vue'
const posts = ref([
  { id: 1, title: 'My journey with Vue', slug: 'slug1' },
  { id: 2, title: 'Blogging with Vue', slug: 'slug2' },
  { id: 3, title: 'Why Vue is so fun', slug: 'slug3' }
])



</script>
