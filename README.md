Cdiscount package 
===================
A Python package able to show the price of any product
of the site www.cdiscount.com

## Install

   * Download wheel file <a href="https://github.com/AnthonyH-ecv/cdiscount/raw/master/dist/cdiscount-0.0.1-py2.py3-none-any.whl">here</a>
   
   * Open your terminal and go to the directory where you downloaded the file (*cdiscount-0.0.1-py2.py3-none-any.whl*)
   
   * Now run pip command :
   
    pip install cdiscount-0.0.1-py2.py3-none-any.whl

   OR
   
    pip3 install cdiscount-0.0.1-py2.py3-none-any.whl
   
   ##### Test if you installed the package correctly
   * Open a python terminal
    
    python
   
   * Import cdiscount package and run help command
        
    >>> import cdiscount
    >>>
    >>> help(cdiscount)
  
  

    Help on package cdiscount:
    
    NAME
        cdiscount
    
    FILE
        your_path/cdiscount/__init__.py
    
    DESCRIPTION
        A Python package able to show the price of any product
        of the site www.cdiscount.com
    
    PACKAGE CONTENTS
        price_parser

    

## Usage
   
   #### Parce_price() 
   
   > parce_price(sku)
   
   param: string
  
   return: float
   
   #### Example:
   
   Test with sku : del5397184246030

    >>> from cdiscount.price_parser import parse_price
    >>>
    >>> sku = "del5397184246030"   # product identifier
    >>>
    >>> parse_price(sku)
    >>> 1776.6

# Web-app
We have a web-app using the method parse_price

    docker pull anthonyhecv/image-web-app:latest
AND
    
    docker run -p 5000:5000 anthonyhecv/image-web-app:latest

Now you can see the web app on <a href="http://localhost:5000/" target="_blank">localhost:5000</a>

Welcome to my web app !

# License
This code is licensed  <a href="https://en.wikipedia.org/wiki/GNU_General_Public_License">GPL V3</a>.
