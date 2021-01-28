# How to release

We use gitflow for development (see A successful git branching model for more details). You could use gitflow with native git commands, but then you would have to change the versions in the poms manually. Therefore we use the mvn gitflow plugin, which handles this and other things nicely.

You can build a release with:

    ./mvnw gitflow:release-start
    ./mvnw gitflow:release-finish

If the gh-actions completes successfully, you can check 

* https://oss.sonatype.org/#nexus-search;quick~axon-framework-bom

to verify, it will take a few hours until the lib is visible on the maven-central index.
