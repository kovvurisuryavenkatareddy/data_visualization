<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Visualization and Monitoring System</title>
    <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
    <style>
        /* CSS styles from the first code snippet */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: black;
            color: white;
            position: relative;
        }

        .header {
            background-color: #333;
            color: #fff;
            text-align: left;
            padding: 1px;
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .header h1 {
            margin: 0;
            padding: 15px;
            cursor: pointer;
        }

        .header-links {
            display: flex;
            align-items: center;
        }

        .header-links a {
            color: white;
            text-decoration: none;
            margin-right: 20px;
            padding: 5px;
            position: relative;
            font-weight: 100px;
        }

        .header-links a::after {
            content: '';
            display: block;
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background-color: white;
            transition: width 0.3s ease;
        }

        .header-links a:hover::after {
            width: 95%;
        }

        .back-to-top {
            position: fixed;
            bottom: 40px;
            right: 0px;
            background-color: #333;
            color: white;
            padding: 10px 10px;
            border: none;
            cursor: pointer;
            transform: rotate(90deg);
            transform-origin: center;
            white-space: nowrap;
        }

        .back-to-top:hover {
            background-color: #555;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: flex-start;
            margin-top: 70px; /* Adjust according to header height */
        }

        .chart-container {
            width: 500px;
            height: 350px;
            margin: 20px;
            border: 1px solid #555;
            box-sizing: border-box;
            background-color: #222;
        }
        
        table {
            border-collapse: collapse;
            width: 70%;
            border: 3px solid #fff; /* Increase border line width */
            margin: 0 auto; /* Center the table */
        }

        th, td {
            border: 2px solid #fff; /* Increase border line width */
            padding: 10px;
            text-align: left;
        }

        th {
            background-color: #2c2c2c;
        }

        tr:nth-child(even) {
            background-color: #343434;
        }

        tr:nth-child(odd) {
            background-color: #434343;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1 onclick="scrollToTop()">Sensor Data Visualization</h1>
        <div class="header-links">
            <a href="#linePlots">Line Plot</a>
            <a href="#boxPlots">Box Plot</a>
            <a href="#swarmPlots">Swarm Plot</a>
            <a href="#barGraphs">Bar Graph</a>
            <a href="#histograms">Histogram</a>
            <a href="#tables">Tables</a>
        </div>
    </div>

    <!-- Line Plot Page -->
    <div class="container" id="linePlots">
        <div class="chart-container" id="lineChartField1"></div>
        <div class="chart-container" id="lineChartField2"></div>
        <div class="chart-container" id="lineChartField3"></div>
        <div class="chart-container" id="lineChartField4"></div>
    </div>

    <!-- Box Plot Page -->
    <div class="container" id="boxPlots">
        <div class="chart-container" id="boxPlotField1"></div>
        <div class="chart-container" id="boxPlotField2"></div>
        <div class="chart-container" id="boxPlotField3"></div>
        <div class="chart-container" id="boxPlotField4"></div>
    </div>

    <!-- Swarm Plot Page -->
    <div class="container" id="swarmPlots">
        <div class="chart-container" id="swarmChartField1"></div>
        <div class="chart-container" id="swarmChartField2"></div>
        <div class="chart-container" id="swarmChartField3"></div>
        <div class="chart-container" id="swarmChartField4"></div>
    </div>

    <!-- Bar Graph Page -->
    <div class="container" id="barGraphs">
        <div class="chart-container" id="barChartField1"></div>
        <div class="chart-container" id="barChartField2"></div>
        <div class="chart-container" id="barChartField3"></div>
        <div class="chart-container" id="barChartField4"></div>
    </div>

    <!-- Histogram Page -->
    <div class="container" id="histograms">
        <div class="chart-container" id="histogramField1"></div>
        <div class="chart-container" id="histogramField2"></div>
        <div class="chart-container" id="histogramField3"></div>
        <div class="chart-container" id="histogramField4"></div>
    </div>

    <!-- Tables Page -->
    <div class="container" id="tables">
        <h2>Air & Sound Pollution Monitoring System Data</h2>
        <label for="filterDays">Filter by Days:</label>
        <select id="filterDays" onchange="handleFilterChange()">
            <option value="all">All Data</option>
            <option value="2">Last 2 Days</option>
            <option value="3">Last 3 Days</option>
            <option value="4">Last 4 Days</option>
            <option value="7">Last 7 Days</option>
            <option value="15">Last 15 Days</option>
        </select>
        <p></p>
        <table>
            <thead>
                <tr>
                    <th>Timestamp</th>
                    <th>MQ_2_Alcohol</th>
                    <th>MQ_135_CO2</th>
                    <th>Sound_Frequency</th>
                    <th>DH11_Temperature</th>
                    <th>DHT11_Humidity</th>
                </tr>
            </thead>
            <tbody id="dataBody">
                <!-- Data will be populated here -->
            </tbody>
        </table>
    </div>

    <button class="back-to-top" onclick="scrollToTop()">Back to Top</button>

    <script>
        // JavaScript code from the first code snippet
        function scrollToTop() {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        }
        // Function to fetch data from ThingSpeak and visualize it
        async function visualizeData() {
            // Your data visualization code here...
            const response = await fetch('https://api.thingspeak.com/channels/2418848/feeds.json?api_key=W3G79J5VQMRJWW92');
            const data = await response.json();
            const feeds = data.feeds;

            // Get unique field names
            const fieldNames = Object.keys(feeds[0]).filter(key => key.startsWith('field'));

            // Define field descriptions
            const fieldDescriptions = {
                'field1': 'MQ-2 (Alcohol)',
                'field2': 'MQ-135 (CO2)',
                'field3': 'Sound Sensor (Sound Frequency)',
                'field4': 'DHT11 (Temperature)'
            };

            // Create line plots for fields 1 to 4
            fieldNames.slice(0, 4).forEach((fieldName, index) => {
                createLinePlot(fieldName, feeds, index + 1, fieldDescriptions[fieldName]);
            });

            // Create box plots for fields 1 to 4
            fieldNames.slice(0, 4).forEach((fieldName, index) => {
                createBoxPlot(fieldName, feeds, index + 1, fieldDescriptions[fieldName]);
            });

            // Create swarm plots for fields 1 to 4
            fieldNames.slice(0, 4).forEach((fieldName, index) => {
                createSwarmPlot(fieldName, feeds, index + 1, fieldDescriptions[fieldName]);
            });

            // Create bar graphs for fields 1 to 4
            fieldNames.slice(0, 4).forEach((fieldName, index) => {
                createBarGraph(fieldName, feeds, index + 1, fieldDescriptions[fieldName]);
            });

            // Create histograms with density plots for fields 1 to 4
            fieldNames.slice(0, 4).forEach((fieldName, index) => {
                createHistogram(fieldName, feeds, index + 1, fieldDescriptions[fieldName]);
            });
        }

        // Function to create a line plot for a field
        function createLinePlot(fieldName, feeds, index, description) {
            const x = feeds.map(feed => new Date(feed.created_at));
            const y = feeds.map(feed => parseFloat(feed[fieldName]));

            const trace = {
                x: x,
                y: y,
                type: 'scatter',
                mode: 'lines',
                name: description
            };

            const layout = {
                title: 'Line Plot for ' + description,
                xaxis: { title: 'Date' },
                yaxis: { title: description }
            };

            const divId = 'lineChartField' + index;
            Plotly.newPlot(divId, [trace], layout);
        }

        // Function to create a box plot for a field
        function createBoxPlot(fieldName, feeds, index, description) {
            const y = feeds.map(feed => parseFloat(feed[fieldName]));

            const trace = {
                y: y,
                type: 'box',
                name: description,
                marker: {
                    color: 'rgba(128, 0, 128, 0.7)' // Purple color with opacity
                }
            };

            const layout = {
                title: 'Box Plot for ' + description,
                yaxis: { title: description }
            };

            const divId = 'boxPlotField' + index;
            Plotly.newPlot(divId, [trace], layout);
        }

        // Function to create a swarm plot for a field
        function createSwarmPlot(fieldName, feeds, index, description) {
            const x = feeds.map(feed => new Date(feed.created_at));
            const y = feeds.map(feed => parseFloat(feed[fieldName]));

            const trace = {
                x: x,
                y: y,
                mode: 'markers',
                type: 'scatter',
                name: description
            };

            const layout = {
                title: 'Swarm Plot for ' + description,
                xaxis: { title: 'Date' },
                yaxis: { title: description }
            };

            const divId = 'swarmChartField' + index;
            Plotly.newPlot(divId, [trace], layout);
        }

        // Function to create a bar graph for a field
        function createBarGraph(fieldName, feeds, index, description) {
            const x = feeds.map(feed => new Date(feed.created_at));
            const y = feeds.map(feed => parseFloat(feed[fieldName]));

            const trace = {
                x: x,
                y: y,
                type: 'bar',
                name: description
            };

            const layout = {
                title: 'Bar Graph for ' + description,
                xaxis: { title: 'Date' },
                yaxis: { title: description }
            };

            const divId = 'barChartField' + index;
            Plotly.newPlot(divId, [trace], layout);
        }

        // Function to create a histogram with density plot for a field
        function createHistogram(fieldName, feeds, index, description) {
            const x = feeds.map(feed => parseFloat(feed[fieldName]));

            const trace1 = {
                x: x,
                type: 'histogram',
                name: 'Histogram',
                opacity: 0.5,
                marker: {
                    color: 'green',
                },
            };

            const trace2 = {
                x: x,
                type: 'histogram',
                name: 'Density',
                histnorm: 'probability density',
                marker: {
                    color: 'orange',
                },
            };

            const data = [trace1, trace2];

            const layout = {
                title: 'Histogram with Density Plot for ' + description,
                xaxis: { title: description },
                yaxis: { title: 'Probability Density' }
            };

            const divId = 'histogramField' + index;
            Plotly.newPlot(divId, data, layout);
        }

        // Visualize data when the page loads
        window.onload = visualizeData;

        // Poll ThingSpeak every 30 seconds for new data and update visualization
        setInterval(visualizeData, 30000); // Adjust the interval as per your requirement
    </script>

    <script>
        // JavaScript code from the second code snippet
        async function fetchData(page, days) {
            const channelId = '2401875';
            const apiKey = ''; // If your channel is public, leave it empty
            const resultsPerPage = 1000; // Increase the number of results per page
            let apiUrl = `https://api.thingspeak.com/channels/${channelId}/feeds.json?api_key=${apiKey}&results=${resultsPerPage}&orderby=created_at`;
            if (days !== 'all') {
                let startDate = new Date();
                startDate.setDate(startDate.getDate() - days);
                const startStr = startDate.toISOString();
                apiUrl += `&start=${startStr}`;
            }
            const response = await fetch(apiUrl);
            const data = await response.json();
            return data.feeds;
        }

        // Function to update HTML table with fetched data
        async function updateData(page = 1, days = 1) {
            const feeds = await fetchData(page, days);
            const html = feeds.map(feed => {
                return `<tr>
                            <td>${feed.created_at}</td>
                            <td>${feed.field1}</td>
                            <td>${feed.field2}</td>
                            <td>${feed.field3}</td>
                            <td>${feed.field4}</td>
                            <td>${feed.field5}</td>
                        </tr>`;
            }).join('');
            document.getElementById('dataBody').innerHTML = html;
        }

        // Function to handle filter change event
        function handleFilterChange() {
            const days = document.getElementById('filterDays').value;
            updateData(1, days);
        }

        // Function to refresh data every 30 seconds
        function refreshData() {
            updateData(); // Initial call to fetch data
            setInterval(updateData, 3000000); // Refresh every 30 seconds
        }

        // Fetch and refresh data when the page loads
        window.onload = function() {
            document.getElementById('filterDays').value = '15'; // Set default filter to last 15 days
            updateData(1, '15'); // Fetch data for the last 15 days by default
            refreshData(); // Start refreshing data
        };
    </script>
</body>
</html>
