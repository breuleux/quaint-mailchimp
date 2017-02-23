
# quaint-mailchimp

MailChimp integration for Quaint.


## Install

In your Quaint project directory, run the command:

    quaint --setup mailchimp

The setup will prompt you for an API key, which it will use to fetch
information about your mailing lists. The API key will not be saved in
the configuration.


## Sample usage

```
mailchimp ::
  list =>
    list name or id
  body =>
    Subscribe to our amazing mailing list!
  label =>
    Subscribe!
  emailPlaceholder =>
    E-mail address
```


## mailchimp macro

The `mailchimp::` macro takes a list of named arguments:

**list** is the name or id of the list you want to generate a subscribe form for.

**body** is Quaint markup that will be displayed above the form.

**label** is the label of the subscribe button (default: "Subscribe!")

**emailPlaceholder** is the placeholder for the e-mail address input
(default: "E-mail address")

