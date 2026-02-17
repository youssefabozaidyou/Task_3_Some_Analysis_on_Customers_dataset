<!DOCTYPE html>

<html lang="en">

<head>

&nbsp;   <meta charset="UTF-8">

&nbsp;   <title>Customer Data Analysis - Task</title>

</head>

<body style="font-family: Arial, sans-serif; line-height: 1.7; padding: 20px;">



<h1>📊 Customer Data Analysis - Task</h1>



<p>

This project is a dedicated <strong>Data Analysis \& Data Cleaning Task</strong> focused on exploring, cleaning, 

and extracting insights from a <strong>Customer Behavior Dataset</strong>.  

The goal was to demonstrate proficiency in Python data handling, statistical exploration, 

feature engineering, and business-oriented data cleaning techniques.

</p>



<hr>



<h2>📝 Task Objectives</h2>

<p>The primary objective of this task was to perform an in-depth analysis of customer data to understand:</p>

<ul>

&nbsp;   <li>Data structure, integrity, and statistical distribution.</li>

&nbsp;   <li>Income ranges, demographic patterns, and spending behavior.</li>

&nbsp;   <li>Detection and removal of invalid entries and statistical outliers.</li>

&nbsp;   <li><strong>Behavioral Segmentation</strong>: Identifying high and low spenders based on spending scores.</li>

</ul>



<hr>



<h2>📂 Project Structure</h2>

<p>The repository is organized to ensure clarity and reproducibility:</p>

<ul>

&nbsp;   <li><strong>data/</strong>: Contains both raw and cleaned customer datasets.</li>

&nbsp;   <li><strong>notebooks/data\_cleaning.ipynb</strong>: The core Jupyter Notebook containing the full analytical workflow.</li>

&nbsp;   <li><strong>scripts/data\_cleaning.py</strong>: A Python script version of the project pipeline.</li>

&nbsp;   <li><strong>visuals/</strong>: Stores the generated boxplot visualizations for income outliers.</li>

&nbsp;   <li><strong>README.md</strong>: Documentation summarizing the task, methodology, and insights.</li>

</ul>



<hr>



<h2>🛠️ Analysis Steps (What I did)</h2>

<p>In this notebook, I followed a structured, step-by-step data analysis process:</p>



<h3>1. <strong>Data Loading \& Setup</strong></h3>

<ul>

&nbsp;   <li>Loaded the dataset using <code>Pandas</code>.</li>

&nbsp;   <li>Displayed initial samples using <code>.head()</code>, <code>.tail()</code>, and <code>.sample()</code>.</li>

&nbsp;   <li>Examined structure and datatypes using <code>.info()</code> and <code>.describe()</code>.</li>

</ul>



<h3>2. <strong>Data Cleaning \& Validation</strong></h3>

<ul>

&nbsp;   <li>Removed invalid age entries (customers aged <strong>5 years or younger</strong>).</li>

&nbsp;   <li>Filled missing values in the <strong>Profession</strong> column with <em>"Unknown"</em>.</li>

&nbsp;   <li>Detected missing values using <code>.isna().sum()</code>.</li>

&nbsp;   <li>Identified and removed duplicate rows using <code>.duplicated().sum()</code>.</li>

</ul>



<h3>3. <strong>Income Filtering \& Outlier Removal</strong></h3>

<ul>

&nbsp;   <li>Removed unrealistic <code>Annual Income ($)</code> values (≤ 1000).</li>

&nbsp;   <li>Used a <strong>Seaborn boxplot</strong> to visualize income distribution.</li>

&nbsp;   <li>Applied the <strong>IQR Method</strong> (Q1, Q3, IQR) to remove statistical outliers.</li>

</ul>



<h3>4. <strong>Feature Engineering</strong></h3>

<p>Created new business-focused features:</p>

<ul>

&nbsp;   <li><strong>High\_Spender</strong> → Spending Score \&gt; 50</li>

&nbsp;   <li><strong>Low\_Spender</strong> → Spending Score \&lt; 50</li>

&nbsp;   <li><strong>Spending\_Ratio</strong> → (Spending Score) / (Annual Income)</li>

</ul>



<h3>5. <strong>Datatype Optimization</strong></h3>

<ul>

&nbsp;   <li>Converted the <strong>Gender</strong> column to a <code>category</code> datatype for optimized performance.</li>

</ul>



<h3>6. <strong>Data Export</strong></h3>

<ul>

&nbsp;   <li>Exported the cleaned dataset into the <strong>data/processed/</strong> folder.</li>

</ul>



<hr>



<h2>🚀 Technologies Used</h2>

<ul>

&nbsp;   <li><strong>Python 3.x</strong></li>

&nbsp;   <li><strong>Pandas</strong>: Data manipulation and cleaning</li>

&nbsp;   <li><strong>NumPy</strong>: Statistical calculations</li>

&nbsp;   <li><strong>Matplotlib / Seaborn</strong>: Visualization \& outlier detection</li>

</ul>



<hr>



<h2>⚙️ How to Run</h2>

<ol>

&nbsp;   <li>Clone the repository:

&nbsp;       <pre><code>git clone \&lt;repository-link\&gt;</code></pre>

&nbsp;   </li>

&nbsp;   <li>Install required libraries:

&nbsp;       <pre><code>pip install pandas numpy matplotlib seaborn</code></pre>

&nbsp;   </li>

</ol>



</body>

</html>



