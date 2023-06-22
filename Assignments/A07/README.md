## Weather Data Scraper
This project is a Python-based weather data scraper that fetches historical weather data from Weather Underground based on the provided parameters such as a month, day, year, airport code, and frequency. The data is presented to the user in a simple and easy-to-understand table format.
## Requirements
-	Python 3.x
-	Selenium (pip install selenium)
-	BeautifulSoup (pip install beautifulsoup4)
-	PySimpleGUI (pip install PySimpleGUI)
-	Chrome WebDriver is installed and available in PATH or the directory where the scripts are being run
## Files
The project consists of two Python files:
-	gui.py: This file provides a graphical user interface to the user for input parameters and displays the fetched weather data.
-	get_weather.py: This file uses Selenium and BeautifulSoup to scrape historical weather data from Weather Underground.
## Implementation Details
-	The application uses PySimpleGUI for the GUI components. The interface collects the user’s desired parameters, such as date, airport code, and data frequency.
-	The GUI script reads airport codes from a CSV file (airport-codes.csv).
-	Selenium WebDriver is used in the get_weather.py script to render the dynamic web page from Weather Underground.
-	BeautifulSoup is used to parse the page HTML and extract the necessary data. The data is then returned to gui.py, which displays it in a tabular format using PySimpleGUI's Table element.
## How to Run
1.	Install all the necessary requirements mentioned above.
2.	Run the gui.py script.
3.	Fill in the desired parameters in the GUI and click ‘Submit’.
4.	The application will fetch the data and display it in a table.
## Example Queries
Fetching weekly weather data for Dec 31, 2020, for airport code KCHO:
-	Month: 12
-	Day: 31
-	Year: 2020
-	Airport Code: KCHO
-	Frequency: weekly

  ![image](https://github.com/swarajtwok/4883-SoftwareTools-Chirumamilla/assets/67910599/5307b17c-c65f-4213-bc6a-9464b9033097)
  ![image](https://github.com/swarajtwok/4883-SoftwareTools-Chirumamilla/assets/67910599/a4649a9e-fc10-4295-a949-c206c1f5bc33)



Fetching daily weather data for Dec 31 2020 for airport code KTXK:
-	Month: 12
-	Day: 31 
-	Year: 2020
-	Airport Code: KTXK
-	Frequency: monthly
 
   ![image](https://github.com/swarajtwok/4883-SoftwareTools-Chirumamilla/assets/67910599/e2dd50a3-dd51-417d-9720-dbfd27831f67)
   ![image](https://github.com/swarajtwok/4883-SoftwareTools-Chirumamilla/assets/67910599/ef6aa411-6f48-49f8-a5bc-bfca77962220)



 

Fetching monthly weather data for the week of December 31, 2023, for airport code KTXK:

-	Month: 12
-	Day: 31 (it can be any day in the month when selecting monthly frequency)
-	Year: 2020
-	Airport Code: KTXK
-	Frequency: weekly

         
         ![image](https://github.com/swarajtwok/4883-SoftwareTools-Chirumamilla/assets/67910599/abd22477-77dc-40f2-8ee6-ab13c97e8d08)
         ![image](https://github.com/swarajtwok/4883-SoftwareTools-Chirumamilla/assets/67910599/4e9c9bcb-d4af-4e0e-82fe-f59fb8c427ae)



 

Known Limitations
-	The program assumes the existence of airport-codes.csv and chromedriver.exe in the working directory.
-	It only fetches weather data from Weather Underground, so it is limited to the data available on that website.
-	Error handling for edge cases may not be comprehensive, so it’s possible that the program could encounter errors with unusual input or unexpected website changes.
Future Improvements
-	Adding support for more data sources for enhanced reliability and availability of data.
-	Improving error handling and input validation to make the program more robust and user-friendly.
-	Extending the interface to support more input parameters, such as specific hours of the day, or specific weather conditions.