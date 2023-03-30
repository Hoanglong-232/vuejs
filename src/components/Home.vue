<template>
    <div class="container">
        <h3>Đăng nhập</h3>
        <div class="box-login">
            <div class="form-group">
                <label class="label-form">Ten dang nhap</label>
                <input type="text" class="input-form">
            </div>
            <div class="form-group">
                <label class="label-form">Mat khau</label>
                <input type="password" class="input-form">
            </div>
        </div>
        <div class="button">
            <div>
                <button class="btn-orange">
                    <span>Dang ky</span>
                </button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name : 'Home',
};
</script>
<style scoped>
.container {
    width: 300px;
    height: 300px;
}
h3 {
    font-family: Cabin;
    font-size: 40px;
    line-height: 49px;
    font-weight: normal;
    margin-bottom: 24px;
    color: #383F47;
}
.box-login {
    background: #eb6f27;
    border-radius: 12px;
    padding: 16px;
    margin-bottom: 16px;
}
.label-form {
    font-family: Cabin;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 19px;
    color: #0631a0;
}
.input-form {
    background: #FFFFFF;
    border: 1px solid #ECEDF1;
    box-sizing: border-box;
    border-radius: 12px;
    font-size: 16px;
    line-height: 19px;
    padding: 14px 16px 15px 16px;
    width: 100%;
}
.button {
    display: flex;
   justify-content: space-between;
}

.btn-orange {
    color: #fff;
    background: #F39B13;
    border-radius: 12px;
    font-family: Cabin;
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 22px;
    text-align: center;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    padding: 17px 24px;
    border: none;
    cursor: pointer;
}

.btn-orange:hover {
    opacity: 0.7;
}

a {
    color: #007bff;
    text-decoration: none;
    background-color: transparent;
}
</style>