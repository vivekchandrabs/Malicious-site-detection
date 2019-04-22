# Malicious-site-detection

Malicious websites are of great concern due it is a problem to analyze one by one and to index each URL in a black list. The project consisted to evaluate different classification models to predict malicious and benign websites, based on application layer and network characteristics. The data were obtained by using different verified sources of benign and malicious URL's, in a low interactive client honeypot to isolate network traffic.

## Install:

* Numpy
* Pandas 
* Matplotlib
* keras

You will also need to have software installed to run and execute a Jupyter Notebook.

If you do not have Python installed yet, it is highly recommended that you install the Anaconda distribution of Python, which already has the above packages and more included.

## Dataset:
This dataset is from kaggle. https://www.kaggle.com/xwolf12/malicious-and-benign-websites

## Code:

Template code is provided in the “malicious site detection.ipynb” inside the code folder. This is done using keras.

Also include the data set “dataset23.csv” while running the code.

## Run:

In a anaconda promt or in the  terminal, navigate to the code folder and run one of the following commands:

      jupyter notebook "malicious_site_detection.ipynb"
      
This will open the Jupyter Notebook software and project file in your browser.

## Attribute Information:

* URL: it is the anonimous identification of the URL analyzed in the study
* URL_LENGTH: it is the number of characters in the URL
* NUMBER_SPECIAL_CHARACTERS: it is number of special characters identified in the URL, such as, “/”, “%”, “#”, “&”, “. “, “=”
* CHARSET: it is a categorical value and its meaning is the character encoding standard (also called character set).
* SERVER: it is a categorical value and its meaning is the operative system of the server got from the packet response.
* CONTENT_LENGTH: it represents the content size of the HTTP header.
* WHOIS_COUNTRY: it is a categorical variable, its values are the countries we got from the server response (specifically, our script     used the API of Whois).
* WHOIS_STATEPRO: it is a categorical variable, its values are the states we got from the server response (specifically, our script used   the API of Whois).
* WHOIS_REGDATE: Whois provides the server registration date, so, this variable has date values with format DD/MM/YYY HH:MM
* WHOIS_UPDATED_DATE: Through the Whois we got the last update date from the server analyzed
* TCP_CONVERSATION_EXCHANGE: This variable is the number of TCP packets exchanged between the server and our honeypot client
* DIST_REMOTE_TCP_PORT: it is the number of the ports detected and different to TCP
* REMOTE_IPS: this variable has the total number of IPs connected to the honeypot
* APP_BYTES: this is the number of bytes transfered
* SOURCE_APP_PACKETS: packets sent from the honeypot to the server
* REMOTE_APP_PACKETS: packets received from the server
* APP_PACKETS: this is the total number of IP packets generated during the communication between the honeypot and the server
* DNS_QUERY_TIMES: this is the number of DNS packets generated during the communication between the honeypot and the server
* TYPE: this is a categorical variable, its values represent the type of web page analyzed, specifically, 1 is for malicious websites     and 0 is for benign websites

## Output variable (desired target):

      "TYPE" - Which tell if the site is malicious or benign. 1 for malicious and 0 for benign.

## Models trained on:
| Algorithm                         | Accuracy| Validation Accuracy | 
| --- | --- | --- |
| Neural Network               | 99.22% | 97.20% |

