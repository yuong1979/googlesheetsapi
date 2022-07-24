# Sample google sheets project with docker

## Based on tutorial on  https://www.youtube.com/watch?v=4ssigWmExak&t=179s

**Clone project**

`git clone https://github.com/yuong1979/googlesheetsapi.git`

**Change directory into the project**

`cd googlesheetsapi`

**Start a the virtual environment**

`python3 -m venv venv`

**Run the virtual environment**

`source venv/bin/activate`

**Install the requirements**

`pip install -r requirements.txt`

Create a service account, create a new google sheets api, create a keys.json and leave it in the main folder

### Deploy on local without docker

**Run the server only local**

`python3 read.py`

Check the google sheets for changes


### Deploy with docker on local

Comment out the production code on Dockerfile

**Build the image**

`docker build -t googleapipython .`

**Deploy the image**

`docker run googleapipython`
