# <a href="https://apres-apparel.herokuapp.com/">Après Apparel</a>

![responsive_screenshot]()

This [project](https://apres-apparel.herokuapp.com/) is my fourth milestone project (Full Stack Frameworks with Django) in Full Stack Software Development course run by [Code Institute](https://codeinstitute.net/)

Après Apparel is an outdoor lifestyle brand founded by my friend, Stephen Rice, with the main aim of manifesting a positive brand image & culture amongst those who lead active lifestyles whilst also supplying apparel & accessories to suit 
those lifestyles.
The approach of this business relies heavily on creating community & a culture around the brand and team members, rather than being detached and strictly ecommerce for products.
The Après Apparel vision is to build a strong following around the brand & its values on social media & to hopefully use that platform to give back and support that community.

---

## Table of Contents
1. [**UX**](#ux)
    - [**User Stories**](#user-stories)
    - [**Design**](#design)
        - [**Framework**](#framework)
        - [**Color Scheme**](#color-scheme)
        - [**Icons**](#icons)
        - [**Typography**](#typography)

2. [**Features**](#features)
    - [**Existing Features**](#existing-features)
    - [**Features Left to Implement**](#features-left-to-implement)

3. [**Technologies Used**](#technologies-used)
    - [**Front-End Technologies**](#front-end-technologies)
    - [**Back-End Technologies**](#back-end-technologies)

4. [**Testing**](#testing)
    - [**Validators**](#validators)
    - [**Compatibility**](#compatibility)
    - [**Known Issues**](#known-issues)
    - [**Automated Testing**](#automated-testing)

5. [**Deployment**](#deployment)
    - [**Local Deployment**](#local-deployment)
    - [**Remote Deployment**](#remote-deployment)

6. [**Credits**](#credits)
    - [**Content**](#content)
    - [**Media**](#media)
    - [**Code**](#code)
    - [**Acknowledgements**](#acknowledgements)

---

## UX

This project is part of my [Code Institute](https://codeinstitute.net/) Full Stack Software Development Diploma Course, specifically the **Full Stack Frameworks** module.
The objective for this project is to "Create a web application that allows users to browse & purchase products, register/login/logout & provide delivery information securely, display team members behind the brand & real athletes we wish to support in future." 
This e-commerce site is made for those who love sport, adventuring and the outdoors!
We also have a section dedicated to athletes we support & follow, and the team members behind the Après Apparel brand, with social media links provided
for any curious visitors to site to check out.

"**_As a user, I would like to_** _____________________________"

:white_check_mark: *denotes items that have been successfully implemented*

- :white_check_mark: *view the site* from **any device** *(mobile, tablet, desktop)*.
- :white_check_mark: *view all products* as a **Guest**.
- :white_check_mark: *view individual product details* as a **Guest**.
- :white_check_mark: *add products to my shopping bag* as a **Guest**.
- :white_check_mark: *remove products from my shopping bag* as a **Guest**.
- :white_check_mark: *manage products in my shopping bag* as a **Guest**
- :white_check_mark: *sort/order products* by **name, category, price, rating**.
- :white_check_mark: *search products* by **name, category, description**.
- :white_check_mark: **limit** the number of *products* to display by name (alphabetical sorting), product category type, or see *all products*.
- :white_check_mark: *create* my **own profile** with secure email verification as a **User**.
- :white_check_mark: *update* & *manage* my **email address, password, delivery information** as a **Registered User**.
- :white_check_mark: *view* **bag subtotal** whilst browsing the store as a **Guest/User**.
- :white_check_mark: *view* **bag contents** whilst browsing the store as a **Guest/User**.
- :white_check_mark: *add* **products** as a **Store Owner/Admin**.
- :white_check_mark: *edit* **products** as a **Store Owner/Admin**.
- :white_check_mark: *delete* **products** as a **Store Owner/Admin**.
- :white_check_mark: be able to **log out**.


### Design 

- The design of the Après Apparel website is a monochromatic color scheme to fit in line with a simplistic high contrast aesthetic, with various star/sunset background images used across the site to 
symbolize the outdoor lifestyle the brand wishes to promote.

#### Framework

- [Bootstrap 4.6.0](https://getbootstrap.com/)
    - My preferred CSS framework for this project because of the simple-to-understand documentation & simplicity of use.
- [jQuery 3.6.0](https://code.jquery.com/jquery/)
    - In an effort to keep the JavaScript minimal, I have decided to use jQuery as foundation to my scripts framework.
- [Django 3.1.0](https://www.djangoproject.com/download/)
    - Django is a free and open-source web framework that I've used to render the back-end Python with the front-end Bootstrap4 CSS3 Framework and AnimateCSS Library. 

#### Color Scheme

- Color scheme is a simple monochromatic scheme (Predominantly Black / White) which fits in with the Surf/Mountain aesthetic the brand falls in line with.
Another reason for the monochromatic color scheme is that it provides high contrast between text & background elements which makes it easier for visitors to visually distinguish and navigate the site.

#### Icons

- [Font Awesome 5.15.3](https://fontawesome.com/)
    - Font Awesome was my preferred source for icon use across the site rather than Materialize Icons. Font Awesome Icons are simplistic & easily customizable and displayed through *classes* rather than *text*
    which fits the aesthetic Après Apparel is targetting.

#### Typography

- [Google Fonts](https://fonts.google.com/) were used across the site:
- [Montserrat](https://fonts.google.com/specimen/Montserrat#standard-styles) : default font.
- [AnimateCSS](https://animate.style/) : Animations used for landing, team & athlete page.
- [Bootstrap](https://getbootstrap.com/) : Typography / Colors Documentation from Bootstrap was used in various headings/texts/alerts around the site such as ".display-x" & ".text-success" classes.


## Features
 
### Existing Features

**Register Account** 
- Anybody can register for free and create their own unique account. There is built-in authentication and authorization to check certain criteria is met before an account is validated. All passwords are hashed for security purposes!

**Log In to Account**
- Log in to existing account securely with Allauth (Django Integrated set of Applications) that addresses sewcure authentication, registration, email confirmation & account management.

**Manage Account**
- Existing users are able to manage details associated with that account such as adding/updating delivery information, account password and primary emails.

**Log Out of Account**
- Existing users can choose to log out if they are finished using the website. 

**View all Products**
- Both registered users & guests can view all existing products available on the site. 

**Search all Products**
- Both registered users & guests can search existing products available on site via search bar on desktop view & mobile.

**Filter Products**
- Both registered users & guests can filter existing products available on site by name, sizes, price, category, rating.

**Manage Products**
- Registered users can view account order history & all associated information such as date/price/item/qty/order number. They can also manage any items in their shopping bag.

**Add Products**
- [CRUD] Store Owners / Superusers can add new products to the website or update/delete current products. Certain defensive programming measures have been implemented such as only granting this permission to registered superusers/store owners.

**Admin**
- Django Admin application that allows superusers / store owners to manually create, update or delete any existing models or products from the store.

**About Us**
- Section designated to showcasing sponsored athletes & the team behind the Après Apparel brand.


## Technologies Used

- ![GitPod]
    - [GitPod](https://www.gitpod.io/) - Used as my primary IDE for developing projects.
- ![GitHub]
    - [GitHub](https://github.com/) - Used as remote storage of my projects online.


### Front-End Technologies

- ![HTML5]
    - [HTML5](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5) - Used as the base for markup text.
- ![CSS3]
    - [CSS3](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS3) - Used as the base for cascading styles.
- ![jQuery 3.4.1]
    - [jQuery 3.4.1](https://code.jquery.com/jquery/) - Used as the primary JavaScript functionality.
- ![Bootstrap 4]
    - [Bootstrap 4.6.0](https://getbootstrap.com/) - Used as the front-end framework for layout and design.
- ![Stripe API]
    - [Stripe API](https://stripe.com/docs/api?lang=python) - Used to make secured payments on *Feature Tickets*.
- ![Amazon AWS S3]
    - [Amazon AWS S3](https://aws.amazon.com/) - Used to store *staticfiles* and *media* folders and files.

### Back-End Technologies


- ![Python]
    - [Python 3.6.7](https://www.python.org/) - Used as the back-end programming language.
- ![Django]
    - [Django 2.2.16](https://docs.djangoproject.com/en/2.2/) - Used as my Python web framework.
- ![Heroku]
    - [Heroku](https://www.heroku.com) - Used for *"Platform as a Service"* (PaaS) for app hosting.
- ![PostgreSQL 11.4]
    - [PostgreSQL 11.4](https://www.postgresql.org/) - Used as relational SQL database plugin via Heroku.
    

Further details on all Python packages used on this project can be found in the [requirements.txt](project/requirements.txt) file. Each of these is outlined below (click below to expand the dropdown), with the package version and a brief description.