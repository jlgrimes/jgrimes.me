<style lang="scss">
  :root {
    /* https://coolors.co/palette/f8f9fa-e9ecef-dee2e6-ced4da-adb5bd-6c757d-495057-343a40-212529 */
    --gray-100: #f8f9fa;
    --gray-200: #e9ecef;
    --gray-300: #dee2e6;
    --gray-400: #ced4da;
    --gray-500: #adb5bd;
    --gray-600: #6c757d;
    --gray-700: #495057;
    --gray-800: #343a40;
    --gray-900: #212529;
  }

  h1, h2 {
    margin: 0;
  }

  h1 {
    font-size: min(5rem, 14vw);
    color: var(--gray-900);
  }

  h2 {
    font-size: min(2rem, 8vw);
    color: var(--gray-600);
  }

  .container {
    display: flex;
    flex-direction: column;
    padding: 20px;
    gap: 8px;
  }

  .header {
    display: flex;
    flex-direction: column;
    padding: 20px 0;
  }

  .card {
    cursor: pointer;

    border-radius: 0.25rem;
    padding: 2rem;
    display: flex;
    flex-direction: column;
    gap: 12px;

    transition: 200ms ease-out;
    transition-property: box-shadow, transform;
    box-shadow: 0 4px 4px var(--gray-500);
    transform: scale(1);

    
    &:hover {
      box-shadow: 0 8px 16px var(--gray-500);
      transform: scale(1.01);
    }

    &__header {
      color: var(--gray-700);
      text-transform: uppercase;
      font-weight: 900;
      letter-spacing: 1px;
      font-size: medium;
    }

    &__description {
      color: var(--gray-800);
      font-size: medium;
    }
  }

  .projects {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 16px
  }
</style>

<div class="container">
  <div class="header">
    <h1>Hi, I'm Jared.</h1>
    <h2>I'm a UX Engineer.</h2>
  </div>
  <div class="projects">
    <div class="card">
      <div class="card__header">
        PokeStats Live
      </div>
      <div class="card__description">
        Changing the way Pokemon TCG players view and interact with tournaments.
      </div>
    </div>
    <div class="card">
      <div class="card__header">
        PokeXWord
      </div>
      <div class="card__description">
        Wordle for Pokemon cards.
      </div>
    </div>
    <div class="card">
      <div class="card__header">
        Bubble
      </div>
      <div class="card__description">
        Swiss tournament generator optimized for procedural efficiency.
      </div>
    </div>
    <div class="card">
      <div class="card__header">
        CEDH Tournament System
      </div>
      <div class="card__description">
        Pairing generator for Magic the Gathering CEDH tournaments.
      </div>
    </div>
  </div>
</div>
