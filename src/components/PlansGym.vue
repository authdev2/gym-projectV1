<template>
  <div class="plans-gym">
    <h1>Choose Your Plan</h1>
    <p>Flexible pricing options to fit your lifestyle and budget</p>

    <div class="plan-gym-container">
      <div class="plan-gym-item">
        <h2>Basic</h2>
        <h3>$29<span>/month</span></h3>
        <p>Perfect for beginners</p>
        <ul>
          <li>
            <i class="fa-solid fa-check"></i>
            Gym access
          </li>
          <li>
            <i class="fa-solid fa-check"></i>
            Personalized training
          </li>
          <li>
            <i class="fa-solid fa-check"></i>
            Nutrition guidance
          </li>
          <li>
            <i class="fa-solid fa-xmark cruz-vermelho"></i>
            Personal training
          </li>
        </ul>
        <button>Get Started</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.plans-gym {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 20px;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.1);
}

.plan-gym-container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.1);
}

.plan-gym-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 20px;
  background-color: #1a1f2e;
  width: 400px;
  height: 450px;
  border-radius: 10px;
}

.plan-gym-item h2 {
  font-size: 30px;
}

.plan-gym-item h3 {
  font-size: 25px;
}

.plan-gym-item span {
  font-size: 1rem;
  color: #9ca3af;
}

.plan-gym-item p {
  font-size: 1rem;
  color: #9ca3af;
}

.plan-gym-item ul {
  list-style: none;
}

.plan-gym-item ul li {
  display: flex;
  gap: 10px;
  align-items: center;
  margin-bottom: 10px;
}

.plan-gym-item ul li:last-child {
  color: #6B7280;
}

.plan-gym-item ul li i {
  color: #667eea;
}

.plan-gym-item ul li i.cruz-vermelho {
  color: #ff0000ce;
}

.plan-gym-item button {
  padding: 15px 70px;
  background-color: #374151;
  border: none;
  border-radius: 20px;
  color: white;
  font-size: 16px;
  font-weight: 600;
}
</style>
