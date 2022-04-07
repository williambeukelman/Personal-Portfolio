<style>
  @import url("https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@700&display=swap");
  .container-fluid {
    box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
      rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
  }
  .projectBox {
    width: 100%;
    overflow-x: scroll;
    scroll-snap-type: mandatory;
    scroll-snap-points-y: repeat(22rem);
    scroll-snap-type: y mandatory;
  }
  .card {
    scroll-snap-align: start;
    max-width: 50%;
    min-width: 22rem;
    padding: 0;
    overflow: hidden;
    border-radius: 1rem;
    background-color: transparent;
    color: white;
  }
  .card-img-top {
    height: 100%;
    width: 100%;
    z-index: -1;
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
  let projects = [
    {
      title: "Music Library Application",
      desc:
        "A simple mock music library and player coded in Vue3, HTML, CSS, and JS.",
      demo: "https://v62igf.csb.app/artist",
      code: "https://github.com/williambeukelman/Music-Library-App",
      image:
        "https://camo.githubusercontent.com/ad0810c98f921ee6571c2274ea4398eb022877d97642ea0b974dd482b16db718/68747470733a2f2f77696c6c69616d6265756b656c6d616e2e6769746875622e696f2f6d757369632d706c617965722d616c62756d732e706e67",
      badges: [
        {
          name: "vue3",
          url:
            "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg"
        }
      ]
    },
    {
      title: "Recyclical Energy",
      desc:
        "A mock business website I designed and coded using Bootstrap in a parallax style.",
      demo: "https://owv4in.csb.app/",
      code: "https://github.com/williambeukelman/Recyclical-Energy-Website/",
      image: "https://williambeukelman.github.io/energy-home.png",
      badges: [
        {
          name: "Bootstrap",
          url:
            "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg"
        }
      ]
    },
    {
      title: "Twenty Letter Wordle",
      desc:
        "A Svelte application intended to mimic the game of Wordle but with a much longer letter count",
      demo: "https://s9o1y6.csb.app/",
      code: "https://github.com/williambeukelman/Twenty-Letter-Wordle/",
      image:
        "https://williambeukelman.github.io/screenshot-twenty-letter-wordle.png",
      badges: [
        {
          name: "Svelte",
          url:
            "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/svelte/svelte-original.svg"
        }
      ]
    }
  ];
</script>

<!-- Projects Section -->
<div class="container-fluid my-3 p-2">
	<div class="projectBox d-flex gap-2 flex-row">
  {#each projects as project}
    <div class="card">
      <div class="langs">
      {#each project.badges as badge} 
        <img class="language-badge" src="{badge.url}" alt="{badge.name}-logo" />
      {/each}
      </div>
      <img class="card-img-top" src="{project.image}" alt="project">
      <div class="card-body">
        <h5 class="card-title">{project.title}</h5>
        <p class="card-text">{project.desc}</p>
        <a href="{project.demo}" class="btn btn-outline-danger">Demo</a> 
        <a href="{project.code}" class="btn btn-outline-light">Code</a>
      </div>
    </div>
  {/each}
	</div>
</div>