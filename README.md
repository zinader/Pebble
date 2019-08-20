html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      height: 100vh;
      font-family: Helvetica;
}

.topnav a {
  float: left;
  display: block;
  color: black;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

.topnav input[type=text] {
  float: right;
  padding: 6px;
  
  border-radius:10%;
  margin-top: 8px;
  margin-right: 16px;
  font-size: 17px;
}

.topnav input[type=text]:hover {
  float: right;
  padding: 6px;
  border: 1px solid black;
  border-radius:10%;
  margin-top: 8px;
  margin-right: 16px;
  font-size: 17px;
}

.left-col, .right-col {
      position: absolute;
      width: 50%;
      height: 100vh;
}

.left-col {
      background: #d45b48;
}

.right-col {
      left: 50%;
}

.upper {
      position: absolute;
      width: 100%;
      height: 50vh;
      background: #4f4538;
      opacity: 0;
      animation: appear-text 0.0001s linear forwards;
      animation-delay: 3s;
}

.bottom {
      position: absolute;
      top: 50%;
      height: 50vh;
      width: 100%;
      background: url(next-cover.jpg) no-repeat 50% 50%;
      background-size: cover;
      opacity: 0;
      animation: appear-text 0.0001s linear forwards;
      animation-delay: 4.2s;
}

@media(max-width: 900px) {
      .left-col {
            width: 100%;
      }
      .right-col {
            top: 100%;
            left: 0%;
            width: 100%;
      }

}

.logo {
      font-family: Poppins;
      color: #5a2020;
      position: relative;
      margin: 1.4em;
      font-size: 4rem;
      font-weight: bolder;
      z-index: 1;
}

.year {
      position: absolute;
      color: #000;
      font-family: Poppins;
      bottom: 8%;
      font-weight: bolder;
      transform: rotate(-90deg);
      left: 0%;
}

.buy {
      color: #f4c8ad;
      text-transform: uppercase;
      font-family: Poppins;
      text-decoration: underline;
      position: absolute;
      right: 0%;
      top: -2.6%;
      margin: 1.4em;
}

.cover {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 45%;
      height: 50%;
      background: url(album-art.jpg) no-repeat 50% 50%;
      background-size: cover;
      opacity: 0;
      animation: appear-text 0.0001s linear forwards;
      animation-delay: 2.6s;

}

.data {
      position: absolute;
      top: 36%;
      left: 33%;
      transform: translate(-50%, -50%);
      color: #cdbba5;
      font-family: Poppins;
      text-transform: uppercase;
      letter-spacing: 4px;
}

#name {
      font-weight: bolder;
}

#artist {
      font-size: 10px;
}

.play, .next ion-icon {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      color: #fff;
      opacity: 0.6;
      border-radius: 50%;
      border: 1px solid rgba(255, 255, 255, 0.3);
      padding: 2em;
}

.about {
      position: absolute;
      top: 40%;
      left: 26%;
      transform: translate(-50%, -50%);
}

.about h1 {
      font-weight: bolder;
      color: #6f6457;
      font-family: Poppins;
      text-transform: uppercase;
}

.about p {
      color: #bcac98;
      font-family: Poppins;
      text-transform: uppercase;
      letter-spacing: 4px;
      font-size: 10px;
      cursor: pointer;
}

.about span:hover {
      text-decoration: underline;
}

.media {
      margin-top: 40px;
}

.media p {
      color: #6f6457;
      margin-bottom: 0;
}

.media ul {
      position: absolute;
      list-style: none;
      left: -24%;
}

.media ul li {
      display: inline-block;
      color: #bcac98;
      padding-right: 10px;
}

.next {
      position: absolute;
      top: 24%;
      left: 16%;
}

.data2 {
      position: absolute;
      top: 12%;
      left: 28%;
      color: #cdbba5;
      font-family: Poppins;
      text-transform: uppercase;
      letter-spacing: 4px;
}

.more {
      position: absolute;
      top: 80%;
      left: 10%;
      font-size: 15px;
      color: #f4c8ad;
      text-transform: uppercase;
      font-family: Poppins;
      text-decoration: underline;
}

.block-cover {
      position: absolute;
      top: 60%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 50%;
      height: 30%;
}

.block-bottom img{
    top:300px;
    margin-top: 80px;
    margin-left: 100px;

	width:50%;
}

.block-cover::after {
     background-image: url("/Users/pulkitaggarwal/Desktop/41eEE4yUooL.jpg");
     
     content: '';
     top: 0;
     left: 0;
     position: absolute;
     width: 0%;
     height: 100%;
    
     animation: rev-block 1.5s cubic-bezier(0.19, 1, 0.22, 1) forwards;
     animation-delay: 1s;
}

@keyframes rev-block {

     0% {
          left: 0;
          width: 0%;
     }
     50% {
          left: 0;
          width: 100%;
     }
     100% {
          left: 90%;
          width: 90%;
     }

}

@keyframes appear-text {

     0% {
          opacity: 0;
     }
     100% {
          opacity: 1;
     }

}

.upper-block {
      position: absolute;
      width: 100%;
      height: 50vh;
}

.upper-block::after {
     content: '';
     top: 0;
     left: 0;
     position: absolute;
     width: 0%;
     height: 100%;
     background: #9a8b78;
     animation: rev-block 1.5s cubic-bezier(0.19, 1, 0.22, 1) forwards;
     animation-delay: 2.4s;
}

#player {
  position: fixed;
  height: 330px;
  width: 300px;
}

/* Apologies for the large base64 image file */



.speakerplay {
  background-position: 0 0;
}

.block-bottom {
      position: absolute;
      top: 50%;
      height: 50vh;
      width: 100%;
}

.block-bottom::after {
     content: '';
     top: 0;
     left: 0;
     position: absolute;
     width: 0%;
     height: 100%;
     background-color: #011;
     animation: rev-block 1.5s cubic-bezier(0.25, 1, 0.22, 1) forwards;
     animation-delay: 3.6s;
}

