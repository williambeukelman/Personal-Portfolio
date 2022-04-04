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
			<button type="button" class="btn btn-outline-dark">
				<div class="skill-card">
					<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/svelte/svelte-original.svg" alt="svelte-logo" />
					<span class="badge bg-dark">Svelte</span>
				</div>
			</button>
			<button type="button" class="btn btn-outline-dark">
				<div class="skill-card">
					<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" alt="vue3-logo" />
					<span class="badge bg-dark">Vue3</span>
				</div>
			</button>
			<button type="button" class="btn btn-outline-dark">
				<div class="skill-card">
					<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg" alt="bootstrap-logo" />
					<span class="badge bg-dark">Bootstrap</span>
				</div>
			</button>
		</div>
	</div>
</div>