# JPA based address book example

This is a simple example application about creating JPA backed Java EE application
with rich Vaadin based UI. Its not trying to be a good address book app, but it
demonstrates good technologies to create rich web applications your your custom
needs. The domain model is bit more complex than typical one table examples
to to demonstrated how to handle relations that you most likely have in you 
own domain model. It also demonstrates a very simple add-on usage with Vaadin 
(the iconic "switch" add-on).

## Run the example
```
git clone https://github.com/felixbarny/jpa-addressbook.git
cd jpa-addressbook
mvn wildfly:run
```

Open your browser at [http://localhost:8080]()

## Debug
You can connect to the application with remote debugging at port is 5005.

To get this running execute "mvn wildfly:run" to launch this locally on Wildfly
server. Or deploy to a Java EE 6+ server that support Java 8
properly, like Wildfly, Glassfish or latest TomEE. With Liberty you'll need to 
present a data source (other modern servers proved "development datasource" when 
no jta-datasource is present in persistence.xml). 

This is a suitable basis for small to medium sized apps. For larger applications,
consider using MVP to structure your UI code. See e.g. [this example 
application](https://github.com/peterl1084/cdiexample).


