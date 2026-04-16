# Data visualisation week 07 
# Student Instructions:
# _
# Import Plotly Express and load the dataset.
# Filter to show only the year 2007.
# Create a scatter plot:
# X = gdpPercap
# Y = lifeExp
# Color = continent
# Size = pop
# Add a title: “GDP vs Life Expectancy (2007)”
# Hover over points to see details.
# Hints
# _
# import plotly.express as px
# _
# df = px.data.gapminder()
# _
# # TIP: To show one year only
# _
# # df_year = df[df["year"] == 2007]
# _
# # TIP: Use px.scatter(...)
# _
# # log_x=True makes GDP scale easier to read
# _
# Expected Outcome:
# An interactive bubble chart where hovering shows country names and stats.
# _
# Task 2 : Add Controls with ipywidgets (20 min)
# _
# Student Instructions:
# _
# Add an integer slider for selecting a year.
# Add a dropdown for selecting a continent (or “All”).
# Link both controls to the chart-update function.
# When a control changes, the plot updates automatically.
# Hints
# _
# import ipywidgets as widgets
# _
# from IPython.display import display
# _
 
# _
# # TIP: widgets.IntSlider(...)  -> for year
# _
# # TIP: widgets.Dropdown(...)   -> for continent
# _
# # TIP: Use df[(df["year"]==year) & (df["continent"]==continent)]
# _
# #      or skip the continent filter if "All" is chosen
# _
# Add a title that automatically updates:
# _
# title=f"GDP vs Life Expectancy ({year}, {continent})"
# _
#  Task 3: Replicate in Tableau (20 min)
# _
# Steps:
# _
# Connect Tableau to the gapminder.csv file (or use World Indicators).
# Drag GDP per Capita → Columns, Life Expectancy → Rows.
# Drag Country → Detail, Population → Size, Continent → Color.
# Drag Year → Pages shelf → Tableau adds a slider (animation).
# Add hover tooltips (right-click → Tooltip → Edit).
# Optionally add Continent to Filters → Show Filter (dropdown).
# Reflection Questions (5 min)
# _
# Which tool was faster to build with?
# Which gave more control?
# How could you make the chart more user-friendly?