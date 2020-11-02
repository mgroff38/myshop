Matthew Groff
CIDM 6325 

Online shop project.

##Issues
1. Issue with weasyprint - needed Cairo, after installing Cairo Packages unable to find Django. 
    Redid virtual env, limited install to weasprint v 51. Install of Cairo not needed.

2. Issue with parler and Python 39. 
    -add from django.forms.boundfield import BoundField to Forms.py of django
    -add pretty_name to forms.py of django. 




## Notes
source env/myshop/bin/activate
pip install celery==4.4.2
pip install flower
pip install braintree==3.59.0
pip install WeasyPrint==51

brew services start rabbitmq
brew services restart rabbitmq

celery -A myshop worker -l info
celery -A myshop flower


Not necessary to install WeasyPrint for Final Project
****Evaluate for PDF install
brew install cairo
brew install pango

Use of OnlineShop for final makes sense, need to customize for BBQ and stop before PDF implementation. Add PDF at End if time permits.