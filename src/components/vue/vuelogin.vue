<script>

import { Image } from "astro:assets";
import user from "../img/user-logo-stok.svg";
import done from "../img/done.svg";
import { defineComponent } from '@vue/composition-api'

export default {
    data() {
        return {
            user: require('../../img/user-logo-stok.svg'),
            done: require('../../img/done.svg')

        };
    }
};
</script>



<template>
    <div class="fluid">
        <div class="container">
            <div class="login-box">
                <div class="head">
                    <!-- <img :src="user" alt="logo" /> -->

                    <p class="p700-40">Вход в систему</p>
                </div>
                <form>
                    <input class="login" type="text" id="username" placeholder="ИИН" required />
                    <input class="login" type="password" id="password" placeholder="Пароль" required />
                    <button class="submit" type="submit">Register</button>
                </form>
                <!-- <a href="/userPage.astro" class="save-me"> <img :src="done" alt="logo" /> -->

                    <p class="p400-20">Запомнить меня</p>
                <!-- </a> -->
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style>
.fluid {
    font-family: Proxima Nova;
}

.container {
    display: flex;
    align-items: center;
    justify-content: center;
    align-content: center;
    height: 100vh;
}

.login-box {
    padding: 50px 40px 60px;
    background-color: #fff;
    border-radius: 20px;
}

.head {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 16px;
}

.login,
.login:active {
    width: auto;
    min-width: 440px;
    max-width: 480px;
    border-radius: 90px;
    background: #f6f6f6;
    padding: 38px 0px 38px 50px;
    border: none;
    color: #282828;

    font-family: Proxima Nova;
    font-size: 24px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

form,
form:hover,
form:active {
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    border: none;
    gap: 20px;
}

.submit {
    border-radius: 100px;
    background: #007aff;
    padding: 38px 0 38px;
    border: none;
    color: #282828;

    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;

    color: #fff;
    font-family: Proxima Nova;
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    letter-spacing: 2.4px;
    text-transform: uppercase;

    opacity: 0.8;
    transition: 0.3s;
}

.submit:hover {
    opacity: 1;
}

.save-me {
    display: flex;
    justify-content: center;
    align-items: center;
    align-content: center;
    margin-top: 19px;
    gap: 13px;
    text-decoration: none;
}

.save-me .p400-20:hover {
    color: green;
}

.p700-40 {
    color: #282828;
    font-family: Proxima Nova;
    font-size: 40px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

.p400-20 {
    color: #282828;
    font-family: Proxima Nova;
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

@media screen and (max-width: 992px) {
    .login-box {
        padding: 42px 25px 42px;
        background-color: #fff;
        border-radius: 20px;
    }

    .login {
        min-width: 260px;
        padding: 28px 0px 28px 50px;
    }

    .submit {
        padding: 28px 0 28px;
    }

    .p700-40 {
        font-size: 28px;
    }

    .p400-20 {
        font-size: 18px;
    }
}

/* @media screen and (min-width: 770px) and (max-width: 992px) {
        .container {
            width: auto;
            max-width: 750px;
        }
    }
    @media screen and (min-width: 992px) and (max-width: 1200px) {
        .container {
            width: auto;
            max-width: 750px;
        }
    }
    @media screen and (min-width: 1200px) and (max-width: 1500px) {
        .container {
            width: auto;
            max-width: 900px;
        }
    } */
</style>
