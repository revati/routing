This Laravel 4 package provides a additional routes for soft deletable resources:

- route for restoring resource `PUT/PATCH`
- route for force deleting resource `DELETE` (default delete used as soft delete)
- route for trashed resources list `GET`

## Installation

Begin by installing this package through Composer. Edit your project's `composer.json` file to require `revati/routing`.

    "require": {
        "laravel/framework": "4.1.*",
        "revati/routing": "dev-master"
    }

Next, update Composer from the Terminal:

    composer update

Once this operation completes, the final step is to add the service provider. Open `app/config/app.php`, and add a new item to the providers array.

    'Revati\Routing\RoutingServiceProvider'

That's it! You're all set to go.

