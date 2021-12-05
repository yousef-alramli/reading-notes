# Django Tutorial Part 3: Using models

## Designing the LocalLibrary models
while designing your models it makes sense to have separate models for every "object" (a group of related information). In this case, the obvious objects are books, book instances, and authors. also use models to represent selection-list options.

## Model primer

Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata. 

### Fields
A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.

### Common field arguments
The following common arguments can be used when declaring many/most of the different field types:

- **help_text**: Provides a text label for HTML forms (e.g. in the admin site), as described above.
- **verbose_name**: A human-readable name for the field used in field labels. If not specified, Django will infer the default verbose name from the field name.
- **default**: The default value for the field. This can be a value or a callable object, in which case the object will be called every time a new record is created.
- **null**: If True, Django will store blank values as NULL in the database for fields where this is appropriate (a CharField will instead store an empty string). The default is False.
- **blank**: If True, the field is allowed to be blank in your forms. The default is False, which means that Django's form validation will force you to enter a value. This is often used with null=True , because if you're going to allow blank values, you also want the database to be able to represent them appropriately.
- **choices**: A group of choices for this field. If this is provided, the default corresponding form widget will be a select box with these choices instead of the standard text field.
- **primary_key**: If True, sets the current field as the primary key for the model (A primary key is a special database column designated to uniquely identify all the different table records). If no field is specified as the primary key then Django will automatically add a field for this purpose.

### Common field types
The following list describes some of the more commonly used types of fields.

- **CharField** is used to define short-to-mid sized fixed-length strings. You must specify the max_length of the data to be stored.
- **TextField** is used for large arbitrary-length strings. You may specify a max_length for the field, but this is used only when the field is displayed in forms (it is not enforced at the database level).
- **IntegerField** is a field for storing integer (whole number) values, and for validating entered values as integers in forms.
- **DateField and DateTimeField** are used for storing/representing dates and date/time information (as Python datetime.date in and datetime.datetime objects, respectively). These fields can additionally declare the (mutually exclusive) parameters auto_now=True (to set the field to the current date every time the model is saved), auto_now_add (to only set the date when the model is first created) , and default (to set a default date that can be overridden by the user).
- **EmailField** is used to store and validate email addresses.
- **FileField and ImageField** are used to upload files and images respectively (the ImageField adds additional validation that the uploaded file is an image). These have parameters to define how and where the uploaded files are stored.
- **AutoField** is a special type of IntegerField that automatically increments. A primary key of this type is automatically added to your model if you don’t explicitly specify one.
- **ForeignKey** is used to specify a one-to-many relationship to another database model (e.g. a car has one manufacturer, but a manufacturer can make many cars). The "one" side of the relationship is the model that contains the "key" (models containing a "foreign key" referring to that "key", are on the "many" side of such a relationship).
- **ManyToManyField** is used to specify a many-to-many relationship (e.g. a book can have several genres, and each genre can contain several books). In our library app we will use these very similarly to ForeignKeys, but they can be used in more complicated ways to describe the relationships between groups. These have the parameter on_delete to define what happens when the associated record is deleted (e.g. a value of models.SET_NULL would set the value to NULL).

# Django Tutorial Part 4: Django admin site
The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records. This can save you a lot of time during development, making it very easy to test your models and get a feel for whether you have the right data. The admin application can also be useful for managing data in production, depending on the type of website. The Django project recommends it only for internal data management (i.e. just for use by admins, or people internal to your organization), as the model-centric approach is not necessarily the best possible interface for all users, and exposes a lot of unnecessary detail about the models.

## Registering models
First, open admin .py in the catalog application (/locallibrary/catalog/admin.py).

## Creating a superuser
In order to log into the admin site, we need a user account with Staff status enabled. In order to view and create records we also need this user to have permissions to manage all our objects.  You can create a "superuser" account that has full access to the site and all needed permissions using manage.py.

## Logging in and using the site
To login to the site, open the /admin URL (e.g. http://127.0.0.1:8000/admin) and enter your new superuser userid and password credentials (you'll be redirected to the login page, and then back to the /admin URL after you've entered your details).

## Advanced configuration
Django does a pretty good job of creating a basic admin site using the information from the registered models:

- Each model has a list of individual records, identified by the string created with the model's __ str__() method, and linked to detail views/forms for editing. By default, this view has an action menu at the top that you can use to perform bulk delete operations on records.
- The model detail record forms for editing and adding records contain all the fields in the model, laid out vertically in their declaration order.  

*You can further customise the interface to make it even easier to use. Some of the things you can do are:*

- List views:
    - Add additional fields/information displayed for each record.
    - Add filters to select which records are listed, based on date or some other selection value (e.g. Book loan status).
    - Add additional options to the actions menu in list views and choose where this menu is displayed on the form.
- Detail views
    - Choose which fields to display (or exclude), along with their order, grouping, whether they are editable, the widget used, orientation etc.
    - Add related fields to a record to allow inline editing (e.g. add the ability to add and edit book records while you're creating their author record).

## Register a ModelAdmin class
To change how a model is displayed in the admin interface you define a ModelAdmin class (which describes the layout) and register it with the model.

## Configure list views
The LocalLibrary currently lists all authors using the object name generated from the model __ str__() method. This is fine when you only have a few authors, but once you have many you may end up having duplicates. To differentiate them, or just because you want to show more interesting information about each author, you can use list_display to add additional fields to the view.

## Add list filters
Once you've got a lot of items in a list, it can be useful to be able to filter which items are displayed. This is done by listing fields in the list_filter attribute. Replace your current BookInstanceAdmin class with the code fragment below.


