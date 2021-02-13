## About
Sniffipy is a simple wrapper for the [sniffip.com](https://sniffip.com) website, which gives you the ip of a person entering a specialy crafted link.

## dependencies
- [geckodriver-autoinstaller](https://pypi.org/project/geckodriver-autoinstaller/)
- [selenium](https://pypi.org/project/selenium/)
- [firefox](https://www.mozilla.org/firefox/new/)

## Installation

`pip install sniffipy`</br></br>

or</br></br>

`git clone https://github.com/SmellyN3rd/sniffipy`</br></br>
`pip install -r sniffipy/requirements.txt`</br></br>

## Usage

`python`</br></br>
`import sniffipy`</br></br>
`sniffipy.create_sniffer(url)`</br></br> 
where the url is the url you want the person clicking it to be redirrected to, for example: https://www.youtube.com/watch?v=dQw4w9WgXcQe  </br></br>
this will return a dict with two values: the sniffer id which you will need later and the short url to send to someone who's ip you want to know </br></br>
`sniffipy.sniffer_data(id)`</br></br> 
You need to replace the id with the id that was generated earlier. This function will return a dict with three lists: a list of ips, their user agents and the time they clicked the link
