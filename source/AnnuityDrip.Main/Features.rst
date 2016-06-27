Features Page
=============

The 'Features' page contains mostly plain text and a simple Trial Registration form. The very same form that you can find on the :doc:`Index`.

The ViewModel contains a few interesting properties and methods:

* Its *Testimonials* property contains the various quotes that you can see below the subscription plans. These are loaded into a dot:Repeater and are perceived as a carousel by the user.

* It also contains validation methods like: *CheckEmailChanged()* and *IsEmailUnique()*, that ensure that the Trial Registration form is filled with valid information and that an already registered user cannot register again with the same email address.

* When the user presses the *GET STARTED* button, the *RegistrationTrial()* method is called. First, it checks if all the information in the form is valid and passes it to an AgentFacade that saves the user into the database and to *EmailAddressFacade* that sends the Registration and Confirmation email to the newly registered agent.
