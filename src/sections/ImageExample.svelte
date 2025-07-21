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
                    As a Latina currently in a STEM major, I am curious to learn 
                    more about what might be preventing Hispanic women 
                    from entering the STEM job field, even after earning their 
                    degree.
                </strong>
            </ArticleText>

            <ArticleText><strong>
                Though there are low employment rates in the STEM field for Hispanic women, 
                they still saw about a 2% increase between the years 2019 and 2021. This goes to show 
                that even with barriers in their way at times, Latinas are determined in paving their 
                ways into  STEM careers.
                </strong>
            </ArticleText>
        {/snippet}
    </Scroller>
</div>

<style>
    .stem-img {
        width: 90%;
        margin: 0px auto;
    }
</style>
