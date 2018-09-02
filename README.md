# django-contactus

The application can be easily extended by other modules.

Installation

Install the package via pip: pip install django-contactus. It's preferred to install the module in a virtual environment.

Configuration

settings.py:
```
INSTALLED_APPS += (
    'contactus',
)
```
Add a CONTACT_US_EMAIL setting to specify the email address that submissions will be sent to.You also need your Django app to be configured properly to send email.

urls.py:
```
('^contactus/', include('contactus.urls')),
```
In any template, you can link to the contact page with ```{% url 'contactus' %}```.
