# github-action-pipeline
This repo is a ci/cd pipeline to deploy flutter mobile apps to Google Play Store and App Store on i0S


### iOS ci/cd pipeline to come soon.

Two important things to get done. 

- To create the Google Play JSON key. Head to Google Cloud Platform. On creating a new project or an existing one, search for _APIs & Services_ on the search bar. Enable 3 APIs, use again the search bar: 
Google Play Android Developer API, Google Play Developer Reporting API, Google Play Games Services Publishing API. But enabling Google Play Android Developer API is enough. After enabling them, go to _IAM & Admin_ and create a Service Account (or can use an existing one), fill the fields and save. On the Service account create a new key in JSON, it will download to your system. Copy the key and head to actions and secret and create a variable for [GOOGLE_PLAY_JSON] and save.

- The second part, head to Google Play Developer console. Go to _User & Permissions_ and invite a new user. The new user is the client email account of the Service account created earlier and assign it the right permission. One of which must be; View app information (read-only). Manage production releases (for uploading to the production track). Hit save.

Run the pipeline and good luck.

