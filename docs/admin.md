# Deploy GeoNEX











## Appendix

### Build GeoNEX doc on readthedocs @ sami - sami@Jun: done

So far the GeoNEX doc is hosted on [here](https://github.com/suredream/geonex-doc) as a public repository, building seamlessly after commits on readthedocs and accessible at:

[https://geonex.readthedocs.io/en/latest/](https://geonex.readthedocs.io/en/latest/).

To setup the above continuous integration mechanism, follow these steps:

1. Create a ReadTheDocs account
	* Sign up to ReadTheDocs: <https://readthedocs.org/accounts/signup/>

	* Verify email address


2. Link to Github account

	* Make sure you are on the main page of ReadTheDocs
	* Click on "Import a Project" button
	* If you were not previously connected, Click on "Connect to GitHub" button (note: it works with gitlab as well)
​	* Otherwise, Click on "Authorize readthedocs"
​	* Your repos will appear as a list

3. Adding a Github repo 
	* Make sure you are on the main page of ReadTheDocs
	* Click on + sign of the repo you want to add
	* in Name field, enter the project name you want, ex: geonex. Note that this will automatically be part of your base URL - ATTENTION: this is irreversible, choose name carefully
	* click Next
	* click Admin tab
	* select "mkdocs" instead of default "sphinx" in Documentation type
	* click Save
	* you will get: build failed -> reason: unrecognized configuration "nav". It turns out Read The Docs uses an old version of mkdocs

4. Fixing old version of mkdocs issue
	* Make sure you are on the main page of ReadTheDocs, under desired project.
	* click Admin
	* click Advanced Settings
	* in requirements file, add the entry "requirements.txt".
	* create a requirements.txt file in your github home directory with the following content:
		* mkdocs==1.0.4 
	* click Save (this should resolve the build issue)
	* After few minutes, visit the URL <https://geonex.readthedocs.io/en/latest/>

​	

​	

