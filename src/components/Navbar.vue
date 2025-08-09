<template>

    <nav>
        <div class="log-name">
            <i class="fa-solid fa-dumbbell"></i>
            <h1>Gym Project</h1>
        </div>

        <div class="main-links">
                <a href="#">Home</a>
                <a href="#">Programs</a>
                <a href="#">Trainers</a>
                <a href="#">Pricing</a>
                <a href="#">Contact</a>
        </div>

        <div class="join-now">
            <button>Join Now</button>
        </div>
    </nav>

</template>

<style scoped>
    nav{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 15px;
        background: linear-gradient(to right, #0e111b, #2f1c41);        
    }

    .log-name, .main-links, .join-now{
        display: flex;
        align-items: center;
        gap: 10px;
    }

    .log-name i{
        font-size: 25px;
    }

    .main-links a{
        text-decoration: none;
        color: #FFFFFF;
        font-size: 16px;
        font-weight: 500;
        padding: 10px 20px;
        border-radius: 5px;
        transition: 0.3s;
    }

    .join-now button{
        color: white;
        background-color: transparent;
        border: 1px solid white;
        padding: 10px 25px;
        border-radius: 20px;
        font-size: 16px;
        font-weight: bold;
    }
</style>