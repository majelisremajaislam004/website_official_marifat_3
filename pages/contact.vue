<template>
    <main>
        <navbar/>
        <div class="container">
            <div class="row justify-content-center">
                <div class="content">
                    <div class="image-box">
                        <img src="~/static/assets/img/mjd.jpg" alt="ini gambar mesjid">
                    </div>
                    <form action="#">
                    <div class="topic">Send us a message</div>
                    <div class="input-box">
                        <input type="text" required>
                        <label>Enter your name</label>
                    </div>
                    <div class="input-box">
                        <input type="text" required>
                        <label>Enter your email</label>
                    </div>
                    <div class="message-box">
                        <label>Enter your message</label>
                    </div>
                    <div class="input-box">
                        <input type="submit" value="Send Message">
                    </div>
                    </form>
                </div>
            </div>
        </div>
        <end/>
    </main>
</template>

<style scoped>
.container{
  z-index: 12;
  max-width: 1050px;
  width: 100%;
  background: rgb(255, 255, 255);
  border-radius: 12px;
  margin-top: 2rem;
  margin-bottom: 2rem;
  box-shadow: 0 15px 25px rgba(0,0,0,0.25);
}
.container .content{
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 25px 20px;
}
.content .image-box{
  max-width: 55%;
}
.content .image-box img{
  width: 100%;
}
.content .topic{
  font-size: 22px;
  font-weight: 500;
  color: #FFD700;
}
.content form{
  width: 40%;
  margin-right: 30px;
}
.content .input-box{
  height: 50px;
  width: 100%;
  margin: 16px 0;
  position: relative;
}
.content .input-box input{
  position: absolute;
  height: 100%;
  width: 100%;
  border-radius: 6px;
  font-size: 16px;
  outline: none;
  padding-left: 16px;
  background: #a7a1816e;
  border: 2px solid transparent;
  transition: all 0.3s ease;
}
.content .input-box input:focus,
.content .input-box input:valid{
  border-color: #FFD700;
  background-color: #fff;
}
.content .input-box label{
  position: absolute;
  left: 18px;
  top: 50%;
  color: #a7a181;
  font-size: 15px;
  pointer-events: none;
  transform: translateY(-50%);
  transition: all 0.3s ease;
}
.content .input-box input:focus ~ label,
.content .input-box input:valid ~ label{
  top: 0;
  left: 12px;
  display: 14px;
  color: #FFD700;
  background: #fff;
}
.content .message-box{
  min-height: 100px;
  position: relative;
}
.content .message-box textarea{
  position: absolute;
  height: 100%;
  width: 100%;
  resize: none;
  background: #a7a181;
  border: 2px solid transparent;
  border-radius: 6px;
  outline: none;
  
}
.content .message-box textarea:focus{
  border-color: #FFD700;
  background-color: #fff;
}
.content .message-box label{
  position: absolute;
  font-size: 16px;
  color: #a7a181;
  left: 18px;
  top: 6px;
  pointer-events: none;
  transition: all 0.3s ease;
}
.content .message-box textarea:focus ~ label{
  left: 12px;
  top: -10px;
  color:#FFD700;
  font-size: 14px;
  background: #fff;
}
.content .input-box input[type="submit"] {
  color: #fff;
  background: #FFD700;
  padding-left: 0;
  font-size: 18px;
  font-weight: 500;
  cursor: pointer;
  letter-spacing: 1px;
  transition: all 0.3s ease;
}
.content .input-box input[type="submit"]:hover{
  background-color: #FFD700;
}
@media (max-width:1000px) {
  .content .image-box{
    max-width: 70%;
  }
  .content{
    padding: 10px 0;
  }
}
@media (max-width:900px) {
  .content .image-box{
    display: none;
  }
  .content form{
    width: 100%;
    margin-left: 30px;
  }
}
</style>
