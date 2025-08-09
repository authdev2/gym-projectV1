<template>
    <div class="trainers">
        <h2>Meet Our Trainers</h2>
        <p>World-class professionals dedicated to your success</p>

        <div class="trainer-cards">
            <div class="trainer-card" v-for="item in trainers" :key="item.name">  
                <img :src="`./src/assets/trainers/${item.image}`" alt="Treinadores">
                <div class="info-trainer">
                    <h3>{{ item.name }}</h3>
                    <p class="trainer-description">{{ item.description }}</p>
                    <p>{{ item.description2 }}</p>
                    <div class="social-media">
                        <i class="fa-brands fa-facebook"></i>
                        <i class="fa-brands fa-instagram"></i>
                        <i class="fa-brands fa-twitter"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.trainers{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 80px;
}
.trainers h2{
    font-size: 48px;
    font-weight: 700;
    margin-bottom: 20px;
    background: linear-gradient(135deg, #f093fb 0%, #667eea 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}
.trainers p{
    font-size: 18px;
    color: #e5e7eb;
    line-height: 1.6;
    opacity: 0.9;
    margin-bottom: 30px;
}

.trainer-cards{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
}

.trainer-card{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #1a1f2e;
    border-radius: 10px;
    width: 350px;
}

.trainer-card img{
    width: 350px;
    height: 240px;
    object-fit: cover;
    border-radius: 10px;
}

.info-trainer{
    padding: 20px;
}

.info-trainer .trainer-description{
    color: #667EEA;
    font-size: 14px;
}


.info-trainer p{
    font-size: 16px;
}

.social-media{
    display: flex;
    gap: 20px;
    color: #f093fb;
}

.social-media i{
    font-size: 20px;
}
</style>

<script setup>
    const trainers = [
        {
            name: 'Flavio Gomes',
            description: 'Strength & Conditioning',
            description2: '10+ years experience in powerlifting and strength training. Certified NASM trainer.',
            image: 'trainer1.jpg'
        },
        {
            name: 'Joao Pedro',
            description: 'Strength & Conditioning',
            description2: '10+ years experience in powerlifting and strength training. Certified NASM trainer.',
            image: 'trainer2.jpg'
        },
        {
            name: 'Jose Carlos',
            description: 'Strength & Conditioning',
            description2: '10+ years experience in powerlifting and strength training. Certified NASM trainer.',
            image: 'trainer3.jpg'
        }   
    ]
</script>