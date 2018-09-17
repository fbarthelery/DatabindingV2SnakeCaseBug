Android gradle plugin databinding V2 bug with snake_case named variable
=======================================================================

When using databinding V2, variable name who contains and `_` make the compilation fails.

    ./gradlew -Pandroid.databinding.enableV2=true clean assemble

This compiles successfully in databinding v1:

    ./gradlew -Pandroid.databinding.enableV2=false clean assemble

This bug happens on version 3.1.4, 3.2.0-rc03, 3.3.0-alpha10 of the Android gradle plugin and possibly others.
