# Flask

## FLASK:

    - Setup a new Flask project
    - Run a simple Flask web application on your computer
    - Utilize basic configuration on a Flask project
    - Create a static route in Flask
    -Create a parameterized route in Flask
    - Use decorators run code before and after requests
    - Identify the "static" route
    - Use WTForms to define and render forms in Flask
    - Use WTForms to validate data in a POST with the built-in validators
    - Use the following basic field types in WTForms
    - BooleanField
    - DateField
    - DateTimeField
    - DecimalField
    - FileField
    - MultipleFileField
    - FloatField
    - IntegerField
    - PasswordField
    - RadioField
    - SelectField
    - SelectMultipleField
    - SubmitField
    - StringField
    - TextAreaField
    - Create a Flask Blueprint
    - Register the Flask Blueprint with the Flask application
    - Use the Flask Blueprint to make routes
    - Configure and use sessions in Flask
    - Use a Jinja template as return for a Flask route with render_template
    - Add variables to a Jinja template with {{ }}
    - Use include to share template content in Jinja

## Psycopg:

    - Connect to a PostgreSQL RDBMS using Psycopg
    - Open a "cursor" to perform data operations
    - Use results performed from executing a SELECT statement on existing database - - entities
    - Use parameterized SQL statements to insert, select, update, and delete data
    - Specify what type Psycopg will convert the following PostgreSQL types into:
    - NULL
    - bool
    - double
    - integer
    - varchar
    - text
    - date
    - Use the with keyword to clean up connections and database cursors

## Python Decorators:

### Callbacks
    - Python functions can be passed as arguments
    example: 
        ``` python
        def say_hi(name):
        print(f'Hi, {name}!')

        def say_good_morning(name):
        print(f'Good morning, {name}!')

        def say_something_to_curtis(say_something_func):
        return say_something_func('Curtis')

        say_something_to_curtis(say_hi)            # Hi, Curtis!
        say_something_to_curtis(say_good_morning)  # Good morning, Curtis!
        ```

### Introspection

    ability to examine objects to determine its behavior or type. You can use the built-in dir() function to observe the say_hi object.
    ``` python 
    def say_hi(name):
    print(f'Hi, {name}!')

    print(say_hi)       # <function say_hi at 0x1037a41f0>
    print(dir(say_hi))
    # ['__annotations__', '__call__', '__class__', '__closure__', '__code__', '__defaults__', '__delattr__', '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__get__', '__getattribute__', '__globals__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__kwdefaults__', '__le__', '__lt__', '__module__', '__name__', '__ne__', '__new__', '__qualname__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__']

    print(say_hi.__closure__) # None
    ```

## Inner functions
