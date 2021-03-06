---
layout: default
---

## Introduction
Start here if you are new to using the TOM Toolkit.

[Getting Started](/docs/getting_started) - First steps for getting a TOM
up and running.

[Workflow](/docs/workflow) - The general workflow used with TOMS.

## Extending and Customizing
Start here to learn how to customize the look and feel of your TOM or
add new functionality.

[Custom Settings](/docs/customsettings) - Settings available to the TOM Toolkit
which you may want to configure.

[Customizing your TOM](/docs/customize_templates) - Learn how to override
built in TOM templates to change the look and feel of your TOM.

[Adding Custom Target Fields](/docs/target_fields) - Learn how to add custom
fields to your TOM Targets if the defaults do not suffice.

[Building a TOM Alert Broker](/docs/create_broker) - Learn how to build
an Alert Broker module to add new sources of targets to your TOM.

[Running Custom Code Hooks](/docs/custom_code) - Learn how to run your own scripts
when certain actions happen within your TOM (for example, an observation
completes).

[Creating Plots from TOM Data](/docs/plotting_data) - Learn how to create plots
using plot.ly and your TOM data to display anywhere in your TOM.

## Deployment
Once you've got a TOM up and running on your machine, you'll probably want to
deploy it somewhere so it is permanently accessible by you and your collegues.

[Deploy to Heroku](/docs/deployment_heroku) - [Heroku](https://heroku.com) is a
PaaS that allows you to publicly deploy your web applications without the need
for managing the infrastructure yourself.

[Using Amazon S3 to Store Data for a TOM](/docs/amazons3) - Enable storing data on
the cloud stoage service Amazon S3 instead of your local disk.

## Contributing

[Contribution Guide](/docs/contributing) - If you find an issue, you need help with your TOM, you have a useful idea, or you wrote a module you'd like to be included in the TOM Toolkit, start with the contribution guide.


## Frequently Asked Questions

### I try to observe a target with LCO but get an error.

You might not have added your LCO api key to your settings file under the
`FACILITIES` settings. See [Custom Settings](/docs/customsettings#facilities) for
more details.

### How do I create a super user?
You can create a new superuser using the built in management command:

    ./manage.py createsuperuser

The `manage.py` file can be found in the root of your project.

Alternatively, you can give a user superuser status if you are already logged
in as a superuser by visiting the admin page for users:
[http://127.0.0.1/admin/auth/user/](http://127.0.0.1/admin/auth/user/)
