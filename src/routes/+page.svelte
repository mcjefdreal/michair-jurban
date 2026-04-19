<script>
    import PollutionHeroPic from "$lib/assets/hero_pic_pollution.jpg";
</script>
<div class="flex flex-col">
    <div class="sticky top-0 z-1 w-auto h-full overflow-hidden">
        <img class="w-full" src={PollutionHeroPic} alt="pollution" />
    </div>

    <div class="z-20 absolute w-auto h-full text-light-cyan text-center shadow-lg bg-jet-black/70 p-4 flex flex-col justify-center gap-4">
        <div class="flex flex-col gap-2">
            <h1 class="font-bold text-8xl">michAIR jURBAN:</h1>
            <h1 class="text-4xl">Exploring the correlation between a region's GDP and the Air Quality Indices (AQI) of its cities</h1>
        </div>
        <span><b>Typst Sheet:</b> Jelo Fan, MJ Pascual, MJ Real</span>
    </div>
    
    <!-- card for research questions -->
    <div class="z-20 text-jet-black text-left shadow-lg bg-light-blue p-4">
        <h1 class="font-bold text-5xl mb-4">Research Questions</h1>
        <div class="flex flex-col gap-2">
            <p class="text-2xl">What are the Air Quality Indices and air pollutant counts of the different cities in the Philippines from January to May of 2025?</p>
            <p class="text-2xl">In the Philippines, what is the correlation between a city's Gross Domestic Product (GDP) and its Air Quality Index?</p>
        </div>
    </div>

    <!-- res hypothesis -->
    <div class="z-20 text-jet-black text-right shadow-lg bg-cool-steel p-4">
        <h1 class="font-bold text-5xl">Research Hypothesis</h1>
        <p class="text-2xl">
            Regions with a higher GDP per capita will have more financial resources to spend on infrastructure 
            (e.g. transportation infrastructure, green spaces, and monitoring systems), 
            thus they would have a higher Air Quality Index than regions with a lower GDP per capita.
        </p>
    </div>
    
    <div class="z-20 text-left text-light-cyan shadow-lg bg-blue-slate p-4">
        <h1 class="font-bold text-5xl">Objectives</h1>
        <ol>
            <li>1. Identify the Air Quality Index of different cities in the Philippines</li>
            <li>2. Analyze the relationship between city GDP and air quality/infrastructure</li>
        </ol>
    </div>

    <div class="z-20 text-right text-light-cyan flex flex-col gap-4 text-center shadow-lg bg-jet-black p-4">
        <h1 class="font-bold text-5xl">Dataset</h1>
        <p>
            This data set includes Air Quality Index (AQI) data from January 2025 to May 2025 for cities in the Philippines. 
            It includes hourly snapshots of the AQI, as well as different components, including CO, NO, NO2, O3, SO2, NH3, PM2.5, 
            and PM10 measurements per city. The data set also includes Gross Domestic Product (GDP) data for different cities in the 
            Philippines from 2024. Note that as GDP data is only released annually, there is not yet complete GDP data specific to cities 
            for 2025, so the 2024 data set was chosen for analysis as the most updated information.
        </p>
        <p>
            The data set for AQI includes 409,554 individual data points (rows), and GDP data for 34 different cities (rows) in the Philippines.
        </p>
        <p>
            Preprocessing steps for this data set included compiling the separate AQI source data sets for the different months into one sheet. 
            Additionally, the city names for the GDP set were changed to match the city names in the AQI data set. Cities found in the GDP set 
            but not in the AQI set were also removed from the GDP set.
        </p>
        <a href="https://docs.google.com/spreadsheets/d/1_RwuhXFlo51kelxt1T5t7qZmq8JKDoqIQpRssywSPFs/edit?gid=0#gid=0">Dataset Google sheet</a>
    </div>
    
    
    
</div>