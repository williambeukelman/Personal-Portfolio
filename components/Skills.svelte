<style>
  /** Temp Mobile dev settings **/
  div.container {
    max-width: 450px;
    min-width: 450px;
  }
  .section-skills {
    background: white;
    color: black;
  }
  .skill-card {
    width: 6rem;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 0.3rem;
  }
  .skill-card img {
    max-width: 3rem;
    padding: 0.2rem;
  }
  .skill-icons button.btn {
    padding: 0 1rem;
    border: none;
  }
  h1::after {
    display: block;
    content: "";
    width: 80%;
    margin-top: 0.1rem;
    margin-right: auto;
    margin-left: auto;
    height: 0.3rem;
    border-radius: 0.5rem;
    background: linear-gradient(to right, tomato, blueviolet);
  }
</style>

<script>
  let skills = [
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/svelte/svelte-original.svg",
      name: "Svelte"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg",
      name: "Vue3"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg",
      name: "Bootstrap"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg",
      name: "C#"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg",
      name: "Flask"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg",
      name: "Git"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg",
      name: "Javascript"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jquery/jquery-original.svg",
      name: "Jquery"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-plain.svg",
      name: "Linux"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg",
      name: "Python"
    },
    {
      url:
        "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/arduino/arduino-original.svg",
      name: "Arduino"
    }
  ];
</script>

<!-- Skills Section -->
<div class="container section-skills">
	<div class="row py-3">
		<div class="col">
			<h1>Skills & Technologies</h1>
			<p>Tap an icon below to filter for projects matching a skill or technology.</p>
		</div>
	</div>
	<div class="row skill-icons">
		<div class="d-flex gap-3 flex-wrap justify-content-between">
      {#each skills as skill}
        <button type="button" class="btn btn-outline-dark">
          <div class="skill-card">
            <img src="{skill.url}" alt="{skill.name}-logo" />
            <span class="badge bg-dark">{skill.name}</span>
          </div>
        </button>
      {/each}
		</div>
	</div>
</div>