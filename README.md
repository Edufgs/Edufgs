### Hi there 👋

- 🔭 Atualmente não estou trabalhando
- 🌱 Estou fazendo o curso de Engenharia da Computação e atualmente aprendendo JavaScript

<hr>

<div align="center">

  ![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=Edufgs&show_icons=true&theme=tokyonight&include_all_commits=true)

  [![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Edufgs&layout=compact)](https://github.com/anuraghazra/github-readme-stats)
</div>

<hr>

<div>
  <a href="https://www.youtube.com/channel/UCqQPtmiVCX4bDb6HFwHibyw" target="_blank"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" target="_blank"></a>
  <a href="https://www.instagram.com/edu_gon_silva/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a href = "edu.fgs14@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://steamcommunity.com/id/Edufgs" target="_blank"><img src="https://img.shields.io/badge/Steam-000000?style=for-the-badge&logo=steam&logoColor=white" target="_blank"></a>
  
  <img align="right" alt="Rafa-pic" height="150" style="border-radius:50px;" src="https://user-images.githubusercontent.com/44234388/137406055-a655eb7a-db0f-46f5-b5be-6c9895327c40.gif">
</div>

<hr>
@primaryClr: #fed75a; // Adjust this value to change the color
@pacman-zise: 70px;

body {
  background: #1d1d1d;
  height: 100%;
}

.pac-man {
  border-radius: 50%;
  margin: 0 auto;
  margin-top: calc(50%
    - (@pacman-zise / 2));
  border-radius: 100em 100em 0 0;
  background: #f00;
  transform-origin: bottom;
  animation: eating-top .5s infinite;
  
  &, &::before {
    width: @pacman-zise;
    height: calc(@pacman-zise/2);
    background: @primaryClr;
  }
  
  &::before {
    content: '';
    display: block;
    margin-top: calc(@pacman-zise/2);
    position: absolute;
    transform-origin: top;
    border-radius: 0 0 100em 100em;
    transform: rotate(80deg);
    animation: eating-bottom .5s infinite;
  }
  
  &::after {
    position: absolute;
    border-radius: 100em;
    content: '';
    display: block;
    height: 20px;
    width: 20px;
    margin-top: calc((@pacman-zise / 2) - 10px);
    margin-left: calc((@pacman-zise / 2) - 10px);
    transform-origin: center;
    animation: 
      center .5s infinite,
      ball .5s -.33s infinite linear;
  }
}

@keyframes eating-top{
  0%{ transform: rotate(-40deg); }
  50% { transform: rotate(0deg); }
  100%{ transform: rotate(-40deg); }
}

@keyframes eating-bottom{
  0%{ transform: rotate(80deg); }
  50% { transform: rotate(0deg); }
  100%{ transform: rotate(80deg); }
}

@keyframes center{
  0%{ transform: rotate(40deg); }
  50% { transform: rotate(0deg); }
  100%{ transform: rotate(40deg); }
}

@keyframes ball{
  0%{ 
    opacity: .7;
    box-shadow: 
      70px 0 0 0 @primaryClr,
      120px 0 0 0 @primaryClr,
      170px 0 0 0 @primaryClr,
      220px 0 0 0 @primaryClr
    ;
  }
  100% { 
    box-shadow: 
      20px 0 0 0 @primaryClr,
      70px 0 0 0 @primaryClr,
      120px 0 0 0 @primaryClr,
      170px 0 0 0 @primaryClr
    ;
  }
  
}
