# spring5-servlet-context-changed
Spring 5 servlet context changed?

```groovy
allprojects { project ->

    tasks.withType(Test) {
        // Spring 5 sets this to ServletContext and it can't be read /WEB-INF/ resources.
        systemProperties = System.properties
    }

}
```
