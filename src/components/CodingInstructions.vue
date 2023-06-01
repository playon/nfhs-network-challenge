<template>
  <div class="instructions">
    <section>
      <img alt="Vue logo" src="../assets/logo.svg">
      <h1>{{ title }}</h1>
      <p>
        Congrats, you got the project running!
      </p>
      <small>
        Instructions for this challenge can be found in the <a href="https://github.com/playon/nfhs-network-challenge#readme" target="_blank">README.md</a> file located at the root of the project.
        We just wanted to say, thank you for taking the time to work on this coding challenge and we look forward to seeing what you do with it!
      </small>
    </section>
  </div>
</template>

<script>
export default {
  name: 'CodingInstructions',
  props: {
    title: String
  }
}
</script>

<style lang="less" scoped>
  @import '../assets/variables.less';

  .instructions {
    word-wrap: break-word;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    height: calc(100vh - 15em);
    flex-wrap: nowrap;

    section {
      max-width: 28rem;
      margin: 0 auto;
    }

    a {
      font-weight: 800;
      color: @color-accent;
      text-decoration: none;

      &:visited {
        color: lighten(@color-accent, 10%);
      }
    }

    img {
      height: auto;
      width: 50%;
      max-width: 120px;
    }

    p, small {
      line-height: 1.5rem;
    }
  }
</style>
