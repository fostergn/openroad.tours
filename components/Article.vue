<template>
  <section>
    <h3>Checklist before arriving to Vietnam</h3>
    <p class="list-head">Documents:</p>
    <ul>
      <li>Passport</li>
      <li>Visa Invitation Letter + 2 Photos + stamping fee $25 in Cash (in US Dollars) + Vietnam immigration Form</li>
      <li>Proof of Medical Insurance</li>
    </ul>

    <p class="list-head">General Packing (in order of importance):</p>
    <ul>
      <li>Gear (Open Road doesn’t supply gear so anything that you feel comfortable driving with should come along. We recommend full faced helmets)</li>
      <li>

        Depending on the time of year the weather in Northern Vietnam is different.

        <ul class="sub-list">
          <p class="list-head sub">Please pack clothes accordingly:</p>
          <li>May - August (hot)</li>
          <li>August - December (medium)</li>
          <li>December - February (can get very cold)</li>
          <li>February - April (medium)</li>
        </ul>

      </li>
      <li>Toiletries</li>
      <li>Camera Equipment</li>
      <li>Phone</li>
      <li>Recreational Items -- Books, etc.</li>
    </ul>
  </section>
</template>

<style lang="scss" scoped>

  h3 {
    font-size:2rem;
    text-align:center;
    margin:4rem 0 2rem;
    opacity:.8;
  }

  p.list-head {
    font-size:1rem;
    color:#323648;
    font-weight:bold;
    padding:.5rem 0;
  }

  p.list-head.sub {
    position: relative;
    left: -1rem;
  }


  ul {
    list-style-type: circle;
    line-height:1.4rem;
    margin-bottom:1rem;
    font-size:.8rem;
    margin-left:2rem;

    &.sub-list {
      padding-left:1rem;
    }
  }
  section {
    width:100%;
    margin:1rem;
    display:flex;
    flex-direction:column;
  }

  .image__wrapper {

    & > img {
      width: 100%;
    }
  }

  .list-second-head {
    font-weight: 600;
    position: relative;
    left: -1rem;
    margin:.5rem 0;
  }

  .price {
    font-family: 'Playfair Display', serif;
  }
</style>
