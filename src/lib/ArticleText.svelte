<script>
    let { children } = $props();
</script>

<div class="article-text">
    <p>
        {@render children()}
    </p>
</div>

<style>
    .article-text {
        margin: 50vh auto;
        width: 50%;
        background-color: #97976a;
        color: #f7efda;
        border: solid #6f5e4f 3px;
        border-radius: 20px;
        padding: 20px;
        box-shadow: 16px 16px #df949d;
    }
</style>
