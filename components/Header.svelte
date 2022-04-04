<script>
  import profilePic from "../assets/avatar_sweater_transparent.png";
</script>

<style>
  /** Temp Mobile dev settings **/
  div.container {
    max-width: 450px;
    min-width: 450px;
  }
  .profile {
    max-width: 12rem;
    background: linear-gradient(tomato, blueviolet);
    filter: grayscale(0.3);
  }
  .section-header {
    background-color: black;
    color: white;
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
  h2 {
    text-transform: uppercase;
    opacity: 0.6;
    line-height: 50%;
  }
  .page-divider svg {
    width: 100%;
    max-height: 4rem;
  }
</style>

<div class="container-fluid section-header">
  <div class="container py-3">
    <div class="row">
      <div class="col">
        <img src={profilePic} class="img img-fluid profile rounded-circle" alt="profile">
        <h1>William Beukelman</h1>
        <h2>Tagline about me</h2>
      </div>
    </div>
  </div>
  <!--
  <span class="page-divider">
    <svg>
      <path d="M 205,5 L 1140,5 L 1140,295 L 0,65 L 1140,5 z" id="path59" style="fill:white;stroke:none" />    </svg>
  </span>
  -->
</div>