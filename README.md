# API BDD Generator

A simple tool that generates Cucumber BDD feature files and step definitions from API requests.

## Prerequisites
- **Java 11+** installed and on your `PATH`.  
  Verify:
   ```sh
  java -version
   ````

## Usage
Run the JAR with:

```sh
java -jar target/api-bdd-generator-1.0-SNAPSHOT.jar [options]
```

### Examples

* **Generate feature from a cURL command**

  ```sh
  java -jar target/api-bdd-generator-1.0-SNAPSHOT.jar \
    --input "curl -X POST https://api.example.com/login -H 'Content-Type: application/json' -d '{\"user\":\"u\",\"pass\":\"p\"}'" \
    --output ./features
  ```

* **See help options**

  ```sh
  java -jar api-bdd-generator-1.0-SNAPSHOT.jar --help
  ```

## License

MIT License. See [LICENSE](LICENSE) for details.\`\`\`
