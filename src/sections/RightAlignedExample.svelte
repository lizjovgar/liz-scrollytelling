<script>
    import * as Highcharts from "highcharts";
    import "highcharts/modules/exporting";
    import { Chart } from "@highcharts/svelte";
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";


    let degreeData = "https://i.imgur.com/bxiacMI.png"; 
    let debtData = "https://i.imgur.com/EI1XNW2.png";
    let latinasInStem = "https://moirastudio.com/wp-content/uploads/2024/03/Latinas-in-stem_Blog-Thumbnail.jpg";
    let siSePuede = "https://media.licdn.com/dms/image/v2/D4E22AQE0XkpXA6CPzA/feedshare-shrink_2048_1536/feedshare-shrink_2048_1536/0/1685726352513?e=2147483647&v=beta&t=jh0ED1gO9tAAfj9RorFRxpxf_gEEZLfFQ6BpZ6iZaeY";

</script>





<div>
    

    <Scroller layout="right">
        {#snippet sticky()}

            <h3>
                Data Insights:
                
            </h3>


            <img class="chartImg" src={degreeData} alt="STEM vs. non STEM Employment Rates among female hispanics" />

            <p>STEM vs. non-STEM Employment Rates Among 25-34 Year Olds with a STEM Degree </p>



            <p>
                <br>
            </p>




            <img class="chartImg"  src={debtData} alt="Median total debt for households" />

            <p>Median Total Debt for Households. by Race/Ethnicity</p>



        {/snippet}

        

        {#snippet scrolly()}
            <ArticleText>
                <strong> While exploring the BWDC site, it caught my attention 
                    that in both 2019 and 2021, Hispanic females with STEM 
                    degrees had some of the lowest rates of STEM employment 
                    (24.9% and 26.4% respectively) compared to other racial 
                    and gender groups.
                </strong>
            </ArticleText>

            <ArticleText>
                <strong>Following the first insight, I came across the chart that depicts Hispanic women
                    holding the highest debt in comparison to other women in different racial groups. Both data
                    sets combined, this can indicate possible systemic barrier for Latinas when it comes to 
                    the economic return of education.
                     </strong>
            </ArticleText>

            <ArticleText><strong>
                This mismatch brings out the Harsh reality for Latinas in STEM: 
                They go for the high educational investment 
                (which for most is associated with debt), but have limited access to high-paying roles 
                that would make that investment sustainable.
            </strong>

            </ArticleText>

        {/snippet}
    </Scroller>
</div>

<style>
    .chart {
        width: 90%;
        margin: 0px auto;
    }


    .chartImg {
    display: block;
    max-width: 90%;
    margin: 1px auto;
    border-radius: 12px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }   
</style>
