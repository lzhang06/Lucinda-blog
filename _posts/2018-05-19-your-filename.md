---
published: true
---
## mini-marine-traffic-api
### About
- Built with Flask Python.
- Scraped marine traffic data from www.marinetraffic.com by Beautiful Soup, a popular python package. 
- Deployed on Heroku. 
- Provided search parameters to search vessel by vessel ID/port/name/location(here using [mmsi](https://en.wikipedia.org/wiki/Maritime_Mobile_Service_Identity) as vessel ID). 

Click here to see the [demo](https://arcane-plains-26721.herokuapp.com/query?key_word=YUEJIANGCHENG90609). 

### Instruction
- You can change the search by different parameters, which are not case sensitive. 
- Example queries: 
	1. [fetch data by port name and filter data by port type](https://arcane-plains-26721.herokuapp.com/query?key_word=shanghai&search_type=port)
    
	request: GET /query?key_word=shanghai&search_type=port
    
    [2. fetch data by vessel name and vessel location](https://arcane-plains-26721.herokuapp.com/query?key_word=YUEJIANGCHENG90609&location=CN)
    
    request: GET query?key_word=YUEJIANGCHENG90609&location=CN
    
    [3. fetch data by name](https://arcane-plains-26721.herokuapp.com/query?key_word=edward)
    request: GET /query?key_word=edward
    
    4. [fetch data by Vessel ID](https://arcane-plains-26721.herokuapp.com/query?key_word=218776000)
    
    request: GET/query?key_word=218776000
   

### Set Up
1. Install Python 3.x enviroment.
2. Install Python packages by running pip install -r requirements.txt .
3. Run app.py your terminal windows to start Flask Api, which is on http://localhost:5000


