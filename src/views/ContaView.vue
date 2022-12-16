<template>
  <main>
    <body>
      <div class="center">
        <h1 class="title">Login</h1>
        <form method="">
          <div class="txt_field">
            <input type="text" required />
            <span></span>
            <label>Nome de usuário</label>
          </div>
          <div class="txt_field">
            <input type="password" required />
            <span></span>
            <label>Senha</label>
          </div>
          <div class="pass">Esqueceu sua senha?</div>
          <input type="submit" value="Login" />
          <div class="signup_link">
            Não tem conta?
            <RouterLink to="/registrar"> Inscreva-se já!</RouterLink>
          </div>
        </form>
      </div>
    </body>
  </main>
</template>
<style scoped>
.title {
  color: black;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  margin: 0;
  padding: 0;
  height: 100vh;
}
.center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 400px;
  background: #f5b5bb;
  border-radius: 10px;
  box-shadow: 10px 10px 15px rgba(0, 0, 0, 0.05);
}
.center h1 {
  text-align: center;
  padding: 20px 0;
  border-bottom: 1px solid silver;
}
.center form {
  padding: 0 40px;
  box-sizing: border-box;
}
form .txt_field {
  position: relative;
  border-bottom: 2px solid #adadad;
  margin: 30px 0;
}
.txt_field input {
  width: 100%;
  padding: 0 5px;
  height: 40px;
  font-size: 16px;
  border: none;
  background: none;
  outline: none;
}
.txt_field label {
  position: absolute;
  top: 50%;
  left: 5px;
  color: black;
  transform: translateY(-50%);
  font-size: 16px;
  pointer-events: none;
  transition: 0.5s;
}
.txt_field span::before {
  content: "";
  position: absolute;
  top: 40px;
  left: 0;
  width: 0%;
  height: 2px;
  background: black;
  transition: 0.5s;
}
.txt_field input:focus ~ label,
.txt_field input:valid ~ label {
  top: -5px;
  color: black;
}
.txt_field input:focus ~ span::before,
.txt_field input:valid ~ span::before {
  width: 100%;
}
.pass {
  margin: -5px 0 20px 5px;
  color: black;
  cursor: pointer;
}
.pass:hover {
  text-decoration: underline;
}
input[type="submit"] {
  width: 100%;
  height: 50px;
  border: 1px solid black;
  background: #e19da3;
  border-radius: 25px;
  font-size: 18px;
  color: black;
  font-weight: 700;
  cursor: pointer;
  outline: none;
  transition: 0.25s;
}
input[type="submit"]:hover {
  border-color: black;
  transform: scale(1.1);
}
.signup_link {
  margin: 30px 0;
  text-align: center;
  font-size: 16px;
  color: black;
}
.signup_link a {
  color: #2691d9;
  text-decoration: none;
}
.signup_link a:hover {
  text-decoration: underline;
}
</style>
