<p align="center">
  <a href="https://github.com/XpressAI/xircuits/tree/master/xai_components#xircuits-component-library-list">Component Libraries</a> •
  <a href="https://github.com/XpressAI/xircuits/tree/master/project-templates#xircuits-project-templates-list">Project Templates</a>
  <br>
  <a href="https://xircuits.io/">Docs</a> •
  <a href="https://xircuits.io/docs/Installation">Install</a> •
  <a href="https://xircuits.io/docs/category/tutorials">Tutorials</a> •
  <a href="https://xircuits.io/docs/category/developer-guide">Developer Guides</a> •
  <a href="https://github.com/XpressAI/xircuits/blob/master/CONTRIBUTING.md">Contribute</a> •
  <a href="https://www.xpress.ai/blog/">Blog</a> •
  <a href="https://discord.com/invite/vgEg2ZtxCw">Discord</a>
</p>





<p align="center"><i>Xircuits Component Library for Apache Spark! Process and analyze big data with powerful, scalable components.</i></p>

---
## Xircuits Component Library for Spark

The Spark component library makes it easy to use Apache Spark within Xircuits workflows. You can process, analyze, and visualize large datasets efficiently.

## Table of Contents

- [Preview](#preview)
- [Prerequisites](#prerequisites)
- [Main Xircuits Components](#main-xircuits-components)
- [Try the Examples](#try-the-examples)
- [Installation](#installation)

## Preview

### SparkLinePlot Example

![SparkLinePlot](https://github.com/user-attachments/assets/5900c7e9-05d3-44e2-9332-ffeb5c885350)

### SparkLinePlot Result

<img src="https://github.com/user-attachments/assets/1294489b-db91-4371-9d18-f0ce8778bb20" alt="SparkLinePlot"/>

### SparkLogisticRegressionSample Example

![SparkLogisticRegressionSample](https://github.com/user-attachments/assets/8570b3f5-50e7-4b6d-bd2c-f70c05194ad4)

### SparkLogisticRegressionSample Result

<img src="https://github.com/user-attachments/assets/9bba50c3-bbf4-492a-b07f-67ea3075b0f3" alt="SparkLogisticRegressionSample_result"/>

### SparkSQLPlotBar Example 

![SparkSQLPlotBar](https://github.com/user-attachments/assets/81279a92-ef57-4581-80cb-ed184e994e53)


### SparkSQLPlotBar Result

<img src="https://github.com/user-attachments/assets/7bbc5723-d982-4f2e-928f-34b37030763c" alt="SparkSQLPlotBar_result"/>

## Main Xircuits Components

### xSparkSession
Initializes a Spark session to enable distributed data processing.

<img src="https://github.com/user-attachments/assets/04fa8a54-5972-44c3-a0ed-61bbf2779bae" alt="xSparkSession" width="200" height="125" />

### SparkReadFile Component:
Reads data from files in formats like csv, json, parquet, or orc into a Spark DataFrame.

<img src="https://github.com/user-attachments/assets/4adea79f-026f-42d6-868f-c2f8ec6a0743" alt="SparkReadFile" width="200" height="85" />

### SparkWriteFile Component:
Saves Spark DataFrames to files in formats such as csv, parquet, or orc.

### SparkReadCSV Component:
Reads CSV files into a Spark DataFrame with options for custom delimiters and headers.

### SparkSQL Component:
Executes SQL queries on a Spark DataFrame, returning query results as a new DataFrame.

### SparkVisualize Component:
Creates bar, scatter, or line plots from Spark DataFrames and saves them as images.

### SparkSplitDataFrame Component:
Splits a Spark DataFrame into training and testing sets based on a specified ratio.

### SparkLogisticRegression Component:
Trains a logistic regression model using a Spark DataFrame.

### SparkPredict Component:
Uses a trained Spark model to make predictions on a test DataFrame.

## Try the Examples

We have provided an example workflow to help you get started with the Spark component library. Give it a try and see how you can create custom Spark components for your applications.

### SparkLinePlot 

This example demonstrates creating a line plot from a CSV file using Spark. It reads the dataset, processes it into a Spark DataFrame, and visualizes the relationship between the Year and Wind columns as a line plot saved as Lineplot.png.

### SparkLogisticRegressionSample 

This example uses the SparkLoadLIBSVM component to load data, splits it for training and testing with SparkSplitDataFrame, and trains a multinomial logistic regression model to make predictions.

### SparkSQLPlotBar

This example loads penguin data from a CSV file, queries species information using Spark SQL, and generates a bar plot visualizing species distribution, saving it as 'pinguin_distribution.png'.

## Installation
To use this component library, ensure that you have an existing [Xircuits setup](https://xircuits.io/docs/main/Installation). You can then install the Spark library using the [component library interface](https://xircuits.io/docs/component-library/installation#installation-using-the-xircuits-library-interface), or through the CLI using:

```
xircuits install spark
```
You can also do it manually by cloning and installing it:
```
# base Xircuits directory  
git clone https://github.com/XpressAI/xai-spark xai_components/xai_spark  
pip install -r xai_components/xai_spark/requirements.txt  
```