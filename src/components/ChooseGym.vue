<template>
  <section>
    <div class="choose-gym">
      <h2>Why Choose Us?</h2>
      <p>
        Experience the difference with our premium facilities, expert trainers,
        and personalized approach to fitness.
      </p>

      <div class="container-items">
        <div class="choose-gym-items" v-for="item in chooseGymItems" :key="item.id">

          <img :src="`./src/assets/svg-icons/${item.img}`" alt="Icons Choose Gym">

          <h3>{{ item.title }}</h3>
          <p>
            {{ item.description }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.choose-gym {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  color: #fff;
  margin-top: 50px;
  padding: 80px;
}

.choose-gym h2 {
  font-weight: bold;
  background: linear-gradient(135deg, #f093fb 0%, #667eea 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  font-size: 30px;
}

.choose-gym p {
  color: #9ca3af;
  max-width: 600px;
  font-size: 17px;
  text-align: center;
}

.container-items {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.choose-gym-items {
  background-color: #21272f50;
  border-radius: 10px;
  padding: 20px;
  width: 400px;
  height: 230px;
  margin-top: 50px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  padding: 20px;
}

.choose-gym-items h3 {
  font-size: 20px;
  margin-top: 20px;
}

.choose-gym-items p {
  text-align: start;
  margin-top: 20px;
  color: #d1d5db;
}

.choose-gym-items img{
  width: 50px;
  height: 50px;
}
</style>


<script setup>

  const chooseGymItems = [
    {
      img: 'svg1.svg',
      title: 'Expert Trainers',
      description: 'Our trainers are certified professionals with years of experience in helping clients achieve their fitness goals.'
    },
    {
      img: 'svg2.svg',
      title: '24/7 Access',
      description: 'Work out on your schedule with round-the-clock access to our state-of-the-art facilities.'
    },
    {
      img: 'svg3.svg',  
      title: 'Advanced Analytics',
      description: 'Advanced analytics and personalized insights to track your progress and optimize your workouts.'
    },
    {
      img: 'svg3.svg',  
      title: 'Advanced Analytics',
      description: 'Advanced analytics and personalized insights to track your progress and optimize your workouts.'
    },
    {
      img: 'svg3.svg',  
      title: 'Advanced Analytics',
      description: 'Advanced analytics and personalized insights to track your progress and optimize your workouts.'
    },
    {
      img: 'svg3.svg',  
      title: 'Advanced Analytics',
      description: 'Advanced analytics and personalized insights to track your progress and optimize your workouts.'
    }
  ]

</script>