<script lang="ts">
</script>

<div class="love">
  <div class="container" style="margin-left: 900px; margin-top: 300px;">
    <span>T</span>
    <span>E</span>
    <span>A</span>
    <span>M</span>
    <span>O</span>
  </div>
  <div>
    <div class="heart"></div>
  </div>
</div>

<style>
  .love {
    width: 100%;
    min-height: 500vh;
    min-width: 500vh;
    display: flex;
    background: #0b1522;
  }
  .container > span {
    position: relative;
    font-size: 5rem;
    justify-content: center;
    align-items: center;
    white-space: nowrap;
    font-family: "baloo Thambi", cursive;
    animation: glow 2s ease-in-out infinite;
    &:before {
      content: "[";
    }

    &:after {
      content: "]";
    }
  }
  @keyframes glow {
    0%,
    100% {
      color: #fff;
      text-shadow:
        0 0 12px #f20044,
        0 0 50px #f20044,
        0 0 100px #f20044;
    }
    10%,
    90% {
      color: #111;
      text-shadow: none;
    }
  }
  .container > span:nth-child(2) {
    animation-delay: 0.25s;
  }
  .container > span:nth-child(3) {
    animation-delay: 0.5s;
  }
  .container > span:nth-child(4) {
    animation-delay: 0.75s;
  }
  .container > span:nth-child(5) {
    animation-delay: 1s;
  }

  .heart {
    position: relative;
    height: 70px;
    width: 70px;
    background-color: #f20044;
    margin-left: -350px;
    margin-top: 500px;
    transform: rotate(-45deg);
    box-shadow: -10px 10px 90px #f20044;
    animation: heart 0.6s linear infinite;
  }
  @keyframes heart {
    0% {
      transform: rotate(-45deg) scale(1.07);
    }
    80% {
      transform: rotate(-45deg) scale(1);
    }
    100% {
      transform: rotate(-45deg) scale(0.8);
    }
  }
  .heart::before {
    content: "";
    position: absolute;
    height: 70px;
    width: 70px;
    background-color: #f20044;
    top: -50%;
    border-radius: 50px;
    box-shadow: -10px -10px 90px #f20044;
  }
  .heart::after {
    content: "";
    position: absolute;
    height: 70px;
    width: 70px;
    background-color: #f20044;
    right: -50%;
    border-radius: 50px;
    box-shadow: 10px 10px 90px #f20044;
  }
</style>
