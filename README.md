# rent-v-buy


When selecting a new city to move to, the question is oftem: "which one makes the most fiscal sense?"

This will help compare the pricing details on renting or buying a home, with various mortgage terms considered.

The app uses current housing data and specific inputs to determine if we should Rent or Purchase our new home in our city of choice. In order to make the best choice we will be presented with the total estimated cost of mortgage of our home purchase and our cost incurred from renting a home for our selected city.



## Technologies

This code was created with Python 3.9 and Jupyter Lab

* [pandas] - To create DataFrames and create functions to manipulate the DataFrames into various outputs

* [tkinter] - For creating the GUI input field and for displaying our outputs as graphs, dataframes, and

* [tkintermapview] - For creating a map view widget within tkinter

* [numpy] - For creating mortgage calculations

* [matplotlib] - For implementing our plots and data into our GUI

* [ChatGpt] (https://openai.com/blog/chatgpt/) - For creating amortization tables.

## Installation Guide
pip install -r Requirements.txt

## Usage

Welcome to our Rent v. Buy application!
Note there are two 'entry points' to our project
1. A tkinter gui application (gui_notebook.ipynb)
2. A notebook for data visualization (plots.ipynb)

### The Tkinter Gui
To begin this application open our File "gui_notebook.ipynb" in jupyter notebook. Run the cell containing the code, then maximize the Tkinter window that opens. This creates a pop out GUI where we are presented with our first step.

Step 1: Select the city; the dropdown menu displays 10 cities that can be selected from

        Pick a city we would like to move toX

Step 2: Click on Page 1 to continue, here the GUI displays a various data points related to the city we selected
        
Step 3: Analyze the print out
        Here are the relevant data points that were pulled from our RedFin DataFrame,
        Keep in mind this is only a list for the selected city:

        -Monthly Mortgage Payment with a 20% downpayment
        -Monthly Mortgage Payment with a 5% downpayment
        -Average yearly Home Price percentage increase 
        -Median Home Value
        -Averaage yearly Rent Price percentage increase
        -Average Monthly Rent Price


Step 4: Click on Page 2 to contiue, here the GUI displays a breakdown 

Step 5: Analyze the print out
        Here we will see a breakdown of the Average Mortgage details for the possible options.
        We've been given 4 different Mortage options:
        1) 15 year, 5% downpayment
        2) 15 year, 20% downpayment
        3) 30 year, 5% downpayment
        4) 30 year, 20% downpayment


        From these 4 Mortgage options we are being shown the details of the Mortgage
        -Home Price, Median home price pulled from our DataFrame
        -DownPayment, percentage shown from the the above Mortgage options
        -Loan Amount, which is calculated from the total loan subtract the downpayment
        -Interest Rate, is pulled from a database of current average rates for each Mortgage option
        -Loan Duration, determined by the loan term and displayed in Months
        -Monthly Taxes, pulled from our dataset and calculated for home price
        -Total Monthly Payment, calculated from Loan Amount, Loan Duration and Interest
        -Total Cost of Loan, creates a sum of all costs for the loan duration



Step 6: Click on Page 3 to continue, here the GUI displays the map of the selected city

Step 7: Here we are able to look around the general area of the selected city



Below is a Demo Video link to see how the GUI can be used      

    (https://www.youtube.com/watch?v=tWnIwwQ7OVg)


## Contributors

Austin Caras
Ben Harrington
Madhuri Krishna
Brian Peebles
Ben Wood


## License

MIT
