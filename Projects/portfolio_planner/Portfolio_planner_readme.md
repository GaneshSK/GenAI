# **Portfolio Planner Tool**

## **Overview**

The Portfolio Planner Tool is a Python-based application designed to help users create a personalized investment strategy. Leveraging the power of OpenAI's GPT-4, the tool provides detailed recommendations on asset allocation based on the user's financial goals, risk tolerance, and market data. It dynamically adjusts investment strategies to help users achieve their financial objectives efficiently.

## **Features**

* **User Input Collection**: Collects essential financial information directly from the user, such as income, expenses, goals, and risk profile.  
* **Market Data Integration**: Utilizes real-world market data to provide accurate and relevant investment recommendations.  
* **Dynamic Portfolio Allocation**: Recommends an optimal portfolio allocation based on the user's risk level and financial goals.  
* **SIP Calculation**: Calculates the required Systematic Investment Plan (SIP) based on expected returns for each goal.  
* **Real-Time Adjustments**: Adjusts investment strategies dynamically based on changes in market conditions and user feedback.  
* **Comprehensive Reports**: Generates detailed reports summarizing the user's financial profile, portfolio recommendations, and required actions.

## **Project Structure**

Copy code  
`.`  
`├── portfolio_planner_tool.ipynb   # Jupyter notebook containing the main code`  
`├── market_data.csv                # CSV file containing market data used for portfolio recommendations`  
`├── README.md                      # Project documentation`  
`└── requirements.txt               # List of Python dependencies`

## **Getting Started**

### **Prerequisites**

To run this project, you'll need:

* Python 3.7 or later  
* A Google Colab account (recommended for running the notebook)  
* An OpenAI API key

### **Installation**

**Clone the Repository**:  
bash  
Copy code  
`git clone https://github.com/yourusername/portfolio-planner-tool.git`  
`cd portfolio-planner-tool`

1. **Set Up Google Colab**:  
   * Upload the `portfolio_planner_tool.ipynb` notebook to your Google Drive.  
   * Ensure the `market_data.csv` file is also uploaded to the correct folder in your Google Drive.  
2. **Install Dependencies**:  
   * Open the notebook in Google Colab.  
   * Run the cell that installs the necessary Python packages listed in `requirements.txt`.  
3. **Set Up OpenAI API**:  
   * Obtain an API key from OpenAI.  
   * Save the API key in a text file named `openai_api_key.txt` and upload it to the same folder in your Google Drive.

### **Running the Project**

1. **Mount Google Drive**:  
   * The notebook will guide you through mounting your Google Drive to access the necessary files.  
2. **Load Market Data**:  
   * The notebook will load market data from the `market_data.csv` file.  
3. **Input User Data**:  
   * The notebook will prompt you to enter your financial details, including income, expenses, and financial goals.  
4. **Generate Portfolio Recommendations**:  
   * The tool will use your inputs, along with market data, to generate personalized portfolio recommendations and calculate the required SIP.  
5. **Review the Final Report**:  
   * The notebook will output a comprehensive report summarizing your financial profile and recommended investment strategy.

### **Example Usage**

Here's a brief overview of how to use the tool:

python  
Copy code  
`# Load market data`  
`market_data = load_market_data()`

`# Input user data`  
`user_data = get_user_inputs()`

`# Evaluate portfolio allocation`  
`portfolio_results = evaluate_portfolio_allocation(user_data, market_data)`

`# Recommend portfolio allocation based on risk level`  
`risk_level = assess_risk_profile_with_llm(user_data['risk_profile'])`  
`allocation_recommendation = recommend_portfolio_allocation_with_llm(risk_level, market_data)`

`# Generate and print the final report`  
`final_report = generate_final_report(user_data, portfolio_results, allocation_recommendation)`  
`print(final_report)`

### **Sample Market Data Format**

The `market_data.csv` file should have the following structure:

plaintext  
Copy code  
`Name,Type,6 months returns,1 yr XIRR,2 yr XIRR,3 yr XIRR,5 yr XIRR,7 yr XIRR,10 yr XIRR,15 yr XIRR`  
`NIFTY 50,Index,10.00%,12.10%,15.30%,14.00%,12.80%,12.50%,11.40%,10.50%`  
`NIFTY Next 50 (NIFTY JR),Index,8.70%,9.30%,14.00%,13.70%,11.50%,12.00%,10.80%,9.80%`  
`...`

### **Dependencies**

The following Python libraries are required:

* `openai`  
* `pandas`  
* `numpy`  
* `google-colab` (for running in Google Colab)

All dependencies are listed in the `requirements.txt` file.

### **License**

This project is licensed under the MIT License. See the LICENSE file for more details.

### **Contact**

If you have any questions or need further assistance, please reach out to:

* **Ganesh S K**  
* **s.k.ganesh91@gmail.com**  
* **Your GitHub Profile**: https://github.com/GaneshSK

### **Acknowledgments**

Special thanks to OpenAI for providing the GPT-4 API, and to the open-source community for the tools and libraries that made this project possible.

