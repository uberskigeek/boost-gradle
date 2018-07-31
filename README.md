# boost-gradle
Boost Gradle repository

This is an initial attempt at using the greeting plugin to have a dependency on the
liberty gradle plugin that will install liberty locally. 

This is an exercise in attempting to understand Plugin relationships for Gradle. j

2 Current issues
1) if I uncomment  //       project.getPluginManager().apply(net.wasdev.wlp.gradle.plugins.Liberty.class); from GreetingPlugin.java I get a class not found exception,
Trying to figure this out.. after which I hope to have the hello task depend on libertyinstall
2) With the above Commented I get:
* What went wrong:
A problem occurred evaluating root project 'greeting-plugin'.
> Could not find method hello() for arguments [build_363vvk2x48fehqhstx8bw13bk$_run_closure2@41ed809f] on root project 'greeting-plugin' of type org.gradle.api.Project.
