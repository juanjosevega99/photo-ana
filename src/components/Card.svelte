<script>
  import Comments from './Comments.svelte'
</script>

<style>
  .Card {
    border: 1px solid rgba(219, 219, 219, 1);
    border-radius: 4px;
    background-color: white;
    margin: 0 0 2em 0;
  }
  .Card-Header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1em;
  }
  .Card-user {
    display: flex;
    align-items: center;
    justify-content: flex-end;
  }
  .Card-user img {
    width: 32px;
    height: 32px;
    border-radius: 50%;
  }
  .Card-user h2 {
    margin: 0;
    padding: 0;
    font-size: 14px;
    font-weight: 600;
    margin: 0 0 0 1em;
    color: black;
  }
  .Card-user h2 span {
    display: block;
    font-size: 12px;
    font-weight: normal;
    color: rgba(38, 38, 38, 0.7);
  }
  .Card-photo {
    padding: 0;
    margin: 0;
  }
  .Card-photo img {
    width: 100%;
    height: auto;
  }
  .Card-photo figure {
    margin: 0;
    padding: 0;
    cursor: pointer;
  }
  .Card-settings i {
    cursor: pointer;
  }
  .Card-icons {
    padding: 1em;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .Card-icons i {
    margin: 0 1em 0 0;
    cursor: pointer;
    font-size: 20px;
  }
  .Card-icons i:last-child {
    margin: 0;
  }
  .Card-description {
    padding: 0 1em 1em 1em;
  }
  .Card-description h3 {
    font-size: 14px;
    font-weight: bold;
    color: black;
  }
  .Card-description span {
    font-size: 14px;
  }
  .active-like {
    color: #bc1888;
    animation: bounce linear 0.8s;
    animation-iteration-count: 1;
    transform-origin: 20% 20%;
  }
  .active-bookmark {
    color: #f09433;
  }

  @keyframes bounce {
    0% {
      transform: translate(0px, 0px);
    }
    15% {
      transform: translate(0px, -25px);
    }
    30% {
      transform: translate(0px, 0px);
    }
    45% {
      transform: translate(0px, -15px);
    }
    60% {
      transform: translate(0px, 0px);
    }
    75% {
      transform: translate(0px, -5px);
    }
    100% {
      transform: translate(0px, 0px);
    }
  }
</style>

<div class="Card">
  <div class="Card-container">
    <div class="Card-Header">
      <div class="Card-user">
        <img src="https://instagram.fnva1-1.fna.fbcdn.net/v/t51.2885-19/s150x150/93571183_700157570811057_7056976415194873856_n.jpg?_nc_ht=instagram.fnva1-1.fna.fbcdn.net&_nc_ohc=_cTj6kBSRSEAX_mFVf2&oh=737d31baa078beb7c27db72698b2ba39&oe=5EC6C750" alt="">
        <h2>
          manuelaarias_98
          <span>Huila, Colombia</span>
        </h2>
      </div>
      <div class="Card-settings">
        <i class="fas fa-ellipsis-h" />
      </div>
    </div>
    <div class="Card-photo">
      <figure>
        <img src="https://instagram.fnva1-1.fna.fbcdn.net/v/t51.2885-15/e35/p1080x1080/75358229_151183719510830_145204898161177428_n.jpg?_nc_ht=instagram.fnva1-1.fna.fbcdn.net&_nc_cat=102&_nc_ohc=BVwn8gSEelcAX_BOIQk&oh=a1103b21b563c4fa50f02f9909327daa&oe=5EC4F6AE" alt="">
      </figure>
    </div>
    <div class="Card-icons">
      <div class="Card-icons-firsts">
        <i class="fas fa-heart" />
        <i class="fas fa-paper-plane" />
      </div>
      <div class="Card-icons-second">
        <i class="fas fa-bookmark" />
      </div>
    </div>
    <div class="Card-description">
      <h3>manuelaarias_98</h3>
      <span>Estudio, tomo café y leo; cazo atardeceres y tengo flores amarillas enterradas bajo la piel.</span>
    </div>
    <Comments />
  </div>
</div>