Error even though BaseClass has configured 

```RestAssuredMockMvc.standaloneSetup(personRestController);```

Generated test shows BaseClass is extended 

```public class ContractVerifierTest extends BaseClass {```

Error: Run ```mvn clean install```

```
[ERROR] validate_find_person_by_id  Time elapsed: 0.125 s  <<< ERROR!
java.lang.IllegalStateException:
You haven't configured a MockMVC instance. You can do this statically

RestAssuredMockMvc.mockMvc(..)
RestAssuredMockMvc.standaloneSetup(..);
RestAssuredMockMvc.webAppContextSetup(..);

or using the DSL:

given().
                mockMvc(..). ..

        at com.example.cdc.ContractVerifierTest.validate_find_person_by_id(ContractVerifierTest.java:27)
```