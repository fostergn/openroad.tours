<template>
  <footer>
    <ul>
      <li><a href="/tours">Tours</a></li>
      <li><a href="/terms">Terms</a></li>
      <li><a href="/contact">Contact Us</a></li>
    </ul>
    <ul>
      <li class="facebook">
        <a href="https://www.facebook.com/OpenRoadToursSEA/" target="_blank">
          <icon name="brands/facebook-f" size="l"></icon>
        </a>
      </li>
      <li>
        <a href="https://www.instagram.com/openroadtours/?hl=en" target="_blank">
          <icon name="brands/instagram" size="l"></icon>
        </a>
      </li>
    </ul>
  </footer>
</template>

<style lang="scss" scoped>
  footer {
    font-size: .8rem;
    background-color: #f5f5f5;
    padding: 1rem 6rem 1rem 3rem;
    color: #888;
    display:flex;
    justify-content:space-between;
    align-items:center;

    & ul:first-child {
      li {
        margin-right:10px;
      }
    }

    & ul:nth-child(2) {
      font-color:#666;
      li {
        margin-left:20px;
      }
    }

    & >ul {
      display:flex;
      align-items:center;
    }
  }

  .fa-icon {
      width: auto;
      height: 1.8em;
      max-width: 100%;
      max-height: 100%;
  }

  .facebook {
    height:1.5em;
  }

</style>
