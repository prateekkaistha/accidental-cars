# accidental-cars
Requirements:-
    1. flask
    2. npm     
    3. node.js    
    4. ws module for JS (websockets).

Installation process for linux based distros
    To install pip       
        sudo apt-get install python3-pip
    1.pip install Flask       
    2.sudo apt-get install npm 
    3.sudo npm install -g n
    4.sudo n latest    
      Go to the server directory and execute  
    5.npm install ws.
        
Running the program        
Since we did not have the device to fetch the exact gps coordinates so we used static coordinates sent by the client to the server as soon as the web application is loaded. The server on receiving the coordinates broadcasts to the nearby devices.
    1.To run the application on LAN first go to the index.html and edit line 32, replace "ipaddress required" with your own PC's local IP and remove the quotes.
    2.Open a terminal and go to the server directry and execute "node index.js".
    3.Open another terminal on the proj folder execute "export FLASK_APP=application.py".    
    4.Then on the same terminal execute "flask run --host=0.0.0.0 --port=5000".    
    5.Open the browser and go to "ipaddress:5000" replace ipaddress with IPaddress of the server PC.
