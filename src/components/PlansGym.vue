<template>
  <div class="plans-gym">
    <h1>Choose Your Plan</h1>
    <p class="description-plans">Flexible pricing options to fit your lifestyle and budget</p>

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
          <li class="last-item">
            <i class="fa-solid fa-xmark cruz-vermelho"></i>
            Personal training
          </li>
        </ul>
        <button>Get Started</button>
      </div>

      <div class="plan-gym-item degrade-item">
        <h2>Premium</h2>
        <h3>$50<span>/month</span></h3>
        <p>Everything you need</p>
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
            <i class="fa-solid fa-check"></i>
            2x personal training sessions
          </li>
        </ul>
        <button>Get Started</button>

        <div class="most-popular">
          <p>Most Popular</p>
        </div>
      </div>

      <div class="plan-gym-item top-item">
        <h2>Elite</h2>
        <h3>$70<span>/month</span></h3>
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
            <i class="fa-solid fa-check"></i>
            8x personal training sessions
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
}

.plans-gym .description-plans {
  color: white;
  font-size: 16px;
  font-weight: 600;
  margin-bottom: 50px;
}

.plan-gym-container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
  padding: 20px;
  border-radius: 10px;
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

.plan-gym-item ul li.last-item {
  color: #6b7280;
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

.degrade-item {
  background: linear-gradient(to right, #1f253f, #764ba2);
  height: 500px;
  position: relative;
}

.degrade-item button{
    background-color: white;
    color: #667EEA;
}

.most-popular {
  position: absolute;
  top: -4%;
  right: 30%;
  background-color: #F093FB;
  padding: 10px 20px;
  border-radius: 20px;
}

.most-popular p {
  font-size: 16px;
  font-weight: 600;
  color: #1f253f;
}

.top-item {
  position: relative;
}

.top-item h2{
    font-size: 40px;
    color: #c39709b7;

}

.top-item h3{
    font-size: 30px;

}

.top-item p{
    font-size: 16px;
}

.top-item button{
    background-color: #c39709b7;
}
</style>
