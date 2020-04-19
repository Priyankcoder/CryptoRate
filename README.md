# CryptoRate
It is a website which show dynamic pricing with the help of Coinbase API.

#### Overview

This web application creates an online catalog for a small local library, where users can browse available books and manage their accounts.
The CryptoRate website is built on a Python and a web framework called Django.
 
#### **The main features that have currently been implemented are:**

1. Users can view list and detail information for crypto-currency.

2. Admin users can create and manage models. The admin has been optimised (the basic registration is present in admin.py, but commented out).

3. This website shows the real timing exchange rates of the crypto-currency.

Setup your development environment
Fork this repository to your account.

1. Create a virtual environment on your machine.   
   ````
   virtualenv -p python3 env
   ````
   
2. We recommend using python3-virtualenv. Any other packages would do fine though.

3. Activate the newly created virtual environment.

    ````
    cd env
    source bin/activate
   ````
4. Clone this repository (this would make rebasing easier).
   ````
   git clone https://github.com/chaudharypraveen98/CryptoRate.git
   ````
   
5. Install the dependencies for the project.
    ````
    cd website
    pip3 install -r requirements.txt
    ````
6. Change DEBUG=True in ``/CryptoRate/settings.py`` file (DO NOT COMMIT this change to settings.py in your PRs).

7. Run the migrations and collect static files.
    ``````
    python3 manage.py migrate
    python3 manage.py collectstatic
   ````
8. Run the live development server on your machine and test it.
   ````
   python3 manage.py runserver
   ````
    Once the server is started, open http://127.0.0.1:8000/home in a web browser. Everything went well if the webpage loads correctly and you don't see any errors.

9. Add a remote to your forked repository. This remote will be needed to push your changes to your repo.
    ````
   git remote add myfork https://github.com/<username>/website.git
   ````
