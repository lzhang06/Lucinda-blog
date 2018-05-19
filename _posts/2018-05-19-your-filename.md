---
published: false
---
## A New Post

Enter text in [Markdown](http://daringfireball.net/projects/markdown/). Use the toolbar above, or click the **?** button for formatting help.
## mini-marine-traffic-api
### About
- Built with Flask Python.
- Scraped marine traffic data from www.marinetraffic.com by Beautiful Soup, a popular python package. 
- Deployed on Heroku. 
- Provided search parameters to search vessel by vessel ID/port/name/location. 

Click here to see the [demo](https://arcane-plains-26721.herokuapp.com/query?key_word=shanghai&location=CN&search_type=Vessel). 

### Instruction
- You can change the search by different parameters, which are not case sensitive. 
- Example queries: 
	1. fetch data by port name and filter data by port type
    	request: GET /query?key_word=shanghai&search_type=port 
    return: JSON(title, company, cleaned description, applied date)
	https://arcane-plains-26721.herokuapp.com/query?key_word=shanghai&search_type=port
    
    2. fetch data by vessel name and vessel location 
    request: GET query?key_word=YUEJIANGCHENG90609&location=CN
    https://arcane-plains-26721.herokuapp.com/query?key_word=YUEJIANGCHENG90609&location=CN
    
    3. fetch data by name
    https://arcane-plains-26721.herokuapp.com/query?key_word=edward

### Set Up
1. Install Python 3.x enviroment.
2. Install Python packages by running pip install -r requirements.txt .
3. Run app.py your terminal windows to start Flask Api, which is on http://localhost:5000
