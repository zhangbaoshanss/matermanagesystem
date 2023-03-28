<template>
    <div id="main-container">
        <div id="container-img">
            <img src="../assets/login.jpg" alt="" id="bg-img">
            <div id="container-form">
                <div id="container-h1">
                    <h1>DRX物资管理系统</h1>
                </div>
                <form action="" method="post" id="form">
                    <input type="text" placeholder="  账户">
                    <input type="password" placeholder="  密码" id="pass-input">
                    <div id="container-btn">
                        <button type="submit" id="login-btn" class="btn">登录</button>
                        <button type="button" id="regist-btn" class="btn">注册</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>
<script>
    export default{
        propos:{
            name:"IndexPage",
            msg:String
        },
    }
</script>
<style>
    #main-container{
        width: 100vw;
        height: 100vh;
        background-color: rgb(51, 32, 108);
        display: flex;
        justify-content: center;
        align-items: center;
        
    }
    #container-img{
        width: 80vw;
        height: 75vh;
        background-color: rgb(228, 218, 232);
        border-radius: 40px;
        display: flex;
        overflow: hidden;
    }
    #bg-img{
    }
    #container-form{
        width: 40vw;
        height: 75vh;
        min-width: 620px;
        overflow: hidden;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        /* background-color: aqua; */
    }
    #container-h1{
        /* background: #ce2a2a; */
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: end;
        order: 1;
        flex-grow: 1;
    }
    #form{
        display: flex;
        flex-direction: column;
        justify-content: start;
        align-items: center;
        margin-top: 50px;
        width: 55%;
        /* background: #956b6b; */
        order: 2;
        flex-grow: 1;
    
    }
    input{
        width: 100%;
        height: 40px;
        border: 1px solid black;
        outline: 0px;
        border-radius: 5px;
    }
    #pass-input{
        margin-top: 30px;
    }
    input:focus{
        border: 1px solid rgb(79, 133, 226);
        /* outline-style: solid;
        outline-width: 5px;
        outline-color: aquamarine; */
    }
    #container-btn{
        margin-top: 30px;
        width: 100%;
        display:flex;
        flex-direction: row;
        order: 3;
        flex-grow: 2;
        /* background-color: brown; */
        justify-content: space-between;
    }
    .btn{
        width: 30%;
        height: 40px;
        display: block;
        outline-style: none;
        border: 1px solid red;
        border-radius: 3px;
    }
    #login-btn{
        
        background: rgb(79, 133, 226);
    }
</style>