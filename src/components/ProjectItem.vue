<template>
    <b-card no-body :img-src="'https://picsum.photos/600/300/?image=' + repository.id %100" img-alt="Image" img-top>
        <b-card-body>
            <h5>{{repository.name}}</h5>
             <span><strong>Lang:</strong><i style="color:blue"> {{repository.language}}</i></span>
            <p class="card-text">
                {{repository.description}}
            </p>
        </b-card-body>
        <b-card-body>
            <div class="d-flex flex-row justify-content-center">
                <div class="p-2">
                    <i class="fas fa-code-branch"></i>
                    <span>{{repository.forks_count}}</span>
                </div>
                <div class="p-2">
                    <b-button :href="repository.html_url" variant="outline-primary">
                        <i class="fab fa-github"></i> Open
                    </b-button>
                </div>
                <div class="p-2">
                    <i class="fas fa-star"></i>
                    <span>{{repository.stargazers_count}}</span>
                </div>
            </div>
        </b-card-body>
    </b-card>
</template>

<script>
export default {
  name: "project-item",
  props: ["repository"]
};
</script>


<style scoped>
h5 {
    font-weight: 700;
}
</style>
