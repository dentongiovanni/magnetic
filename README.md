"# magnetic" 


ADD THIS TO YOUR composer.json

  "extra": {
        "laravel": {
            "providers": [
                "Magnetic\\Planner\\Providers\\PlannerServiceProvider",
                "Magnetic\\Planner\\Providers\\PlannerEventServiceProvider"
                
            ],
            "dont-discover": []
        }
    },
    "autoload": {
        "psr-4": {
            "App\\": "app/",
            "Magnetic\\Planner\\": "packages/magnetic/planner/src",
            "Magnetic\\Planner\\Models\\": "packages/magnetic/planner/src/Models",
            "Magnetic\\Planner\\Providers\\": "packages/magnetic/planner/src/Providers",
            "Magnetic\\Planner\\Events\\": "packages/magnetic/planner/src/Events/",
            "Magnetic\\Planner\\Listeners\\": "packages/magnetic/planner/src/Listeners/"
        },

EXECUTE composer dump-autoload

EXECUTE php artisan migrate to install db tables


NOTE: Dont forget to modify your email config

