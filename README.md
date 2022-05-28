# Project Name 


# Problem Description
```As a fan of geometry,
I want to model a line based on points consisting of (x, y) coordinates using the cartesian system,
So that I can calculate its length.
```

# Prerequisites
* java version "17"
* Gradle 7.4.2


# Build instructions
Build the project : `gradle build` <br>
Build the project after cleaning : `gradle clean build`


# Run instructions
Run all test : `gradle test` <br>
Run all test after cleaning : `gradle test` 


#### Add these to show testcases passing in console

```import org.gradle.api.tasks.testing.logging.TestExceptionFormat
import org.gradle.api.tasks.testing.logging.TestLogEvent

test {

    testLogging {
        events TestLogEvent.FAILED,
                TestLogEvent.PASSED,
                TestLogEvent.SKIPPED,
                TestLogEvent.STANDARD_ERROR,
                TestLogEvent.STANDARD_OUT
        exceptionFormat TestExceptionFormat.FULL
        showCauses true
        showExceptions true
        showStackTraces true
    }
    useJUnitPlatform()
}
```