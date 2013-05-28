# Pusher on OpenShift using PHP

This git repository provides a quickstart demonstrating how to use Pusher on OpenShift in a PHP application.

## Create an OpenShift App

Create an account at http://openshift.redhat.com and set up your local machine with the [client tools](https://www.openshift.com/get-started).

Create a PHP 5.3 application. Rename `realtimeapp` to something else if you like.

    rhc app create realtimeapp php-5.3 --from-code https://github.com/pusher/pusher-php-openshift-quickstart
    cd realtimeapp

## Sign up for a free Pusher account

1. Sign up via http://pusher.com/signup
2. Take a note of your application credentials: `app_id`, `app_key` and `app_secret`
3. Replace the values in `php/config.php` with the credentials

## Deploy your Pusher application

    git add .
    git commit -m "my first commmit"
    git push origin master

## Run your Pusher application 

    http://myapp-<yournamespace>.rhcloud.com

## More Information

* Pusher documentation: http://pusher.com/docs
* Debugging your application: http://pusher.com/docs/debugging
* Pusher client and server libraries: http://pusher.com/docs/libraries
* Pusher Support on StackOverflow: http://stackoverflow.com/questions/tagged/pusher