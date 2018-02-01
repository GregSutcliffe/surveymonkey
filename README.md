Access the SurveyMonkey API
====================================

Setup
-------------
Get an OAuth token for your SurveyMonkey account and add it to your .Renviron file like this:
`sm_oauth_token = "dslkajalsgjfaskgfjaslknfel`

API diagramming
-----------------
I laid out the nested list structure and some of the desired interim data.frame outputs here:
https://docs.google.com/document/d/1qZ8WfJ2bMW1qaL-ABd0JQJg9LROVlEI2aXyWffGaJX0/edit?usp=sharing


Usage
---------
Workflow for retrieving survey data:
* `browse_surveys()` returns a data.frame of your surveys
* `fetch_survey()` returns a survey object, to save on API calls
* `about_survey` returns information about a survey (*TBD*)
* `get_responses()` returns a survey's responses. You can specify an ID or name.
* ...
