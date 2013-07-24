# 30(500) Redirect Blame
a.k.a. zero blametime deploys

See it in action at http://bitfission.com/redirect_blame

My site isn't down, your internet connection isn't working. This index.html file proves it.  Set it as your error page, and your users will be non-the-wiser that you're site is down.

On heroku:

    heroku config:set \
    ERROR_PAGE_URL=http://bitfission.com/redirect_blame/index.html \
    MAINTENANCE_PAGE_URL=http://bitfission.com/redirect_blame/index.html
