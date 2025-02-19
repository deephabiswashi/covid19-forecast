
<h1 style="color: #2F4F4F; text-align:center;">
  <b>Covid-19 Forecasting and Prediction Project</b>
</h1>

<p style="text-align:center;">
  <em>Predict and analyze COVID-19 casualties using ML</em>
</p>

<hr style="border: 1px solid #ccc; margin: 20px 0;" />

<h2 style="color:#4169E1;">1. Overview</h2>

<p>
  This repository demonstrates a <strong>machine learning project</strong> for predicting COVID-19 trends. 
  It merges multiple datasets (epidemiology, geography, hospitalizations, government response, and vaccinations) 
  to provide a comprehensive view of the pandemic. Key features include:
</p>

<ul>
  <li><strong>Data Merging & Preprocessing:</strong> Combining five CSV files into a unified dataset.</li>
  <li><strong>Visualizations:</strong>
    <ul>
      <li>Interactive map of COVID-19 spread using cumulative confirmed cases.</li>
      <li>Time-series plots for global daily new confirmed cases and deaths.</li>
    </ul>
  </li>
  <li><strong>Forecasting:</strong> Using 
    <a href="https://facebook.github.io/prophet/" target="_blank">Facebook Prophet</a> 
    to predict future daily new confirmed cases.
  </li>
</ul>

<hr style="border: 1px solid #ccc; margin: 20px 0;" />

<h2 style="color:#4169E1;">2. Project Structure</h2>

<pre>
Covid-19 Forecast Model/
├── Datasets/
│   ├── epidemiology.csv
│   ├── geography.csv
│   ├── hospitalizations.csv
│   ├── oxford-government-response.csv
│   └── vaccinations.csv
│
├── notebooks/
│   └── covidpredict.ipynb   # Main notebook with code
│
├── README.md                # Project description
├── requirements.txt         # Python dependencies (if any)
└── .gitignore               # Git ignore rules
</pre>

<hr style="border: 1px solid #ccc; margin: 20px 0;" />

<h2 style="color:#4169E1;">3. Datasets</h2>

<ol>
  <li><strong>epidemiology.csv</strong>  
    <em>Columns:</em> date, location_key, new_confirmed, new_deceased, new_recovered, new_tested, cumulative_confirmed, cumulative_deceased, cumulative_recovered, cumulative_tested
  </li>
  <li><strong>geography.csv</strong>  
    <em>Columns:</em> location_key, openstreetmap_id, latitude, longitude, elevation_m, area_sq_km, area_rural_sq_km, area_urban_sq_km
  </li>
  <li><strong>hospitalizations.csv</strong>  
    <em>Columns:</em> date, location_key, new_hospitalized_patients, cumulative_hospitalized_patients, current_hospitalized_patients, new_intensive_care_patients, cumulative_intensive_care_patients, current_intensive_care_patients, new_ventilator_patients, cumulative_ventilator_patients, current_ventilator_patients
  </li>
  <li><strong>oxford-government-response.csv</strong>  
    <em>Columns:</em> date, location_key, school_closing, workplace_closing, cancel_public_events, restrictions_on_gatherings, public_transport_closing, stay_at_home_requirements, restrictions_on_internal_movement, international_travel_controls, income_support, debt_relief, fiscal_measures, international_support, public_information_campaigns, testing_policy, contact_tracing, emergency_investment_in_healthcare, investment_in_vaccines, facial_coverings, vaccination_policy, stringency_index
  </li>
  <li><strong>vaccinations.csv</strong>  
    <em>Columns:</em> date, location_key, new_persons_vaccinated, cumulative_persons_vaccinated, etc.
  </li>
</ol>

<hr style="border: 1px solid #ccc; margin: 20px 0;" />

<h2 style="color:#4169E1;">4. Installation</h2>

<ol>
  <li>
    <strong>Clone this repository:</strong>
    <pre><code>git clone https://github.com/deephabiswashi/covid19-forecast
cd "Covid-19 Forecast Model"
</code></pre>
  </li>
  <li>
    <strong>Create and activate a virtual environment (optional):</strong>
    <pre><code>python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
</code></pre>
  </li>
  <li>
    <strong>Install dependencies:</strong>
    <pre><code>pip install -r requirements.txt
</code></pre>
  </li>
</ol>

<hr style="border: 1px solid #ccc; margin: 20px 0;" />

<h2 style="color:#4169E1;">5. Usage</h2>

<ol>
  <li><strong>Place the CSV files</strong> in the <code>Datasets/</code> folder.</li>
  <li><strong>Open the Jupyter notebook</strong> (<code>covidpredict.ipynb</code>) in VS Code or Jupyter.</li>
  <li><strong>Run all cells</strong> to:
    <ul>
      <li>Merge and preprocess the datasets</li>
      <li>Generate visualizations (interactive map, time-series plots)</li>
      <li>Use Prophet to forecast future daily new confirmed cases</li>
    </ul>
  </li>
</ol>

<hr style="border: 1px solid #ccc; margin: 20px 0;" />

<h2 style="color:#4169E1;">6. Contributing</h2>

<p>
  Contributions are welcome! Feel free to open issues or submit pull requests.
</p>

<hr style="border: 1px solid #ccc; margin: 20px 0;" />

<h2 style="color:#4169E1;">7. License</h2>

<p>
  This project is licensed under the <strong>MIT License</strong>.
  See the <code>LICENSE</code> file for details.
</p>

<hr style="border: 1px solid #ccc; margin: 20px 0;" />

<p style="text-align:center;">
  <em>Made with ❤️ by &lt;Deep Habiswashi&gt;</em>
</p>
