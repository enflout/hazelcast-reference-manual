
TODO since this section is not completed, it is not used/linked yet 

## Writing your own Simulator Test

...

### Using Maven Archetypes

Alternatively, you can execute tests using the Simulator archetype. Please see the following.

```
mvn archetype:generate  \
    -DarchetypeGroupId=com.hazelcast.simulator \
    -DarchetypeArtifactId=archetype \
    -DarchetypeVersion=0.5 \
    -DgroupId=yourgroupid  \
    -DartifactId=yourproject
```

This creates a fully working Simulator project, including the test having `yourgroupid`.

1. After this project is generated, go to the created folder and execute the following command.

  ```
  mvn clean install
  ```

2. Then, go to your working folder.

  ```
  cd <working folder>
  ```

3. Edit the `simulator.properties` file as explained in the [Simulator.Properties File Description section](#simulator-properties-file-description).

4. Run the test from your working folder using the following command.

  ```
  ./run.sh
  ```

The output is the same as shown in the [Running the Test section](#running-the-test).
