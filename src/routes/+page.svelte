<script>
    import PollutionHeroPic from "$lib/assets/hero_pic_pollution.jpg";
    import AQITrends from "$lib/assets/plots/aqi_trends_2025.png";
    import PollutantTrends from "$lib/assets/plots/pollutant_trends_2025.png";
    import GDPAQICorrelation from "$lib/assets/plots/gdp_aqi_correlation.png";
    import Nutshell from "$lib/assets/plots/nutshellplot.png";
    import Hypothesis from "$lib/assets/hypothesisTest.jpeg";
</script>

<!-- Hero -->
<section class="relative min-h-[70vh] flex items-center justify-center overflow-hidden">
    <div class="absolute inset-0 z-0">
        <img class="w-full h-full object-cover" src={PollutionHeroPic} alt="pollution" />
        <div class="absolute inset-0 bg-jet-black/75"></div>
    </div>

    <div class="relative z-10 text-center px-6 max-w-4xl mx-auto flex flex-col gap-6">
        <div>
            <h1 class="font-bold text-5xl md:text-7xl text-light-cyan tracking-tight mb-4">
                michAIR jURBAN
            </h1>
            <p class="text-xl md:text-2xl text-light-blue font-light leading-relaxed">
                Exploring the correlation between a region's GDP and the Air Quality Indices (AQI) of its cities
            </p>
        </div>
        <div class="flex items-center justify-center gap-2 text-cool-steel text-sm md:text-base">
            <span class="font-medium">Jelo Fan</span>
            <span>·</span>
            <span class="font-medium">MJ Pascual</span>
            <span>·</span>
            <span class="font-medium">MJ Real</span>
        </div>
    </div>
</section>

<!-- Research Questions -->
<section id="research-questions" class="bg-surface py-20 md:py-28">
    <div class="max-w-4xl mx-auto px-6">
        <div class="mb-10">
            <h2 class="text-3xl md:text-4xl font-bold text-text-primary mb-3">Research Questions</h2>
            <div class="w-16 h-1 bg-accent rounded-full"></div>
        </div>
        <div class="flex flex-col gap-6">
            <div class="p-6 bg-surface-alt rounded-xl border border-border hover:shadow-md transition-shadow">
                <p class="text-lg md:text-xl text-text-secondary leading-relaxed">
                    How do Air Quality Indices and pollutant concentrations vary across cities in the Philippines from January to May 2025?
                </p>
            </div>
            <div class="p-6 bg-surface-alt rounded-xl border border-border hover:shadow-md transition-shadow">
                <p class="text-lg md:text-xl text-text-secondary leading-relaxed">
                    In the Philippines, what is the correlation between a city's Gross Domestic Product (GDP) and its Air Quality Index?
                </p>
            </div>
        </div>
    </div>
</section>

<!-- Hypothesis -->
<section id="hypothesis" class="bg-surface-alt py-20 md:py-28">
    <div class="max-w-4xl mx-auto px-6">
        <div class="mb-10">
            <h2 class="text-3xl md:text-4xl font-bold text-text-primary mb-3">Research Hypothesis</h2>
            <div class="w-16 h-1 bg-accent rounded-full"></div>
        </div>
        <div class="p-8 bg-surface rounded-2xl border border-border shadow-sm">
            <p class="text-lg md:text-xl text-text-secondary leading-relaxed">
                Regions with a higher GDP per capita will have more financial resources to spend on infrastructure 
                (e.g. transportation infrastructure, green spaces, and monitoring systems), 
                thus they would have a lower Air Quality Index than regions with a lower GDP per capita.
            </p>
        </div>
    </div>
</section>

<!-- Objectives -->
<section id="objectives" class="bg-surface py-20 md:py-28">
    <div class="max-w-4xl mx-auto px-6">
        <div class="mb-10">
            <h2 class="text-3xl md:text-4xl font-bold text-text-primary mb-3">Objectives</h2>
            <div class="w-16 h-1 bg-accent rounded-full"></div>
        </div>
        <div class="grid md:grid-cols-2 gap-6">
            <div class="p-6 bg-surface-alt rounded-xl border border-border hover:shadow-md transition-shadow">
                <div class="w-10 h-10 bg-accent/10 rounded-lg flex items-center justify-center mb-4">
                    <svg class="w-5 h-5 text-accent" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 20l-5.447-2.724A1 1 0 013 16.382V5.618a1 1 0 011.447-.894L9 7m0 13l6-3m-6 3V7m6 10l4.553 2.276A1 1 0 0121 18.382V7.618a1 1 0 01-.806-.984A11.962 11.962 0 0115 6.062M15 7v13m0-13l-3-1.5" />
                    </svg>
                </div>
                <p class="text-lg text-text-secondary leading-relaxed">
                    Identify the Air Quality Index of different cities in the Philippines
                </p>
            </div>
            <div class="p-6 bg-surface-alt rounded-xl border border-border hover:shadow-md transition-shadow">
                <div class="w-10 h-10 bg-accent/10 rounded-lg flex items-center justify-center mb-4">
                    <svg class="w-5 h-5 text-accent" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 12l3-3 3 3 4-4M8 21l4-4 4 4M3 4h18M4 4h16v12a1 1 0 01-1 1H5a1 1 0 01-1-1V4z" />
                    </svg>
                </div>
                <p class="text-lg text-text-secondary leading-relaxed">
                    Analyze the relationship between city GDP and air quality/infrastructure
                </p>
            </div>
        </div>
    </div>
</section>

<!-- Data -->
<section id="data" class="bg-surface-alt py-20 md:py-28">
    <div class="max-w-4xl mx-auto px-6">
        <div class="mb-10">
            <h2 class="text-3xl md:text-4xl font-bold text-text-primary mb-3">Dataset & Methodology</h2>
            <div class="w-16 h-1 bg-accent rounded-full"></div>
        </div>

        <div class="flex flex-col gap-12">
            <!-- Dataset Description -->
            <div>
                <h3 class="text-xl font-semibold text-text-primary mb-4">Dataset Description</h3>
                <div class="p-6 bg-surface rounded-xl border border-border shadow-sm">
                    <p class="text-text-secondary leading-relaxed mb-4">
                        This dataset includes Air Quality Index (AQI) data from January 2025 to May 2025 for cities in the Philippines. 
                        It includes hourly snapshots of the AQI, as well as different components, including CO, NO, NO₂, O₃, SO₂, NH₃, PM2.5, 
                        and PM10 measurements per city. The dataset also includes Gross Domestic Product (GDP) data for different cities in the 
                        Philippines from 2024.
                    </p>
                    <p class="text-text-secondary leading-relaxed">
                        Note that as GDP data is only released annually, there is not yet complete GDP data specific to cities 
                        for 2025, so the 2024 dataset was chosen for analysis as the most updated information.
                    </p>
                    <div class="mt-6 flex flex-wrap gap-4">
                        <div class="px-4 py-2 bg-accent/10 rounded-lg">
                            <span class="text-2xl font-bold text-accent">409,554</span>
                            <span class="block text-xs text-text-muted uppercase tracking-wide">AQI Data Points</span>
                        </div>
                        <div class="px-4 py-2 bg-accent/10 rounded-lg">
                            <span class="text-2xl font-bold text-accent">34</span>
                            <span class="block text-xs text-text-muted uppercase tracking-wide">Cities</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Data Collection -->
            <div>
                <h3 class="text-xl font-semibold text-text-primary mb-4">Data Collection</h3>
                <div class="p-6 bg-surface rounded-xl border border-border shadow-sm">
                    <p class="text-text-secondary leading-relaxed mb-4">
                        The AQI dataset was sourced from Kaggle, a public platform for data. The data collection process used data extracted from <a href="https://openweathermap.org/" target="_blank" rel="noopener noreferrer" class="text-accent hover:underline font-medium">OpenWeather</a>.
                    </p>
                    <p class="text-text-secondary leading-relaxed mb-4">
                        The GDP data was sourced from <a href="https://openstat.psa.gov.ph/" target="_blank" rel="noopener noreferrer" class="text-accent hover:underline font-medium">OpenSTAT</a>, an open data platform that allows PSA to share data under an open data license.
                    </p>
                    <p class="text-text-secondary leading-relaxed">
                        Preprocessing steps included compiling separate AQI source datasets for different months into one sheet. 
                        City names for the GDP set were standardized to match the AQI dataset. Cities found in the GDP set 
                        but not in the AQI set were removed.
                    </p>
                </div>
            </div>

            <!-- Links -->
            <div>
                <h3 class="text-xl font-semibold text-text-primary mb-4">Links</h3>
                <div class="flex flex-col gap-3">
                    <a 
                        href="https://docs.google.com/spreadsheets/d/1_RwuhXFlo51kelxt1T5t7qZmq8JKDoqIQpRssywSPFs/edit?gid=0#gid=0"
                        target="_blank"
                        rel="noopener noreferrer"
                        class="flex items-center gap-3 p-4 bg-surface rounded-xl border border-border hover:border-accent hover:shadow-md transition-all group"
                    >
                        <div class="w-10 h-10 bg-green-50 rounded-lg flex items-center justify-center group-hover:bg-green-100 transition-colors">
                            <svg class="w-5 h-5 text-green-600" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M14 2H6a2 2 0 00-2 2v16a2 2 0 002 2h12a2 2 0 002-2V8l-6-6z"/>
                            </svg>
                        </div>
                        <div>
                            <span class="text-text-primary font-medium group-hover:text-accent transition-colors">Compiled Dataset</span>
                            <span class="block text-sm text-text-muted">Google Sheets</span>
                        </div>
                    </a>
                    <a 
                        href="https://www.kaggle.com/datasets/bwandowando/philippine-cities-air-quality-index-data-2026"
                        target="_blank"
                        rel="noopener noreferrer"
                        class="flex items-center gap-3 p-4 bg-surface rounded-xl border border-border hover:border-accent hover:shadow-md transition-all group"
                    >
                        <div class="w-10 h-10 bg-blue-50 rounded-lg flex items-center justify-center group-hover:bg-blue-100 transition-colors">
                            <svg class="w-5 h-5 text-blue-600" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/>
                            </svg>
                        </div>
                        <div>
                            <span class="text-text-primary font-medium group-hover:text-accent transition-colors">Kaggle AQI Dataset</span>
                            <span class="block text-sm text-text-muted">Philippine Cities AQI Data</span>
                        </div>
                    </a>
                    <a 
                        href="https://openstat.psa.gov.ph/Database/Gross-Regional-Domestic-Product"
                        target="_blank"
                        rel="noopener noreferrer"
                        class="flex items-center gap-3 p-4 bg-surface rounded-xl border border-border hover:border-accent hover:shadow-md transition-all group"
                    >
                        <div class="w-10 h-10 bg-purple-50 rounded-lg flex items-center justify-center group-hover:bg-purple-100 transition-colors">
                            <svg class="w-5 h-5 text-purple-600" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zm-5 14H7v-2h7v2zm3-4H7v-2h10v2zm0-4H7V7h10v2z"/>
                            </svg>
                        </div>
                        <div>
                            <span class="text-text-primary font-medium group-hover:text-accent transition-colors">OpenSTAT GDP Data</span>
                            <span class="block text-sm text-text-muted">Gross Regional Domestic Product</span>
                        </div>
                    </a>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Results -->
<section id="results" class="bg-surface py-20 md:py-28">
    <div class="max-w-5xl mx-auto px-6">
        <div class="mb-10">
            <h2 class="text-3xl md:text-4xl font-bold text-text-primary mb-3">Exploration & Results</h2>
            <div class="w-16 h-1 bg-accent rounded-full"></div>
        </div>

        <div class="flex flex-col gap-12">
            <!-- Nutshell Plot -->
            <div>
                <h3 class="text-lg font-semibold text-text-primary mb-4">Nutshell Plot</h3>
                <div class="rounded-xl overflow-hidden border border-border shadow-md hover:shadow-xl hover:-translate-y-1 transition-all duration-300 bg-surface-alt">
                    <img src={Nutshell} alt="Nutshell plot" class="w-full h-auto" />
                </div>
            </div>

            <!-- RQ1 Plots -->
            <div>
                <h3 class="text-lg font-semibold text-text-primary mb-4">Research Question 1: AQI & Pollutant Trends</h3>
                <div class="flex flex-col gap-6">
                    <div class="rounded-xl overflow-hidden border border-border shadow-md hover:shadow-xl hover:-translate-y-1 transition-all duration-300 bg-surface-alt">
                        <img src={AQITrends} alt="AQI plot" class="w-full h-auto" />
                    </div>
                    <div class="rounded-xl overflow-hidden border border-border shadow-md hover:shadow-xl hover:-translate-y-1 transition-all duration-300 bg-surface-alt">
                        <img src={PollutantTrends} alt="Pollutant bar graph" class="w-full h-auto" />
                    </div>
                </div>
            </div>

            <!-- RQ2 Plot -->
            <div>
                <h3 class="text-lg font-semibold text-text-primary mb-4">Research Question 2: GDP-AQI Correlation</h3>
                <div class="rounded-xl overflow-hidden border border-border shadow-md hover:shadow-xl hover:-translate-y-1 transition-all duration-300 bg-surface-alt">
                    <img src={GDPAQICorrelation} alt="GDP-AQI correlation plot" class="w-full h-auto" />
                </div>
            </div>

            <!-- Hypothesis Testing -->
            <div>
                <h3 class="text-lg font-semibold text-text-primary mb-4">Hypothesis Testing</h3>
                <div class="rounded-xl overflow-hidden border border-border shadow-md hover:shadow-xl hover:-translate-y-1 transition-all duration-300 bg-surface-alt">
                    <img src={Hypothesis} alt="Hypothesis testing" class="w-full h-auto" />
                </div>
            </div>
        </div>
    </div>
</section>

<!-- About -->
<section id="about" class="bg-jet-black py-20 md:py-28">
    <div class="max-w-4xl mx-auto px-6 text-center">
        <h2 class="text-3xl md:text-4xl font-bold text-light-cyan mb-6">About Us</h2>
        <p class="text-lg md:text-xl text-cool-steel leading-relaxed max-w-2xl mx-auto">
            Jelo Fan, MJ Pascual, and MJ Real are BS Computer Science students from the University of the Philippines Diliman.
        </p>
    </div>
</section>
