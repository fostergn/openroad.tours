<template>
  <footer>
    <ul>
      <li>Tours</li>
      <li>Blog</li>
      <li>Terms</li>
      <li>Contact Us</li>
    </ul>
    <ul>
      <li class="facebook">
        <icon name="brands/facebook-f" size="l"></icon>
      </li>
      <li>
        <icon name="brands/instagram" size="l"></icon>
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
