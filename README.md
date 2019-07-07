# Dokku Angular Issue
This project illustrates an issue with Angular apps deployed using Dokku.  Once the app loads the first time, manually entering a URL and attempting to navigate to it will always result in the nginx 404 page.

# You can reproduce the issue by following these steps:

1. Clone the project.
2. `cd` into the project directory.
3. Add your remote `git remote add dokku dokku@yoursite.com:example`
4. Run `git push dokku master`
5. Navigate to example.yoursite.com.  Notice how the page loads fine
6. Reload the browser and view the nginx 404 page.  
7. Alternatively the app has two routes: `/home` and `/about`.  Attempt to navigate to a URL directly E.G. `http://example.yoursite.com/about` and view the nginx 404 page

You can view this issue (#3608) in the Dokku Github repo: https://github.com/dokku/dokku/issues/3608
