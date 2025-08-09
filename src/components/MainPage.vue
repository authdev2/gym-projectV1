<template>
  <div class="main-page">
    <div class="left-side">
      <h1>Transform Your <span>Body</span></h1>
      <p>
        Join thousands of members who have achieved their fitness goals with our
        world-class training programs and expert guidance.
      </p>

      <div class="start-your-journey">
        <button>Start Your Journey</button>
        <button>Watch Demo</button>
      </div>

      <div class="info-gym">
        <div class="info-gym-item">
          <i class="fa-solid fa-people-group"></i>
          <h3>100+</h3>
          <p>Members</p>
        </div>

        <div class="info-gym-item">
          <i class="fa-solid fa-dumbbell"></i>
          <h3>50+</h3>
          <p>Trainers</p>
        </div>

        <div class="info-gym-item">
          <i class="fa-solid fa-clipboard-check"></i>
          <h3>98%</h3>
          <p>Results</p>
        </div>
      </div>
    </div>

    <div class="right-side">
      <img src="../assets/mainImage.png" alt="gym" />
    </div>
  </div>
</template>

<style scoped>
.main-page {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 100px;
  color: #fff;
  height: 90vh;
  background: linear-gradient(to right, #0e111b, #2f1c41);
}

.left-side h1 {
  font-size: 60px;
  font-weight: bold;
  max-width: 700px;

  margin-bottom: 50px;
}

.left-side span {
  color: #f093fb;
  text-decoration: underline;
  text-underline-offset: 20px;
}

.left-side p {
  font-size: 20px;
  color: #e5e7eb;
  max-width: 600px;

  margin-bottom: 20px;
  line-height: 1.5;
}

.start-your-journey button {
  color: white;
  background-color: #f093fb;
  border: none;
  padding: 15px 25px;
  border-radius: 20px;
  margin-right: 30px;
  margin-top: 50px;
  font-weight: bold;
  font-size: 16px;
  cursor: pointer;
}

.start-your-journey button:last-child {
  color: white;
  background-color: transparent;
  border: none;
  padding: 15px 25px;
  border-radius: 20px;
  border: 1px solid #ffffff;
}

.info-gym {
  display: flex;
  align-items: center;
  gap: 50px;
  margin-top: 50px;
  text-align: center;
  font-weight: 500;
}

.info-gym-item i {
  font-size: 30px;
  margin-bottom: 10px;
}

.info-gym-item h3 {
  color: #f093fb;
  font-size: 40px;
  font-weight: bold;
  margin-bottom: 10px;
  margin-top: 10px;
}

.right-side img {
  width: 600px;
  height: 600px;
}
</style>
