<template>
  <div id="app">
    <div
      class="jumbotron jumbotron-fluid bg-success text-white jumbo d-none"
      style="position: absolute; left: 0; bottom: 0; z-index: 333"
    >
      <div class="container">
        <h6 class="display-6 text-center">
          Malumotlar Muvaffaqqiyatli yuborildi
        </h6>
      </div>
    </div>

    <div class="box d-flex">
      <div class="col-md-6 col-12 second d-flex align-items-center">
        <div class="urtaga">
          <h2 class="text-center text-light pb-2">Regestration</h2>

          <form method="post" class="form captcha" action="#">
            <input
              type="text"
              placeholder="Ism *"
              class="form-control p-2 w-75 m-auto mb-3 ism"
              required
            />

            <input
              type="text"
              placeholder="Familiya *"
              class="form-control p-2 w-75 m-auto mb-3 familiya"
              required
            />

            <input
              type="text"
              placeholder="Otasining Ismi *"
              class="form-control p-2 w-75 m-auto mb-3 sharif"
              required
            />

            <input
              type="number"
              placeholder="tel: +998 99 999 99 99 *"
              class="form-control p-2 w-75 m-auto mb-3 nomer"
              required
            />

            <input
              type="email"
              placeholder="Email *"
              class="form-control p-2 w-75 m-auto mb-3 email"
              required
            />

            <select
              class="form-select p-2 w-75 m-auto mb-3 tuman"
              aria-label="Default select example "
            >
              <option selected required>Tumaningizni Tanlang *</option>
              <option value="Bulungʻur tumani">Bulungʻur tumani</option>
              <option value="Ishtixon tumani">Ishtixon tumani</option>
              <option value="Jomboy tumani">Jomboy tumani</option>
              <option value="Kattaqoʻrgʻon tumani">Kattaqoʻrgʻon tumani</option>
              <option value="Qoʻshrabot tumani">Qoʻshrabot tumani</option>

              <option value="Narpay tumani">Narpay tumani</option>
              <option value="Nurobod tumani">Nurobod tumani</option>
              <option value="Oqdaryo tumani">Oqdaryo tumani</option>
              <option value="Paxtachi tumani">Paxtachi tumani</option>
              <option value="Payariq tumani">Payariq tumani</option>
              <option value="Pastdargʻom tumani">Pastdargʻom tumani</option>
              <option value="Samarqand tumani">Samarqand tumani</option>

              <option value="Samarqand shaxar">Samarqand shaxar</option>

              <option value="Toyloq tumani">Toyloq tumani</option>
              <option value="Urgut tumani">Urgut tumani</option>
              <option value="Urgut tumani">boshqa</option>
            </select>
            <input
              type="text"
              placeholder="Ta'lim Muassasasi"
              class="form-control p-2 w-75 m-auto mt-2 dargoh"
            />
            <div class="container w-75 pt-3 d-flex justify-content-between p-0">
              <div class="d-flex justify-content-between position-relative">
                <img
                  src="https://avatars.mds.yandex.net/i?id=46c011064e0d50fd5df1fc10a4162c94-4901993-images-thumbs&n=13"
                  alt="rasm yuklanmoqda"
                  class="rasm"
                  style="width: 200px; height: 60px"
                />
                <div
                  class="spinner-border spin"
                  style="position: absolute; left: 85px; top: 15px"
                  role="status"
                ></div>
                <i class="fa fa-arrow-right fa-2x mt-3"></i>
                <input
                  type="text"
                  class="form-control w-25 kod"
                  value=""
                  placeholder="kod"
                />
              </div>
            </div>
            <button
              class="btn btn-primary w-75 d-block m-auto mt-3"
              type="submit"
            >
              jo'natish
            </button>
          </form>
        </div>
      </div>

      <div
        class="
          col-md-6 col-12
          bg-danger
          first
          d-flex
          justify-content-center
          align-items-center
        "
      >
        <div class="w-75 h-100">
          <h2
            class="
              text-white text-center
              position-relative
              z-index-3
              mt-5
              women
            "
            style="
              text-shadow: 10px 10px 50px rgb(243, 195, 4);
              font-size: 50px;
              font-family: 900;
              font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS',
                sans-serif;
            "
          >
            WOMEN IT CUP
          </h2>

          <h3
            class="text-light"
            style="position: absolute; bottom: 200px; left: 100px"
          >
            Batafsil ma'lumotlar uchun
          </h3>

          <div
            class="
              w-50
              h-25
              m-auto
              d-flex
              justify-content-evenly
              flex-column-reverse
            "
            style="position: absolute; bottom: 50px; left: 100px"
          >
            <a
              class="fa fa-telegram fa-2x text-decoration-none fs-6"
              href="https://t.me/dasturchi_qizlar_klubi"
              style="color: rgb(2, 192, 255)"
            >
              <span style="font-family: calibri">Dasturchi Qizlar Klubi</span>
            </a>
            <a
              class="fa fa-instagram fa-2x text-decoration-none fs-6"
              href="https://www.instagram.com/dasturchilarklubi/"
              style="color: rgb(255, 103, 212)"
            >
              <span style="font-family: calibri">Dasturchilar Klubi</span></a
            >

            <a
              class="fs-6 text-white text-decoration-none fa fa-phone fa-2x"
              href="tel:+998 88 406 83 23"
              style="position: absolute; bottom: -15px"
            >
              +998 88 406 83 23</a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "App",
  components: {},

  data() {
    return {};
  },

  mounted() {
    const ism = document.querySelector(".ism");
    const familiya = document.querySelector(".familiya");
    const sharif = document.querySelector(".sharif");
    const nomer = document.querySelector(".nomer");
    const email = document.querySelector(".email");
    const tuman = document.querySelector(".tuman");
    const dargoh = document.querySelector(".dargoh");
    const spin = document.querySelector(".spin");
    const jumbo = document.querySelector(".jumbo");
    const rasm = document.querySelector(".rasm");
    const captcha = document.querySelector(".captcha");
    const kod = document.querySelector(".kod");

    axios.get("https://dk-reg.herokuapp.com/api/bot/cap").then((res) => {
      rasm.src = "data:image/png;base64," + res.data.item1;
      spin.style.display = "none";
      console.log(res.data.id);

      console.log(res);

      captcha.addEventListener("submit", (evt) => {
        evt.preventDefault();
        if (kod.value == "") {
          alert('kaptchani to"ldiring malumotlar junatilmadi');
        }
        if (res.data.id && kod.value !== "") {
          evt.preventDefault();
          axios
            .post(
              `https://dk-reg.herokuapp.com/api/bot/reg/${res.data.id}/${kod.value}`,
              {
                ism: ism.value,
                familiya: familiya.value,
                otasining_ismi: sharif.value,
                nomer: nomer.value,
                email: email.value,
                tuman: tuman.value,
                Talim_Musassasasi: dargoh.value,
              }
            )
            .then((res) => {
              console.log(res.status);
              console.log(typeof res.status);
              if (res.status === 200) {
                jumbo.style.cssText =
                  "display:block !important;position: absolute; left: 0; bottom: 0; z-index: 333;";
                setTimeout(() => {
                  window.location.reload();
                }, 1500);
                setTimeout(() => {
                  jumbo.style.cssText = "display:none !important";
                }, 2000);

                ism.value = "";
                familiya.value = "";
                sharif.value = "";
                nomer.value = "";
                email.value = "";
                tuman.value = "tumaningizni tanlang";
                dargoh.value = "";
                kod.value = "";
              }
            })
            .catch((error) => {
              console.log(error);
              if (
                error.response.data === "incorrect captcha" ||
                error.response.status == 409
              ) {
                alert(
                  "kodni xato kiritdingiz, yoki mavjud kodni qaytadan kirityapsiz"
                );
              }
            });
        }
      });
    });

    axios.get("https://dk-reg.herokuapp.com/api/bot/reg").then((res) => {
      console.log(res);
    });
  },
};
</script>

<style>
*{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}

body{
	display: flex;
	justify-content: center;
	align-items: center;
	min-height: 100vh;
background: rgb(29,101,242);
background: linear-gradient(135deg, rgba(29,101,242,0.8407738095238095) 20%, rgba(177,58,180,0.8519782913165266) 74%);

}


body::before{
	content: '';
	position: absolute;
	top: 0;
	left: 0;
	width: 40%;
	height: 75%;

	border-radius: 50%;
	background: rgb(146,1,255);
background: linear-gradient(90deg, rgba(146,1,255,0.6278886554621849) 16%, rgba(18,169,226,0.8183648459383753) 79%);
filter: blur(3px);

}

body::after{
	content: '';
	position: absolute;
	bottom: 0;
	right: 0;
	width: 10%;
	height: 20%;
	
	border-radius: 50%;
	background: rgb(146,1,255);
background: linear-gradient(90deg, rgba(146,1,255,0.6278886554621849) 16%, rgba(18,169,226,0.8183648459383753) 79%);

filter: blur(3px);
z-index: -1;
}

.box{
width: 1100px;
height: 650px;
border-radius: 10px;

}

.first, .second{
	min-height: 650px;
}

.first{
	background-image:url(https://www.hse.ru/data/2021/07/06/1430854722/3iStock-1194430784.jpg);;
	
	border-top-left-radius: 10px;
	border-bottom-left-radius: 10px;
	position: relative;
	font-family: 'Prompt', sans-serif;
	box-shadow: -10px 20px 30px rgba(0, 0, 0, 0.5);
	transition-duration:1s;
}

.first:before{
	content: '';
	width: 100%;
	height: 100%;
	position: absolute;
	top: 0;
	background: rgba(0,0,0,0.5);
	backdrop-filter: blur(3px) saturate(199%);
    -webkit-backdrop-filter: blur(3px) saturate(199%);
    background-color: rgba(255, 255, 255, 0.14);
   
    border: 1px solid rgba(209, 213, 219, 0.3);
}

.second{
	border-top-left-radius: 10px;
	border-bottom-left-radius: 10px;
	backdrop-filter: blur(9px) saturate(199%);
    -webkit-backdrop-filter: blur(9px) saturate(199%);
    background-color: rgba(255, 255, 255, 0.29);
    border: 1px solid rgba(209, 213, 219, 0.3);

}


.first:hover{
	transform: scale(1.02);
	-moz-transform: scale(1.02);
	-ms-transform: scale(1.02);
	-o-transform: scale(1.02);
	-webkit-transform: scale(1.02);
}



.urtaga{
	width: 90%;
	height: 90%;
	font-family: 'Prompt', sans-serif;
		caret-color: red;
	margin: auto;


}


input{
	background-color: rgba(255,255,255,0.8) !;
}


[placeholder="Ism *"] {
  background:#fff url(https://cdn2.iconfinder.com/data/icons/leto-blue-online-education/64/__woman_laptop_student_studing-256.png)  97% 50% no-repeat ;
  background-size: 10%;

}
[placeholder="Ism *"]::-webkit-inner-spin-button {
  display: none;
}
[placeholder="Ism *"]::-webkit-calendar-picker-indicator {
  opacity: 0;
 
}



[type="number"] {
  background:#fff url(https://cdn3.iconfinder.com/data/icons/token/128/Telephone-Alt.png)  97% 50% no-repeat ;
  background-size: 10%;
}
[type="number"]::-webkit-inner-spin-button {
  display: none;
}
[type="number"]::-webkit-calendar-picker-indicator {
  opacity: 0;
}



[type="email"] {
  background:#fff url(https://cdn0.iconfinder.com/data/icons/leto-blue-web-marketing-content-1/64/_-05-128.png)  97% 50% no-repeat ;
  background-size: 10%;
}
[type="email"]::-webkit-inner-spin-button {
  display: none;
}
[type="email"]::-webkit-calendar-picker-indicator {
  opacity: 0;
}


[placeholder="Ta'lim Muassasasi"] {
  background:#fff url(https://cdn3.iconfinder.com/data/icons/education-1-1/256/School-128.png)  97% 50% no-repeat ;
  background-size: 10%;
}
[placeholder="Ta'lim Muassasasi"]::-webkit-inner-spin-button {
  display: none;
}
[placeholder="Ta'lim Muassasasi"]::-webkit-calendar-picker-indicator {
  opacity: 0;
}


@media  (min-width:200px) and (max-width:800px)  {
	.box{
		display: block !important;
	}


	body{
	min-height: 70vh;
	}


	.rasm{
		width: 150px !important;
	}

	.spin{
		left: 60px !important;
	}

	.jumbo{
		position: absolute !important;
		top: 0 !important;
		left: 0 !important;
		width: 100% !important;
		height: 100px !important;
		display: flex;
		justify-content: center;
		align-items: center;
		
}
.women{
	top: -150px;
}

body::before{
	content: '';
	width: 45%;
	height: 20%;
	position: absolute;
	top: 0;
	background: rgba(0,0,0,0.5);
	backdrop-filter: blur(3px) saturate(199%);
    -webkit-backdrop-filter: blur(3px) saturate(199%);
    background-color: rgba(255, 255, 255, 0.14);
    border: 1px solid rgba(209, 213, 219, 0.3);
	
}
}


</style>
