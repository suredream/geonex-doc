# Deploy GeoNEX











## Appendix

### Build GeoNEX doc on readthedocs @ sami

So far the GeoNEX doc is hosted on [here](https://github.com/suredream/geonex-doc) as a public repository, building on readthedocs and accessible at:

[https://geonex.readthedocs.io/en/latest/](https://geonex.readthedocs.io/en/latest/).



1. Signing up to Read The Docs: <https://readthedocs.org/accounts/signup/>

2. Verify email address

3. Linking to Github account

​	- Click on "Import a Project" button

If you were not previously connected:

​	- Click on "Connect to GitHub" button (note: it works with gitlab as well)

​	- Click on "Authorize readthedocs"

​	Your repos will appear as a list

4. Adding a repo 

Click on + sign of the repo you want to add

​	in Name: field enter the URL you want ex: geonex

​		ATTENTION: this is irreversible, choose name carefully

​	click Next

​	click Admin tab

​	select "mkdocs" instead of default "sphinx" in Documentation type

​	click Save

​	build failed -> reason: unrecognized configuration "nav"

​		turns out Read The Docs uses an old version of mkdocs

Fixing old version issue of mkdocs

​	Under project:

​	click Admin

​	click Advanced Settings

​	in requirements file add the entry "mkdocs==1.0.4" 

click Save (this should resolve the build issue)

After few minutes, visit the URL <https://geonex.readthedocs.io/en/latest/>

​	

​	

