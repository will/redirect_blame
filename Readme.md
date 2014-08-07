# 30(500) Redirect Blame
a.k.a. zero blametime deploys

See it in action at http://bitfission.com/redirect_blame

Zero-downtime deploys are hard. Why bother when you can trick your users into thinking their internet is a little flaky? They'll keep refreshing until your deploy is over.

Set this as your error page, and your users will see an error page that looks like their browser is having some trouble.

On heroku:

    heroku config:set \
    ERROR_PAGE_URL=http://bitfission.com/redirect_blame/index.html \
    MAINTENANCE_PAGE_URL=http://bitfission.com/redirect_blame/index.html

My site isn't down, your internet connection isn't working! This index.html file proves it.

Currently supports chrome, safari, and firefox. Other error pages welcome

## Thanks

* Dan Farina
* Bailey Parker
