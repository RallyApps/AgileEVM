Rally Agile EVM
======================

![Title](https://raw.github.com/RallyApps/AgileEVM/master/screenshots/title-screenshot.png)

## Overview

The Agile EVM app is an adaptation of the traditional project management practice of measuring actual value of integrated cost, schedule and scope against a baseline plan using Earned Value Management (EVM) metrics. The methods of measurement have been adapted to easily fit within the scrum project management framework.

For more information on Agile EVM, consult these articles:

* [AgileEVM: Measuring Cost Efficiency Across the Product Lifecycle](http://www.infoq.com/articles/agile-evm), Tamara Sulaiman, Oct 2007
* Estimating and Tracking Agile Projects, Bachir Kane, May 2007

## How to Use

### Running the App

If you want to start using the app immediately, create an Custom HTML app on your Rally dashboard. Then copy App.html from the deploy folder into the HTML text area. That's it, it should be ready to use. See [this](http://www.rallydev.com/help/use_apps#create) help link if you don't know how to create a dashboard page for Custom HTML apps.

Or you can just click [here](https://raw.github.com/RallyApps/AgileEVM/master/deploy/App.html) to find the file and copy it into the custom HTML app.

### Using the App

To provide valuable results, your agile team should do the following:

* The project should have at least one release
* Developers must consistently populate the Actuals field on all their tasks
* All stories in the release should have their Plan Estimate field populated during release planning

The app assumes the following default values:

* Blended hourly rate for an employee. Default = $50/hour.
* Ratio between story points and task hours. Default = 5.
* Variance for Green, Yellow, and Red indicators. Default = 5.
* Variance of 5: >95% green, 85% to 94% yellow, < 84% red.
* Variance of 10: >90% green, 80% to 89% yellow, < 79% red.

####Change default values

To change the default values above, copy the app code to a Custom HTML app and edit the following variables in the Global Variables section:

* _billableRate: blended hourly rate for an employee.
* _multiplier: Ratio between story points and task hours. Ex: If a story point is equivalent to five ideal developer hours , the multiplier is 5.
* _baseVar : variance for Green, Yellow, and Red indicators. Options are 5 or 10.

## Customize this App

You're free to customize this app to your liking (see the License section for details). Since this app uses a very old version of Rally's SDK, the app is only presented in its deployed form.

## License

AgileEVM is released under the MIT license.  See the file [LICENSE](https://raw.github.com/RallyApps/AgileEVM/master/LICENSE) for the full text.
