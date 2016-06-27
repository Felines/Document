Contact Page
============

The values of form on the page are bound to appropriate properties of a ContactFormDTO object.

When the submit button is pressed the View call the SendContactForm() on its ContactViewModel, which sends the form using EmailAddressFacade.

EmailAddressFacade provides a simple interface to send various kinds of emails to the users.