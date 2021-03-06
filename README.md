#Croissant

Croissant is a simple, minimal, lightweight blogging app written on the Laravel 
framework. Croissant isn't a full fledged CMS, nor is it overloaded with a ton
of features.

The project takes inspiration from Eric Barnes's [Wardrobe](http://wardrobecms.com),
but strays away from some of the more advanced techniques Eric has implemented
with Wardrobe. Like Wardrobe, Croissant also allows you to post your content 
using markdown syntax.

##Installation

*These installation instructions assume you already have [Composer](http://getcomposer.org/) 
installed.*

Clone the repo:

    $ git clone https://github.com/jesseterry/croissant.git

Edit app/config/database.php to configure your database.

Give appropriate permissions to the app/storage folder:

    $ chmod -R 777 app/storage

Run the following from the root of your project to install Laravel and all the 
dependencies:

    $ php composer install

Then run the migrations:

    $ php artisan migrate

Then seed the database:

    $ php artisan db:seed

The database will create a sample post, sample page content, and a default user
account with admin / password as the username / password.

##Using Croissant

Point your browser to the public folder to view the main site.

Point your browser to public/admin to log in to the admin area.
