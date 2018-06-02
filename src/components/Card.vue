<template>
    <b-card-group deck>
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top>
            <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
            <b-button href="#" variant="primary">Go somewhere</b-button>
        </b-card>
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top>
            <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
            <b-button href="#" variant="primary">Go somewhere</b-button>
        </b-card>
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top>
            <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
            <b-button href="#" variant="primary">Go somewhere</b-button>
        </b-card>
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top>
            <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
            <b-button href="#" variant="primary">Go somewhere</b-button>
        </b-card>
    </b-card-group>
</template>

<script>
export default {
  name: "card"
};
</script>

<style scoped>
.card-deck {
  display: flex;
  justify-content: center;
  flex-flow: row wrap;
  align-items: stretch;
}
.card-deck .card {
  display: block;
  flex-grow: 0;
  flex-basis: 22%;
  margin-bottom: 1rem;
}
</style>


