<script>
export default {
    name: "AppMain",
    components: {
    },
    data() {
        return {
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="left-bar">
            <div class="logo-div">
                <img class="logo" src="../assets/img/Il mio progetto.png" alt="">
            </div>
            <div class="section-div">
                <ul class="no-pallini">
                    <li> <span><i class="fa-regular fa-user"></i></span> Admin</li>
                    <li>Customer</li>
                    <li>Policy</li>
                    <li>Domain</li>
                </ul>
            </div>

        </div>
        <div class="central-view"></div>
        <div class="right-bar">
            <div class="wrapper">
                <div class="small-bar"></div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.container {
    position: relative;

    //barra sinbistra con logo e tastini
    .left-bar {
        width: 300px;
        height: 100vh;
        background-color: rgba(0, 128, 0, 0.418);
        ;



        .logo-div {
            display: flex;
            justify-content: center;
            align-items: center;

            .logo {
                width: 50%;
            }

        }

        //parte tastini
        .section-div {
            margin-top: 20px;
            display: flex;
            justify-content: start;
            align-items: center;
            //debug
            // background-color: yellow;

            .no-pallini {
                list-style-type: none;
                width: 100%;

                li {
                    margin-bottom: 10px;
                    padding: 5px;
                    cursor: pointer;


                    &:hover {
                        background-color: lightblue;
                    }
                }
            }

        }

    }

    //barra laterale a destra
    .right-bar {
        width: 400px;
        height: 600px;
        background-color: red;
        border-radius: 30px 0 0 30px;
        position: absolute;
        right: 0;
        top: 20px;

        .wrapper {
            height: 100%;
            width: 100%;
            position: relative;

            .small-bar {
                width: 50px;
                height: 50px;
                background-color: red;
                position: absolute;
                top: 40px;
                left: -50px;
                border-radius: 30px 0 0 30px;
            }
        }
    }
}
</style>