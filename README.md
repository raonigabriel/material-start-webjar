Material Start WebJar
-------------------

Long before nodejs, bower, grunt, gulp, yeoman... there was Maven.

Don´t get me wrong: I do acknowledge the power of nodejs + gulp. I just want to prove that there are another options.
It is already 2016 and some nodejs plugins still have some problems when running under Windows. What if you could use a cross-platform, proven and stable tool that only requires Java?

This project is a clone of [Angular Material Start](https://github.com/angular/material-start) that uses Maven instead of nodejs to manage the dependencies and control the build process. It is a proof of concept: I can´t accept the hype on those frontend tools so I decided to show how the same achieve the same result but using old-but-gold Maven instead. This could also be done using [Gradle](https://gradle.org/).

This sample application is intended to be useful as both a learning tool and a skeleton application
for a typical [AngularJS Material](http://material.angularjs.org/) web app: comprised of a Side navigation
area and a content area. You can use it to quickly bootstrap your AngularJS webapp projects and dev
environment for these projects.

#Features:

1. Based on [Angular Material 1.1.0](https://material.angularjs.org/latest/)
2. Uses [Maven](https://maven.apache.org/) for dependency management and build instead of nodejs. 
  1. All 'static' dependencies are downloaded and unpacked inside 'node_modules'
  2. Uses [jetty-plugin](https://www.eclipse.org/jetty/documentation/9.3.x/jetty-maven-plugin.html) featuring hot-reloading (somewhat like live-server)
3. No changes to the original folder structure and no changes to the original code and markup.
4. It can be used side-by-side with nodejs.
5. The final output is a packed JAR file that can be used as a [WebJar](http://www.webjars.org/documentation). Hence, it can be used as a dependancy on another project.

To get the code:
-------------------
Clone the repository:

    $ git clone https://github.com/raonigabriel/material-start-webjar.git

If this is your first time using Github, review http://help.github.com to learn the basics.

To run the application:
-------------------	
From the command line with Linux or Windows:

    $ cd material-start-java
    $ mvn jetty:run

From the command line with Mac:

    $ echo 'Do yourself a favor and get LinuxMint!'

Access the deployed web application [http://localhost:8080](http://localhost:8080)

## License

Released under the [MIT license](https://opensource.org/licenses/MIT)