<script>
    import second_page from "../src/assets/second_page.png";
    import chess_icon from "../src/assets/icons/chess_icon.png";
</script>

<div class="wrapper">
    <div class="left-side">
        <div class="indigo-cup">
            <span>
                <img src={chess_icon} alt="chess_icon"/>
                Redberry Knight Cup
            </span>
        </div>
        <div class="text"> "when you see a good move,<br> look for a better one"<br></div>
        <div class="name">- emanuel lasker</div>
    </div>
    <div class="right-side">
        <div class="title">
            Start Creating Your Account
        </div>

        <div class="personal">Personal Information</div>
        <div class="subtitle">This Is Basic Information Fields</div>

        <input type="text" required placeholder="Name*">
        <input type="email" required placeholder="Email address*">
        <input type="number" required placeholder="Phone number*">
        <input type="date" required placeholder="Date of birth*">
    </div>
</div>

<style>
    @font-face {
      font-family: "Nunito";
      src: url("../src/assets/fonts/Nunito/Nunito-Regular.ttf");
    }
  
    @font-face {
      font-family: "Open Sans";
      src: url("../src/assets/fonts/OpenSans/OpenSans-Regular.ttf")
    }
  
    :global(body) {
      margin: 0;
      padding: 0;
    }
  
    .wrapper {
      display: flex;
      width: 100%;
      height: 100vh;
    }
  
    .left-side {
      background: url("../src/assets/second_page.png");
      background-size: cover;
      width: 100%;
    }
  
    .indigo-cup {
      background-color: #7025fb;
      height: 84px;
      width: 100%;
      display: flex;
      align-items: center;
      padding-left: 3rem;
    }
  
    .indigo-cup span {
      color: white;
      font-size: 1.3rem;
      font-family: "Nunito";
    }
  
    .right-side {
      width: 100%;
      background-color: white;
      padding-top: 1rem;
      padding-left: 3rem;
    }

    .text {
        font-family: "Nunito";
        color: #212529;
        font-style: italic;
        font-size: 20px;
        text-transform: uppercase;
        font-weight: 800;
        padding-top: 10rem;
        padding-left: 4rem;
    }

    .name{
        font-family: "Nunito";
        font-style: italic;
        font-size: 20px;
        text-transform: uppercase;
        padding-left: 4rem;
        padding-top: 1rem;
        color: white;
        font-weight: 100;

    }
    .title {
      width: 100%;
      display: flex;
      padding-left: 1px;
      font-family: "Open Sans";
      font-weight: 600;
      font-size: 13px;
    }

    .personal {
        font-family: "Open Sans";
        font-weight: 600;
        font-size: 25px;
        margin-top: 10rem;
    }

    .subtitle {
        font-family: "Open Sans";
        color: #95939A;
        font-size: 11px;
    }

    
  
  
  </style>
