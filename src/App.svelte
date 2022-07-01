<script>
  import landing_photo from "../src/assets/landing_photo.png";
  import next_icon from "../src/assets/icons/next_icon.png";
  import chess_icon from "../src/assets/icons/chess_icon.png";

  import SecondPage from "./SecondPage.svelte";

  let secondPage = false;

  function setSecondPage() {
    secondPage = !secondPage
  }

</script>

<div class="wrapper">

  {#if secondPage}
    <SecondPage />

  {:else}
    <div class="left-side">
      <div class="indigo-cup">
        <span>
          <img src={chess_icon} alt="chess_icon">
          Redberry Knight Cup</span>
      </div>
    </div>
    <div class="right-side">
      <div class="big-text">
        chess says
        <span>a lot about</span>
        <br />
        who we are
      </div>
      <button
        on:click={setSecondPage}
        class="start_btn"
        >
        <span>Get Started</span>
        <img src={next_icon} alt="next_icon"/>
      </button>
    </div>


  {/if}



</div>

<style>
  @font-face {
    font-family: "Nunito";
    src: url("../src/assets/fonts/Nunito/Nunito-Bold.ttf");
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
    background: url("../src/assets/landing_photo.png");
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
    background-color: #fd5334;
    padding-top: 7rem;
    padding-left: 3rem;
  }

  .big-text {
    font-size: 4rem;
    color: white;
    text-transform: uppercase;
    font-family: "Nunito";
    font-weight: bold;
  }

  .big-text span {
    color: #333;
    font-size: 1rem;
  }

  .start_btn {
    background-color: #212529;
    border: none;
    border-radius: 8px;
    color: white;
    padding: 0.2rem 1rem;
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 10px 24px;
    margin-top: 5rem;
    cursor: pointer;
    font-family: "Open Sans";
    font-size: 15px;
  }

</style>
