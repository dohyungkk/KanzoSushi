<template>
    <div>
      <div class="backgroundCommentImage">
        <div class='catchyTitle'> Customer Comments</div>
        <hr>
      <div class='comments'>
        <ul id="messages">
          <li>
            <div class="infos">
            <img src="http://farm3.staticflickr.com/2721/4531285963_cd28f61b16_q.jpg" alt=""  title="customer" />
            </div>
            <div class="content">
              <h3>
                Anita Young
                <b>Vancouver, BC</b>
              </h3>
              <p>
                Used to come here after school with my sister. We both loved the Baked Scallop Roll (prawn, cream cheese, avocado, tobiko, crab, and BBQ scallop on top.) It had a very nice BBQ flavour.
              </p>
            </div>
          </li>
          <li>
            <div class="infos">
              <img src="http://farm3.staticflickr.com/2617/3873098259_61c446da22_q.jpg" alt="" title="customer" />
           </div>
           <div class="content">
            <h3>
            DineVancity
            <b>Vancouver, BC</b>
            </h3>
            <p>
              The service was great and they were very patient. My friends and I took about 20 minutes arguing about what to order because there were so many grey choices! The server came multiple times to take our order and was happily at the task. The food came quick and was great. It's a good deal for the part trays!</a>.
            </p>
            </div>
          </li>

           <li>
            <div class="infos">
              <img src="../assets/anita.jpg" alt="" title="customer" />
            </div>
          <li>
          <div class="content">
            <h3>
              Steven K.
              <b>Vancouver, BC</b>
            </h3>
            <p>
              I eat here quite often. Sometimes for dinner, but usually for a quick lunch during work. The sushi is great and the service/preparation is fast. I recommend for work people who need a quick lunch. 

              With that said, their lunch time can get busy and sometimes you have to wait to be seated, but usually not more than 5-10 minutes. Turnover of tables is fast and the food comes out fast.
            </p>
          </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>


<style scoped>

  .comments {
    padding-top: 20px;
  }

  .backgroundCommentImage {
  height: 1000px;
  opacity: 1;
  background: url("../assets/DSC00221.jpg") no-repeat center center fixed;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    background-color:#F5F5EC;
  }

  .catchyTitle {
    color: #CD594A;
    padding-top: 30px;
    text-align: left;
    font-size: 50px;

  }

body {
  background: url("http://i58.tinypic.com/2586qdx.jpg");
  font: 15px/150% serif; }

#messages {
  position: relative;
  margin: 50px auto;
  padding: 0;
  width: 800px;
  list-style: none; }

#messages li {
  float: left;
  margin-bottom: 30px;
  padding-bottom: 30px;
  }

#messages li:nth-child(2n) .infos {
  float: right;
  margin-left: 20px; }

#messages li:nth-child(2n) .infos a {
  -webkit-box-shadow: 1px 1px 0 1px rgba(90, 81, 15, 0.2);
  -moz-box-shadow: 1px 1px 0 1px rgba(90, 81, 15, 0.2);
  box-shadow: 1px 1px 0 1px rgba(90, 81, 15, 0.2);
  left: inherit; }

#messages li:nth-child(2n) .content { border-width: 1px 3px 4px 4px; }

#messages li:nth-child(2n) .content:after,
#messages li:nth-child(2n) .content:before {
  right: -9px;
  left: inherit;
  -webkit-transform: rotate(41deg);
  -moz-transform: rotate(41deg);
  -o-transform: rotate(41deg);
  transform: rotate(41deg); }

#messages li:nth-child(2n) .facebook { right: -10px; }

#messages li:nth-child(2n) .twitter { right: -5%; }

#messages .infos {
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  -ms-border-radius: 50%;
  -o-border-radius: 50%;
  border-radius: 50%;
  position: relative;
  float: left;
  padding: 3px;
  width: 130px;
  height: 130px;
  border: 5px solid #c8c7b4; }

#messages .infos a {
  -webkit-border-radius: 17px;
  -moz-border-radius: 17px;
  -ms-border-radius: 17px;
  -o-border-radius: 17px;
  border-radius: 17px;
  -webkit-box-shadow: -1px 1px 0 1px rgba(90, 81, 15, 0.2);
  -moz-box-shadow: -1px 1px 0 1px rgba(90, 81, 15, 0.2);
  box-shadow: -1px 1px 0 1px rgba(90, 81, 15, 0.2);
  position: absolute;
  width: 20px;
  height: 22px;
  background-color: #d5d2a8;
  color: #fff;
  text-decoration: none;
  text-indent: -10000px;
  font-size: 11px;
  font-style: italic; }

#messages img {
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  -ms-border-radius: 50%;
  -o-border-radius: 50%;
  border-radius: 50%;
  width: 100%; }

.sprite {
  background: url("https://docs.google.com/uc?export=download&id=0B3VygIVAuRCQRzF1d0RyWHFFRU0") no-repeat;
  background-size: 23px; }

.twitter {
  background-position: -1px 5px;
  top: 16%;
  left: -5%; }

.twitter:hover { background-color: #2094dd !important; }

.facebook {
  background-position: -2px -27px;
  top: 42%;
  left: -10%; }

.facebook:hover { background-color: #3b5998 !important; }

.content {
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
  border-radius: 10px;
  position: relative;
  float: left;
  margin-left: 20px;
  padding: 15px 25px;
  width: 510px;
  border-width: 1px 4px 4px 3px;
  border-style: solid;
  border-color: #c8c7b4;
  background-color: #ece5bd;


  background-image: -linear-gradient(0deg, transparent 18px, #dbada9 0, #dbada9 20px, transparent 19px),
                    -linear-gradient(#e1dab0 0.1em, transparent 0.1em);
  background-image: -webkit-linear-gradient(0deg, transparent 11px, #dbada9 0, #dbada9 14px, transparent 12px),
                    -webkit-linear-gradient(#e1dab0 0.1em, transparent 0.1em);
  background-image: -moz-linear-gradient(0deg, transparent 11px, #dbada9 0, #dbada9 13px, transparent 12px),
                    -moz-linear-gradient(#e1dab0 0.1em, transparent 0.1em);
  background-size: 100% 10px;
  color: #333;

}

.content:after, .content:before {
  border-bottom: 23px solid transparent;
  border-right: 20px solid #ece5bd;
  top: 49px;
  content: '';
  position: absolute;
  left: -9px;
  -webkit-transform: rotate(220deg);
  -moz-transform: rotate(220deg);
  -o-transform: rotate(220deg);
  transform: rotate(220deg); }

.content h3 {
  font: 23px "Satisfy";

  margin: 0;
  padding: 0;
  font-weight: normal; }

.content p {
  margin: 10px 0 0 0;
  font-size: 15px;
  font-style: italic;
   }

.content p a {
  text-decoration: none;
  background-color: #f7f3c5;
  border-bottom: solid 1px #cfcebe;
  color: #834202;
  padding: 1px 4px; }

.content p a:hover { background-color: #f5ec82; }

.content b {
  display: block;
  color: #75280c;
  font: italic normal 17px Georgia; }

.content:before {
  top: 48px;
  left: -11px;
  border-right: 19px solid rgba(0, 0, 0, 0.1); }

@media all and (max-width: 1024px) and (min-width: 568px){
  .backgroundCommentImage {height: 1200px; }
}


</style>


