<div id="container">
    <div id="title">
        <h1>I'm <span class="text-gradient">Addy Bhatia</span></h1>
        <img src='meinspace.png' alt=''/>
    </div>
    <div id="space">
        <div class="stars"></div>
        <div class="stars"></div>
        <div class="stars"></div>
        <div class="stars"></div>
        <div class="stars"></div>
    </div>
</div>

<style>
    #container {
        background: #000;
        height: 100vh;
        display: flex;
        align-items: center;
    }

    #title {
        display: flex;
        max-width: 60ch;
        margin: auto;
        align-items: center;
        z-index: 10;
    }

    h1 {
        justify-content: left;
        color: white;
    }

    img {
        animation: bounce 5s infinite;
    }

    .text-gradient {
		font-weight: 900;
		background-image: var(--astro-gradient);
        background-clip: text;
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-size: 100% 200%;
		background-position-y: 100%;
		border-radius: 0.4rem;
		animation: pulse 4s ease-in-out infinite;
	}

    @keyframes bounce {
        0% {
            transform: translateY(0);
        }
        50% {
            transform: translateY(-10px);
        }
        100% {
            transform: translateY(0);
        }
    }

    /* Stars 
    ------------------------------------- */

    #space, .stars {
        overflow: hidden;
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
    }

    .stars {
    background-image: 
        radial-gradient(1px 1px at 20px 30px, #eee, rgba(0,0,0,0)),
        radial-gradient(1px 1px at 40px 70px, #fff, rgba(0,0,0,0)),
        radial-gradient(1px 1px at 50px 160px, #ddd, rgba(0,0,0,0)),
        radial-gradient(1px 1px at 90px 40px, #fff, rgba(0,0,0,0)),
        radial-gradient(1px 1px at 130px 80px, #fff, rgba(0,0,0,0)),
        radial-gradient(1px 1px at 160px 120px, #ddd, rgba(0,0,0,0));
    background-repeat: repeat;
    background-size: 200px 200px;
    animation: zoom 5s infinite;
    opacity: 0;
    }

    .stars:nth-child(1) {
    background-position: 50% 50%;
    animation-delay: 0s;
    }
    .stars:nth-child(2) {
    background-position: 20% 60%;
    animation-delay: 1s;
    }
    .stars:nth-child(3) {
    background-position: -20% -30%;
    animation-delay: 2s;
    }
    .stars:nth-child(4) {
    background-position: 40% -80%;
    animation-delay: 3s;
    }
    .stars:nth-child(5) {
    background-position: -20% 30%;
    animation-delay: 4s;
    }

    @keyframes zoom {
    0% {
        opacity: 0;
        transform: scale(0.5);
        animation-timing-function: ease-in;
    } 
    85% {
        opacity: 1;
        transform: scale(2.8);
        animation-timing-function: linear;
    }
    100% {
        opacity: 0;
        transform: scale(3.5);
    }
    }
</style>