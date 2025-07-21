<script>
    import * as Highcharts from "highcharts";
    import "highcharts/modules/exporting";
    import { Chart } from "@highcharts/svelte";
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";


    let degreeData = "https://i.imgur.com/bxiacMI.png"; 
    let debtData = "https://i.imgur.com/EI1XNW2.png";


</script>





<div>
    

    <Scroller layout="right">
        {#snippet sticky()}
            <p>
            <br><br><br><br><br><br><br>
            </p>


            <h3>Data Collected by BWDC:</h3>
            <img class="chartImg" src={degreeData} alt="STEM vs. non STEM Employment Rates among female hispanics" />

            <p>STEM vs. non-STEM Employment Rates Among 25-34 Year Olds with a STEM Degree </p>

            <img class="chartImg"  src={debtData} alt="Median total debt for households" />

            <p>Median Total Debt for Households. by Race/Ethnicity</p>




    
            <p>
                Since we're using Highcharts through Svelte, the syntax is a
                little different from what you might see in the demos. But all
                of Highcharts' functionality is available through the Highcharts
                for Svelte package.
            </p>
            <p>
                The configuration is done through the
                <code>options</code> json object passed to the chart, which you'll
                see in the source code for this template.
            </p>
            <p>
                Use the
                <a href="https://api.highcharts.com/highcharts/"
                    >API reference</a
                >
                to understand what each element in the <code>options</code> object
                does.
            </p>


        {/snippet}

        

        {#snippet scrolly()}
            <ArticleText>
                <strong> While exploring the BWDC site, I found it interesting 
                    that in both 2019 and 2021, Hispanic females with STEM 
                    degrees had some of the lowest rates of STEM employment 
                    (24.9% and 26.4% respectively) compared to other racial 
                    and gender groups.
                </strong>
            </ArticleText>

            <ArticleText>
                <strong>As a Hispanic female currently in a STEM major, I became curious to learn 
                more about what barriers might be preventing Hispanic women 
                from entering the STEM job field, even after earning their 
                degree. </strong>
            </ArticleText>

            <ArticleText>
                Follwoing the first imsight, I came across the chart that depicts Hispanic women
                holding the highest debt in comparison to other women in different racial groups.
                <br /><br />
                Or, if you want to build something from scratch, you can use it as
                a <strong>reference</strong> for specific functionality.
            </ArticleText>

            <ArticleText>
                This is <strong>just one way</strong> that scrollytelling can
                look.
                <br /><br />
                <strong>
                    If you use this template, be sure to modify it and make it
                    your own!
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
