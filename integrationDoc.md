# Setup PHP

Follow the instructions below to send custom events from your PHP backend.

## Dependency Setup

````
{
    "require": {
        "ablaevent/ablaevent-php": "1.0.*"
    }
}
````

## Install

````
php composer.phar install
Configure
PostHog::init('PHC',
    array('host' => 'https://e.abla.io')
);
````

## Send an Event

````
PostHog::capture(array(
    'distinctId' => 'test-user',
    'event' => 'test-event'
));

````
