<template>
  <div class="training-programs">
    <div class="section-header">
      <h2>Training Programs</h2>
      <p>
        Choose from our diverse range of programs designed to meet your specific
        fitness goals and preferences.
      </p>
    </div>

    <div class="container-training-programs">
      <div class="training-programs-items" v-for="item in trainingProgramsItems" :key="item.id">
        <div class="shadow-black"></div>
        <div class="card-content">
          <h4>{{ item.title }}</h4>
          <p>
            {{ item.description }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.training-programs {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  margin-top: 80px;
  padding: 80px;
  /* background: linear-gradient(to right, #0e111b, #2f1c41); */
}

.section-header {
  text-align: center;
  max-width: 800px;
  margin-bottom: 60px;
}

.section-header h2 {
  font-size: 48px;
  font-weight: 700;
  margin-bottom: 20px;
  background: linear-gradient(135deg, #f093fb 0%, #667eea 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.section-header p {
  font-size: 18px;
  color: #e5e7eb;
  line-height: 1.6;
  opacity: 0.9;
}

.container-training-programs {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
  max-width: 1200px;
  width: 100%;
}

.training-programs-items {
  position: relative;
  width: 100%;
  height: 350px;
  border-radius: 20px;
  overflow: hidden;
  cursor: pointer;
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
}

.shadow-black {
  width: 100%;
  height: 100%;
  background: linear-gradient(
    135deg,
    rgba(0, 0, 0, 0.7) 0%,
    rgba(0, 0, 0, 0.4) 100%
  );
  z-index: 1;
}

.card-content {

  z-index: 2;
  text-align: center;
  padding: 10px;
  color: white;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
}

.card-content h4 {
  font-size: 24px;
  font-weight: 600;
  margin-bottom: 15px;
  color: white;
}

.card-content p {
  font-size: 16px;
  line-height: 1.5;
  color: #e5e7eb;
  margin-bottom: 25px;
  opacity: 0.9;
}

.training-programs-items:nth-child(1) {
  background-image: url("../assets/young-woman-exercising-with-her-headphones.jpg");
  background-size: cover;
  background-position: center;
}

.training-programs-items:nth-child(2) {
  background-image: url("../assets/womencardio.jpg");
  background-size: cover;
  background-position: center;
}

.training-programs-items:nth-child(3) {
  background-image: url("../assets/womanYoga.jpg");
  background-size: cover;
  background-position: center;
}

.training-programs-items:nth-child(4) {
  background-image: url("../assets/womentraining.jpg");
  background-size: cover;
  background-position: center;
}

.training-programs-items:nth-child(5) {
  background-image: url("../assets/womentraining.jpg");
  background-size: cover;
  background-position: center;
}

.training-programs-items:nth-child(6) {
  background-image: url("../assets/womentraining.jpg");
  background-size: cover;
  background-position: center;
}

@media (max-width: 1600px) {

  .training-programs-items {
    width: 300px;
    height: 230px;
}

.card-content h4 {
    font-size: 20px;
  }

  .card-content p {
    font-size: 13px;
}

.section-header h2 {
    font-size: 30px;
}

.section-header p {
    font-size: 17px;
}
}

@media (max-width: 980px) {
  .container-training-programs {
    grid-template-columns: repeat(2, 300px);
    width: 610px;
}
}

@media (max-width: 630px) {
  .container-training-programs {
    grid-template-columns: repeat(1, 300px);
    width: 300px;
}
}

</style>


<script setup>
  const trainingProgramsItems = [
    {
      title: 'Strength Training',
      description: 'Build muscle and increase power with our comprehensive strength training programs.',
    },
    {
      title: 'Cardio Fitness',
      description: 'Improve endurance and burn calories with high-intensity cardio workouts.',
    },
    {
      title: 'Flexibility & Yoga',
      description: 'Enhance flexibility and find inner peace with our yoga and stretching classes.',
    },
    {
      title: 'Wellness Programs',
      description: 'Focus on overall health and wellness with our holistic approach to fitness.',
    },
    {
      title: 'Wellness Programs',
      description: 'Focus on overall health and wellness with our holistic approach to fitness.',
    },
    {
      title: 'Wellness Programs',
      description: 'Focus on overall health and wellness with our holistic approach to fitness.',
    }
  ]
</script>