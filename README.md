# AirBnB Clone V4

This is a complete full-stack web application, integrating a MySQL database and Flask RESTful API with a dynamic HTML5/CSS3/jQuery front-end.

It was based off the basic characteristics of the Airbnb platform.

![](./readme_images/web_dynamic_diagram.png)

# Iterations

The project was developed in several iterations, being V4 the last one. This iterations encompassed several concepts and integrations that will be explained below.

## The Console

The first iteration of the project consisted on building an interactive console in order to allow for development testing.

![The Console](./readme_images/the_console_diagram.png)

The Console was coded in order to work with a temporary storage engine based on JSON, and included the next features:

- Create a new object (ex: a new User or a new Place)
- Retrieve an object from a file, a database etc…
- Do operations on objects (count, compute stats, etc…)
- Update attributes of an object
- Destroy an object

The console has 2 modes.

**Interactive**

```
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
```

**Non Interactive**

```
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
```

## Web Static

This part of the project consisted in building the basic CSS and HTML source code.

![](./readme_images/web_static_diagram.png)

![](./readme_images/web_static.png)

## MySQL

This section consisted on the data modeling for the relational database in MySQL.

![](./readme_images/mysql_diagram.png)

![](./readme_images/mysql_model.jpg)

## Web Framework

This iteration consisted on building the first approach to dynamic content for the application by using Flask and Jinja, and effectively having Server Side Render.

For this development, the MySQL database started being used in order to serve content to the client, and provide it with back end based features.

All of the HTML and CSS source code started being hosted in the server, and no items were hard coded, but instead produced through dynamic data integration.

![](./readme_images/web_framework.jpg)
