<script>
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";
</script>

<div>
    <Scroller layout="right">
        {#snippet sticky()}
           

            <img class="stem-img" src="https://media.licdn.com/dms/image/v2/D4E22AQE0XkpXA6CPzA/feedshare-shrink_2048_1536/feedshare-shrink_2048_1536/0/1685726352513?e=2147483647&v=beta&t=jh0ED1gO9tAAfj9RorFRxpxf_gEEZLfFQ6BpZ6iZaeY" alt="Si Se Puede!" />           

        {/snippet}

        
        {#snippet scrolly()}
            <ArticleText>
                <strong>
                    Through the !
                </strong>
            </ArticleText>

            <ArticleText>It's yours to create.</ArticleText>
        {/snippet}
    </Scroller>
</div>

<style>
    .stem-img {
        width: 90%;
        margin: 0px auto;
    }
</style>
