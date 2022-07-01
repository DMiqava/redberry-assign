<script>
    import second_page from "../src/assets/second_page.png";
    import chess_icon from "../src/assets/icons/chess_icon.png";
    import next_icon from "../src/assets/icons/next_icon.png";
</script>

<div class="wrapper">
    <div class="left-side">
        <div class="indigo-cup">
            <span>
                <img src={chess_icon} alt="chess_icon" />
                Redberry Knight Cup
            </span>
        </div>
        <div class="text">
            "when you see a good move,<br /> look for a better one"<br />
        </div>
        <div class="name">- emanuel lasker</div>
    </div>
    <div class="right-side">
        <div class="top_div">
            <p>Start creating your account</p>
        </div>

        <div class="personal">Personal Information</div>
        <div class="subtitle">This Is Basic Information Fields</div>

        <input type="text" required placeholder="Name*" /><br />
        <input type="email" required placeholder="Email address*" /><br />
        <input type="number" required placeholder="Phone number*" /><br />
        <input type="text" required placeholder="Date of birth*" /><br />

        <div class="btn_wrapper">
            <button class="back">
                <span>Back</span>
            </button>
            <button class="next">
                <span>Next</span>
                <img src={next_icon} alt="next_icon" />
            </button>
        </div>
    </div>
</div>

<style>
    @font-face {
        font-family: "Nunito";
        src: url("../src/assets/fonts/Nunito/Nunito-Regular.ttf");
    }

    @font-face {
        font-family: "Open Sans";
        src: url("../src/assets/fonts/OpenSans/OpenSans-Regular.ttf");
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
        position: relative;
        font-family: "Open Sans";
        font-weight: 600;
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

    .name {
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
        text-align: center;
        width: 100%;
        display: flex;
        padding-left: 1px;
        margin-top: 1rem;
        border: 1px solid #212529;
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
        color: #95939a;
        font-size: 11px;
    }

    .top_div {
        border-bottom: 1px solid #B9B4C34D;
        height: 83px;
        width: 100%;
        display: flex;
        align-items: center;
        position: absolute;
        top: 0;
        left: 0;
        padding-left: 3rem;
    }

    .right-side input {
        font-family: "Open Sans";
        background-color: white;
        border: none;
        font-size: 16px;
        margin-top: 3rem;
        box-shadow: inset 0px -1px 0px rgba(0, 0, 0, 0.125);
        border-radius: 4px;
        width: 750px;
        height: 46px;
    }
    .right-side input :hover {
        color: black;
    }
    
    .btn_wrapper {
        display: flex;
        justify-content: space-between;
        max-width: 750px;
        margin-top: 4rem;
    }


    .next {
        background-color: #212529;
        border: none;
        border-radius: 8px;
        color: white;
        display: flex;
        align-items: center;
        gap: 10px;
        padding: 10px 24px;
        cursor: pointer;
        font-family: "Open Sans";
        font-size: 15px;
    }
    .back {
        background-color: white;
        padding: 10px 24px;
        cursor: pointer;
        gap: 10px;
        align-items: center;
        font-size: 15px;
        font-family: "Open Sans";
        border: 1px solid black;
        border-radius: 8px;
    }

    .back:hover{
        background-color: #f5f5f5;
    }
</style>
