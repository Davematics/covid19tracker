# covid19tracker

Infodemics ([infodemics.com](https://infodemics.com)) uses existing social hierarchies in a community to efficiently and effectively communicate health risk.

The World Health Organisation (WHO) has a [simple message](https://twitter.com/WHO/status/1239581568101945348) for all countries: Test, test, test every suspected COVID19 case.

Infodemics, as a risk communication platform hopes that [this tracker](https://infodemics.com/covid19tracker) would help with this effort.

## What the tracker does

* [The Public](/img/covid19tracker-user-germinal.gif)
* [Health Agencies](/img/covid19tracker-admin.gif)

## The Tracker API

We have included the Postman collection [here](Infodemics-COVID19-Tracker.postman_collection.json). 

Also, the test/dev Infodemics url is _https://test.infodemics.com_, please contact us when you need to publish your solution.

But just to give you a highlight:

### Get tracker data (circle/covid19_tracker)
Read (and then display) existing tracker data.

Note that this has the potential to be bulky (locations especially) and will also have to be obfuscated/censored soon (also locations too).

### Get suggested profile (profile/suggest?meta=meta)
The tracker needs users to fill certain details. This request help with some random fillers for people who wish to be anonymous.

Phone number must be provided later though.

Please note that suggested names are of the form "adjective"+"nigerian noun". And "adjective" might not be flattering.

Names are from the project [stigwue/naija_pikin](https://github.com/stigwue/naija_pikin).

### Submit tracker data (media/covid19_submit)
Submit the provided user data to the tracker so that information can be handled at the backend by CDC.

See details in this [image](/img/covid19_submit.png).


## Request For Comments (wow, I feel so old using RFC!)
Okay, so what next is needed to be done?

* We would like to make filling the forms easier, provide options people must choose from too.
* We would like to do more with the provided location data:
	* perhaps use the [Haversine formula](https://en.wikipedia.org/wiki/Haversine_formula) to drop some of them if they're quite close?
	* tie location to time so we can show a trail?
	* tag other locations of interest to the effort?
* More tools for the health agencies
	* Improve on current comuniciation channels (email and SMS)
	* Help with more reports and collaboration

## Contact us
Send us an [email](mailto:info@infodemics.com) or follow us on [Twitter](https://twitter.com/infodemics1). We write about our work on our [blog](https://infodemics.com/blog) and on LinkedIn.
