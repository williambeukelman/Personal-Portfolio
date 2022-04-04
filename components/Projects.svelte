<style>
  @import url("https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@700&display=swap");
  .container-fluid {
    box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
      rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
  }
  .card {
    max-width: 50%;
    padding: 0;
    overflow: hidden;
    border-radius: 1rem;
  }
  .card-img-top {
    width: 100%;
    filter: blur(1px);
    scale: 1.05;
    transition: all 0.3s linear;
  }
  .card:hover .card-img-top {
    scale: 1.1;
    filter: blur(2px);
    cursor: pointer;
  }
  .card-body {
    background: linear-gradient(to top, black, transparent);
    margin-top: -10rem;
  }
  .card-title {
    font-family: "Roboto Condensed", sans-serif;
    font-size: 1.5rem;
    background: linear-gradient(to left, tomato, blueviolet);
  }
  .language-badge {
    max-width: 3rem;
    max-height: 3rem;
    position: absolute;
    z-index: 1;
    right: 1rem;
    border-bottom: 5px solid white;
  }
</style>

<script>
</script>

<!-- Projects Section -->
<div class="container-fluid my-3 p-2">
	<div class="row d-flex justify-content-center">
    <div class="card">
      <img class="language-badge" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" alt="vue3-logo" />
      <img class="card-img-top" src="https://camo.githubusercontent.com/ad0810c98f921ee6571c2274ea4398eb022877d97642ea0b974dd482b16db718/68747470733a2f2f77696c6c69616d6265756b656c6d616e2e6769746875622e696f2f6d757369632d706c617965722d616c62756d732e706e67" alt="project">
      <div class="card-body">
        <h5 class="card-title">Music Library Application</h5>
        <p class="card-text">A simple mock music library and player coded in Vue3, HTML, CSS, and JS.</p>
        <a href="https://v62igf.csb.app/artists" class="btn btn-outline-danger">Demo</a> 
        <a href="https://github.com/williambeukelman/Music-Library-App" class="btn btn-outline-light">Code</a>
      </div>
    </div>
	</div>
</div>