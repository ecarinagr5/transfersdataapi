<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->




<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">TRANSFER DATA API</h3>

  <p align="center">
      API DOCUMENTATION!
    <br />
  </p>
</div>







<!-- ABOUT THE PROJECT -->
## About The Project
TRANSFER DATA API is an interface to exchange information securely over aplications

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### POST New Lead
Post information in API
URL: https://transfersdata.com/api/leads/
TYPE: POST
FORMAT: JSON

Below Example about structure:
```
{
    "LEAD_ID": "01",
    "LD_NAME": "Lead Test 1",
    "LD_LAST_NAME": "Lead Last Name",
    "LD_EMAIL": "email@gmail.com",
    "LD_PHONE_NUM": "5555555555",
    "LD_ZIPCODE": "58270",
    "VENDOR_ID": 40,
    "MODEL_ID": 7,
    "CAMPAIGN": "Name of Campaign",
    "LD_REG_DATE": "",
    "UTM_SOURCE": "",
    "UTM_MEDIUM": "",
    "UTM_CAMPAIGN": "",
    "ID_FACEBOOK": null,
    "TD_DATE":"2023-02-15T11:11:00",
    "TD_HOUR":"",
    "QTN_PRICE": 0,
    "QTN_TERM_OF_FINANCE": 0,
    "QTN_DOWN_PAYMENT": 0,
    "QTN_AMOUNT": 0,
    "QTN_FINANCING_PLAN": "0",
    "QTN_INSURANCE_COMPANY": "0"
}
```

FIELDS REQUIRED:
```
    "LD_NAME": "Lead Test 1"
    "LD_EMAIL": "email@gmail.com"
    "LD_PHONE_NUM": "5555555555"
```

TYPE OF FIELDS:

    "LEAD_ID": STRING | NULL --> Number of lead
    "LD_NAME": STRING  --> Name of lead
    "LD_LAST_NAME": STRING | NULL  --> last name of lead
    "LD_EMAIL": STRING  --> Email of lead
    "LD_PHONE_NUM": STRING  --> Phone number of lead
    "LD_ZIPCODE": STRING  | NULL --> Zipcode of lead
    "VENDOR_ID": NUMBER  | 0 --> Vendor Id
    "MODEL_ID": NUMBER  | 0 --> Model Id
    "CAMPAIGN":  STRING  | NULL --> campaign
    "LD_REG_DATE":  STRING  | NULL --> date
    "UTM_SOURCE":  STRING  | NULL --> UTM
    "UTM_MEDIUM":  STRING  | NULL --> UTM
    "UTM_CAMPAIGN":  STRING  | NULL --> UTM
    "ID_FACEBOOK":  STRING  | NULL --> ID facebook 
    "TD_DATE": STRING  | NULL --> Date
    "TD_HOUR":STRING  | NULL --> Hour
    "QTN_PRICE": NUMBER  | 0 --> Price
    "QTN_TERM_OF_FINANCE": NUMBER  | 0 
    "QTN_DOWN_PAYMENT": NUMBER  | 0 
    "QTN_AMOUNT": NUMBER  | 0 
    "QTN_FINANCING_PLAN": STRING  | NULL
    "QTN_INSURANCE_COMPANY": STRING  | NULL 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

SUCCESS RESPONSE

CODE STATUS 200
```
  res.json({
    msg: "Value has been inserted"
  });
```

FAIL RESPONSE

CODE STATUS 400
```
  res.json({
    msg: "error: "This value is required, pls try again.""
  });
```


### GET Health Check API

Get Health Validation API
URL: https://transfersdata.com/api/
TYPE: GET


