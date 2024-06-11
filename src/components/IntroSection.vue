<template>
  <section id="intro">
    <div class="intro__inner">
      <h2 class="intro__title">port developer</h2>
      <div class="intro__lines" aria-hidden="true">
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
      </div>
      <div class="intro__text">
        <div class="text">
          <div>Believe you can</div>
          <div>and</div>
          <div>you're halfway there</div>
        </div>
        <div class="img">
          <img src="https://images.unsplash.com/photo-1529139574466-a303027c1d8b?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="나" />
        </div>
      </div>
      <div class="intro__lines" aria-hidden="true">
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
#intro {
  height: 100vh;

  .intro__inner {
    width: 100%;
    height: 130%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 16px;
    text-transform: uppercase;
    background-color: #007481;

    .intro__title {
      font-size: 8.5vw;
      line-height: 1;
      font-weight: 800;
      white-space: nowrap;
      text-transform: uppercase;
      letter-spacing: -0.3vw;
      text-indent: -0.5vw;
      color: #f30017;
      font-family: Dela Gothic One;
    }

    .intro__lines {
      width: 250px;

      .line {
        display: block;
        width: 100%;
        height: 1px;
        background-color: #ea00169c;
        margin-bottom: 0.5vw;

        &:nth-child(1) {
          height: 1px;
        }
        &:nth-child(2) {
          height: 3px;
        }
        &:nth-child(3) {
          height: 7px;
        }
        &:nth-child(4) {
          height: 12px;
        }
        &:nth-child(5) {
          height: 18px;
        }
        &:nth-child(6) {
          height: 24px;
        }
        &:nth-child(7) {
          height: 32px;
        }
      }
      &.bottom {
        display: none;
      }
    }
    .intro__text {
      width: 100%;
      height: 40vh;
      background-color: #024152;
      color: var(--white);
      align-items: center;
      justify-content: center;
      flex-direction: column;
      position: relative;

      .text {
        font-size: 2.8vw;
        line-height: 1;
        font-weight: 900;
        text-transform: uppercase;
        text-decoration: underline;
        text-align: center;
        position: relative;
        z-index: 100;
        transition: all 0.3s;
        cursor: all-scroll;
        color: var(--white);
      }
      .img {
        position: absolute;
        left: 50%;
        top: 60%;
        transform: translate(-50%, -50%);
        width: 30vh;
        height: 30vh;
        border-radius: 50%;
        overflow: hidden;
        filter: grayscale(70%);
        transition: all 0.3s;
        z-index: 1000;
      }
    }
  }
}
</style>
