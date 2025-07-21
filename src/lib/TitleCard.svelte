<script>
    let { title, subtitle} = $props();
</script>

<div class="title-card">
    <div class="content">
        <h1>{title}</h1>
        <h2>{subtitle}</h2>
    </div>
</div>

<style>
    .title-card {
        background-image: linear-gradient(#E7CCCC,#EDE8DC, #C1CFA1);
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 2rem;
        box-sizing: border-box;
        font-family: "Inter", sans-serif;
    }

    .content {
        max-width: 700px;
        background-color:#6f5e4f;
        padding: 2rem;
        border: 6px solid #df949d;
        border-radius: 2rem;
        box-shadow: 16px 16px #6f5e4f91;
    }

    h1 {
        font-size: 3rem;
        margin: 0;
        color: #df949d;
        text-shadow: 1px 1px 0 	#e3bbbd;
        font-family: Gelasio;
    }


    h2 {
        font-size: 1.5rem;
        color: #f7f5eb;
        margin-top: 1rem;
        font-family: Gelasio;
    }

   
    @media (max-width: 600px) {
        h1 {
            font-size: 2.2rem;
        }

    }
</style>
